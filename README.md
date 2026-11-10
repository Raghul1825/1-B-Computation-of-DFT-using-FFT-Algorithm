# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.

## APPARATUS REQUIRED

PC installed with SCILAB

## PROGRAM 

clc;

clear;

clf;

xn = [1,2,3,4,4,3,2,1];

N = length(xn);

n = 0:N-1;

Xk = fft(xn);

disp("FFT output:");

disp(Xk);

K = 0:N-1;

magnitude = abs(Xk);

phase = atan(imag(Xk), real(Xk));

y = ifft(Xk);

subplot(2,2,1);

plot2d3(n, xn);

xtitle("Input Sequence", "n", "x(n)");

subplot(2,2,2);

plot2d3(K, magnitude);

xtitle("Magnitude Spectrum", "k", "|X(k)|");

subplot(2,2,3);

plot2d3(K, phase);

xtitle("Phase Spectrum", "k", "Phase (radians)");

subplot(2,2,4);

plot2d3(n, real(y));

xtitle("Inverse FFT Output", "n", "x(n)");

### CALCULATIONS:

<img width="702" height="1280" alt="image" src="https://github.com/user-attachments/assets/5ad9ae60-5e6d-41e8-9cfc-50bba4a0934f" />
<img width="736" height="1280" alt="image" src="https://github.com/user-attachments/assets/3d3e1348-6932-4ec0-9847-a369cc0f7273" />
<img width="846" height="1280" alt="image" src="https://github.com/user-attachments/assets/5f6ceac5-f54a-4486-994f-8429e462634c" />
<img width="852" height="1280" alt="image" src="https://github.com/user-attachments/assets/d01698e6-6464-466d-bcf2-d7e8ef3099eb" />

### SAMPLE OUTPUT:

<img width="1228" height="1280" alt="image" src="https://github.com/user-attachments/assets/afef22ea-e047-413e-9a94-b961f4d670fd" />

## RESULT:

<img width="1280" height="724" alt="image" src="https://github.com/user-attachments/assets/c27cb75e-f9bc-48d7-a63c-cb700c345581" />

Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

