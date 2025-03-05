EXPERIMENT:3 
 # DIFFERENTIAL AMPLIFIER 
## AIM:design and analyze the MOS Differential Amplifier circuit for the following specifications.
## THEORY:
### Differential Amplifier is basically having two inputs and one output.this will amplify the difference between the two input signal ,so this will avoids or rejects the input values if it is come same, means it will rejects the common-mode signals . it is also the building blocks for the operational amplifiers.
###   Differential Amplifier is made up of mosfets only .so let us try to understant the what makes the difference between normal and differential amplifier. 
### 1.The normal and common amplifier has a single input but in case of differential amplifier we have two inputs
### 2.Output will depend on the input value incase of normal amplifier but in differential amplifier ouput is depends on the difference of input signal values.
### 3.Incase of differential amplifier we can see the noise rejection but incase of normal amplifiers it is absent.
### 4.The usage of this amplifiers make them different like Normal amplifiers are used in speakers,radios .But Differential amplifiers are used in operational amplifiers and sensors. so these will makes us difference between normal and differential amplifiers.
### the differential amplifier has high commom-mode rejection ratio,high differential gain,low coomon mode gain.As normal the differential amplifier has input impedence and  low output impedence. good linearity, Wide bandwidthand noise rejection etc.
##  DC analysis:
### DC analysis is basically analysing the current and voltage values of a given circiut.so here we can get a Q point which is very necessary to get a effecient amplified output .So using this analysis we can easyly find out the state of given mosfet.we ca also find the Vgs,Vds,Id,Is and etc. this is all about DC analysis.
## AC analysis:
### ac analysis is nothing but we get an information about the vary of frequency and output voltage.This can also called as small signal analysis.here we put sinosoidal waves and some frequency from this we will get bandwidth and gain of the given responce.
## Transient analysis:
### This analysis is nothing but it will give idea of the output and input waveform.some important information about the voltage gain,phase shift,so thet we can easily get the information about the input and output signal in the desired wave form.
## Circuit daigram of Differential amplifier
![WhatsApp Image 2025-03-05 at 17 41 51_a3f3fdca](https://github.com/user-attachments/assets/9e7176a3-4bd5-40a0-9da6-4995f4a4e855)

### Differential amplifier  is a voltage subtractor circuit which produces an output voltage proportional to the voltage difference of two input signals applied to the inputs of the inverting and non-inverting terminals of an operation.
## PROBLEM STATEMENT:
## Design differential amplifier for the following specifications Vdd=3.3v, P<=3mW, Vicm=1.72V, Vocm=1.81V ,Vp=0.7V. perform DC analysis, transient analysis, AC analysis and extract the required parameters
![WhatsApp Image 2025-03-05 at 17 35 32_3c24aa7e](https://github.com/user-attachments/assets/83aa5970-f471-49ae-bd49-d30385dc0453)
## PROCEDURE:
### 1.Design the required values from the given data like Rd,Rss,Id so that we can do analysis.
### 2.Open the lt spice software and build the circuit in that sofware by creating a file.
### 3.Link the library file (.lib) to the circuit so that it will get the true values of mosfet ,so we can get the accurate value.
### 4.After that introduce the values that are calculated from the problem statement like Rd=3.3k ohm,vdd=3.3v,vism=1.72v,vosm=1.81v,Rss=770.7ohm.
### 5.First do the DC analysis for to get the correct Id , vout ,q point values by varying the W\L Values so that we will get the mosfet working mossfet region.
### 6.Making L=180nm and varying the w  value and Rd values so that we get our desired value.
### 7.After getting a desired and accurate value from DC analysis next move to other analysis.
### 8.Transient analysis is done by giving 5m time interval so we will get input and output waveforms from this find the gain of the amplifier .
### 9.After that analysis,AC Analysis here by changing the voltage source to sinosoidal and giving some values( amplitude=50m,1K frequency,ac value=1)
### 10.From doing this all analysis at last find the Gain values in AC and Transient analysis.
## CIRCUIT_1:
![WhatsApp Image 2025-03-05 at 21 05 01_64a0d84d](https://github.com/user-attachments/assets/fca0c2bb-9fb0-404a-82a9-de47a4eebb39)
### Here the components are used here is two CMOSN , two Rd (3.311755K),1 Rss(0.77K),voltages sources
### the values are given two mosfets( length=180n,width=2.4199u),voltage sources, vdd=3.3v,vism=1.72v,vosm=1.81v
##  DC ANALYSIS:
![image](https://github.com/user-attachments/assets/331fc779-66d9-42a0-8701-0e88c418d477)
### The mosfet is in the saturation , so that having Id=0.00045A,Vout=1.81V,Iss=0.9mA
## TRANSIENT ANALYSIS:
![image](https://github.com/user-attachments/assets/18b59c41-5092-4683-9415-face7488cf05)
###  output waveform of the given circuit using transient analysis.
![image](https://github.com/user-attachments/assets/ff2e8665-c9bb-4bf6-ae5d-5dd9755dbdf2)
###  input waveform of the given circuit using transient analysis.
![image](https://github.com/user-attachments/assets/113a73ac-c6f3-476f-8b2a-41a839de50b2)
### output value=(Vout)=0.11934v
### inputvalue=(Vin)=0.096306v
### Gain=Vout/Vin=1.2391
 ### As per the observation ,the differential amplifier as higher gain compared to normal amplifier , having of 1.2391 gain.
## AC analysis
### All sources are changed from normal to sinosoidal source and giving values(1.72 50m 1K).In simulation selecting the values like ( DECADE,20,0.1 TO 1T[FREQUENCY RANGE])  so that from this analysis we can cross check the gain value. 
![image](https://github.com/user-attachments/assets/21aa2d53-d505-4b03-ba5c-8a125c63d837)
### Gain in db = 20xLog(gain)=?
### 20xLog(1.2391)=1.862124db.
### By obseravtion gain in AC analysis and Transient analysis are foundm to be similar.
## CIRCUIT_2:
![image](https://github.com/user-attachments/assets/3e836622-2522-4be4-9d64-79b956fae913)

### In this circuit the resister RSS=0.77K  by the Current source of value 0.9mA. all other components will remain as it is.
### lets do the simulations for the given changed circuit:
### As per the observation by varying the width and Rd value we got the needed values like Id=0.45mA,Vout=1.81V.
### W=2.4199u,RD=3.211115K ohm 
## DC ANALYSIS:
![image](https://github.com/user-attachments/assets/c7438f31-8530-4cfc-875c-b98287a53a3c)
### Id value and Vout value get corrected by varying some w value and resistance value.
## TRANSIENT ANALYSIS:
![image](https://github.com/user-attachments/assets/b0af37d2-3038-4c1e-8605-28b8f9edc723)
### output waveform of the given circuit using transient analysis.
![image](https://github.com/user-attachments/assets/147fee4a-07b3-4e3d-8fc5-deb22ff4b2fb)
###  input waveform of the given circuit using transient analysis.
![image](https://github.com/user-attachments/assets/33e448c9-17c4-41fa-8233-bf89d9b7cf20)
### output value=(Vout)=0.31187v
### inputvalue=(Vin)=0.1v
### Gain=Vout/Vin=3.1187
 ### As per the observation ,the differential amplifier as higher gain compared to normal amplifier , having of 3.1187 gain.
## AC ANALYSIS:
### All sources are changed from normal to sinosoidal source and giving values(1.72 50m 1K 0 0 0).In simulation selecting the values like ( DECADE,20,0.1 TO 1T[FREQUENCY RANGE])  so that from this analysis we can cross check the gain value. 
![image](https://github.com/user-attachments/assets/2fb7519e-9a40-4cd3-89bd-e4d32f0a485b)
### Gain in db = 20xLog(gain)=?
### 20xLog(3.1187)=0.87947db
### By obseravtion gain in AC analysis and Transient analysis are foundm to be similar.
## CIRCUIT_3:
