# STIMULATION-OF-AUTOCORRELATION-AND-PSD-USING-SCILAB
AUTOCORRELATION-AND-PSD
#EXP NO 7 SIMULATION OF AUTOCORRELATION AND PSD USING SCILAB

AIM: Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

EQUIPMENTS Needed

• Computer with i3 Processor • SCI LAB

THEORY: The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

Algorithm

Load or Define the Signal: Input your time-domain signal.
Compute Autocorrelation: Calculate the autocorrelation function of the signal.
Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.
Plot Results: Visualize the autocorrelation function and PSD.
PROCEDURE

• Refer Algorithms and write code for the experiment. • Open SCILAB in System • Type your code in New Editor • Save the file • Execute the code • If any Error, correct it in code and execute again • Verify the generated waveform using Tabulation and Model Waveform

PROGRAM:
~~~
clc
clear all; 
t=0:0.01:2*3.14;
x=sin(6*t);
 subplot(3,2,1);
  plot(x); 
  au=xcorr(x,x);
subplot (3,2,2);
 plot (au);
  v=fft(au);
   subplot(3,2,3);
plot(abs(v));
 fw=fft(x);
  subplot(3,2,4);
   plot(real(fw),imag(fw)); 
   fw2=(abs(fw)).^2;
subplot(3,2,5);
 plot(fw2);
~~~
OUTPUT

<img width="1762" height="870" alt="image" src="https://github.com/user-attachments/assets/d437963a-a41c-4ea6-8d20-65c9520205f7" />

RESULT: Thus the Autocorrelation and PSD are executed in Scilab and output is verified.

