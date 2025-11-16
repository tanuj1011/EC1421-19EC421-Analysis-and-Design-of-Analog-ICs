# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
![WhatsApp Image 2025-11-16 at 13 18 15_2261a44a](https://github.com/user-attachments/assets/9a5a82ef-2b2e-4932-8bf9-610f85638a1f)

## HIGH-PASS
![WhatsApp Image 2025-11-16 at 13 18 50_2f426fc8](https://github.com/user-attachments/assets/a90235b0-d1fc-49ca-b763-d86859a78fed)

## BAND-PASS
![WhatsApp Image 2025-11-16 at 13 19 18_7d0ffff5](https://github.com/user-attachments/assets/9f18f54e-c856-4d70-b170-ca03c79540a1)

## MODEL GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-16 at 13 18 29_4bbcce7f](https://github.com/user-attachments/assets/1e2076a0-699a-475e-9af9-d5eb25ea085e)

## HIGH-PASS
![WhatsApp Image 2025-11-16 at 13 19 08_95553731](https://github.com/user-attachments/assets/9f7bfe28-5fe1-4499-b5b0-4e50a5e15633)

## BAND-PASS
![WhatsApp Image 2025-11-16 at 13 19 34_aef8ddfb](https://github.com/user-attachments/assets/086a2de8-4fbf-4f51-bdb1-7665f75af40c)


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
![WhatsApp Image 2025-11-16 at 13 19 53_f85a858e](https://github.com/user-attachments/assets/633a48ab-2290-4d2d-917e-8f0030efa5ae)

## HIGH-PASS
![WhatsApp Image 2025-11-16 at 13 19 45_cba816c5](https://github.com/user-attachments/assets/1c589114-754f-48cc-9311-02b8cefbc907)

## BAND-PASS
![WhatsApp Image 2025-11-16 at 13 20 09_af8f56f6](https://github.com/user-attachments/assets/2ff719c4-9618-42bc-b8b4-26e4e87bd34b)

## GRAPH:
## LOW_PASS
![WhatsApp Image 2025-11-16 at 13 21 36_a4151097](https://github.com/user-attachments/assets/803ddf42-7253-474d-8eac-1f3e6ec8da97)

## HIGH-PASS
![WhatsApp Image 2025-11-16 at 13 21 08_6f2ec120](https://github.com/user-attachments/assets/2590d026-4895-4166-9295-43d5e65894ec)

## BAND-PASS
![WhatsApp Image 2025-11-16 at 13 20 48_b15f101c](https://github.com/user-attachments/assets/7015d91c-c076-4084-9237-4ea54c424e18)


 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

