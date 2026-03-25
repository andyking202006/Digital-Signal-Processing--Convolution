# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc; % clear screen
%clear all; % clear screen
close all; % close all figure windows

% input sequence
% X[n]={2,−1,4−2.3,5,9,−3} h[n]={3,−4,1,1,2.7,3.5,2}

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');

```



## OUTPUT:
<img width="1600" height="847" alt="image" src="https://github.com/user-attachments/assets/ac7ef96e-e3e0-4955-9815-016a4c3c7170" />
<img width="1600" height="849" alt="image" src="https://github.com/user-attachments/assets/08f4b3a8-2859-4577-b543-99915d82e204" />
<img width="1600" height="851" alt="image" src="https://github.com/user-attachments/assets/9da61cf2-2cc1-491e-bfc1-a9366d1c5006" />



## RESULT:
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/d33773d6-27c3-4771-84c9-bfe554b978b4" />


