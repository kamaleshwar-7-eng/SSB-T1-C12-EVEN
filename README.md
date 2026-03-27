# SSB-T1-C12-EVEN
# AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

# EQUIPMENTS NEEDED:

  *Computer with i3 Processor

  *SCI LAB

# ALGORITHM:

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x)=sin(x) or any other function.
Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.
Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
Display Results: Output the computed mean variance and Cross Correlation

# PROCEDURE:

1.Refer Algorithms and write code for the experiment.

2.Open SCILAB in System

3.Type your code in New Editor

4.Save the file

5.Execute the code If any Error, correct it in code and execute again

6.Verify the generated results

# PROGRAM:
```matlab
ac=20;  
Am=10; 
fc=3830;
fm=383;
fs=38300; 
t=0:1/fs:2/fm; 
wc=2*3.14*fc; wm=2*3.14*fm;
e1=(Am*sin(wm*t));
subplot(4,1,1);
plot(t,e1); 
e2=(ac*sin(wc*t)); 
subplot(4,1,2); 
plot(t,e2);
sbsc1=(Am/2.*cos(wc*t-wm*t))-(Am/2.*cos(wc*t+wm*t));
sbsc2=(Am/2.*cos(wc*t-wm*t))+(Am/2.*cos(wc*t+wm*t)); 
e3=(sbsc2)+(sbsc1); 
subplot(4,1,3);
plot(t,e3);
e4=(sbsc2)-(sbsc1); 
subplot(4,1,4); 
plot(t,e4);
xgrid;
```

# OUTPUT GRAPH:

<img width="1532" height="993" alt="FM Modulation using scilab" src="https://github.com/user-attachments/assets/86045ad9-1371-4ded-995c-9df4665e4776" />

# TABULAR COLUMN:

![SSBSC Table](https://github.com/user-attachments/assets/8dd288fd-9786-4974-b6fa-7ea76fffb8d4)


# RESULT:
Thus, the SSB-SC-AM Modulation and Demodulation is experimentally done and the output is verified.

