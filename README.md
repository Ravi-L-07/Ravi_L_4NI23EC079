# Ravi_L_4NI23EC079
# EXPERIMENT 1: Analysis of CS amplifier
## AIM:
### Demonstrating AC analysis,Transient analysis and DC analysis for CS Amplifier using LT spice software.Then finding Bandwidth,gain and etc,
## COMPONENTS REQUIRED:
### Resistor(1K ohm ),Mosfet(CMOSN,CMOSP),Voltage sources(1.8v,0.6v,0.3v),ground.

## THEORY:
### Mosfet is a elcetronic base component and we can say it as "fundamental and basic unit of Electronic components", which is neccesory to build IC circuit.Mosfet is a three terminal device gate,drain and source.we also have 2types of mosfet pmos and nmos which have different terminologies,properties and applications.
###  The amplifier is nothing but it is an application of mosfet.here it will recieve the weak signal and make it amplify or it will increases the amplitude of signal.it is amplyfy the signal which is in the form of power or voltage.By taking milivoltage making it to 10v-100v voltage so efficiency is also more.
### The common source Amplifier which is a voltage amplifier which is related frequency response.we can see the variation of output voltage with varing the frequency.Here the input and output both are having commom source for this reason it is called as CS AMPLIFIER.The CS Amplifier output is 180 phase shifted so we get output and input having different phases. 
### The mosfet will work as amplifier in the region of saturation . so we can do the amplification of the signal without clipping using DC bias (Q point).If Mosfet works in perfect region means in saturation ragion ,some voltage and current value is needed so it is basically called as biasing point.
### The current equation for drain current is given by Id=kn/2*w/l*Vov*Vov.
### where Id is drain current,w is the width, l is the length and Vov is the overdrive voltage which is basically vgs-vt.
## AC analysis:
### ac analysis is nothing but we get an information about the vary of frequency and output voltage.This can also called as small signal analysis.here we put sinosoidal waves and some frequency from this we will get  bandwidth and gain of the given responce.
## DC anaysis:
### DC analysis is basically analysing the current and voltage values of a given circiut.so here we can get a Q point which is very necessary to get a effecient amplified output .So using this analysis we can easyly find out the state of given mosfet.we ca also find the Vgs,Vds,Id,Is and etc. this is all about DC analysis.
## Transient Analysis:
### This analysis is nothing but it will give idea of the output and input waveform.some important information about the voltage gain,phase shift,so thet we can easily get the information about the input and output signal in the desired wave form.

## CIRCUIT-1:
 ![WhatsApp Image 2025-02-16 at 21 50 09_9134c06f](https://github.com/user-attachments/assets/cd915bc0-424b-4cff-925b-1e54a9e051eb)
## PROCEDURE:
### 1.Open the ltspice software,merge the library file for getting accurate values of NMOS and PMOS.
### 2.Select the components which are needed to us like for circuit 1 we need 1k resistor,1 CMOSN,two voltage sources(1.8v,0.6v),ground from the components list.
### 3.Place them all components in  necessory way which is helpfull ,connect  all the components as in  given circuit .
### 4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.
### 5.lets do the DC Analysis first by opting a simulation , we get .op so after placing it we will get the values of it. thet will displayed.
### 6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.
### 7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform( 0.6,50m,1T),after that select the AC simulation from the given options of simulation after giving values of ( Decade,20,01,1T).So we will get a output after placing node to output waveform .
### 8.Here we put the values of l=180nm,w=1.08um,etc

## DC ANALYSIS:
![WhatsApp Image 2025-02-16 at 21 52 41_c0fb03d1](https://github.com/user-attachments/assets/37c9754e-1d00-4734-9991-294ead09bf2b)
### Id = 2.7*e-5 A
### Vds = 1.772v
### W = 1.08um and L=180nm.
### source voltage = 1.8v and 0.9v
## AC ANALYSIS:
![WhatsApp Image 2025-02-16 at 23 01 49_df6fee78](https://github.com/user-attachments/assets/86c64380-4b13-429d-9b9c-64340e6e6fe3)
## TRANSIENT ANALYISIS:
### INPUT WAVEFORM:
![WhatsApp Image 2025-02-17 at 22 05 45_c29ad6df](https://github.com/user-attachments/assets/2b085277-a172-4bc5-bd91-6813642b00aa)
### input voltage= 200mv p-p
### OUPUT WAVEFORM:
![WhatsApp Image 2025-02-17 at 22 04 53_440c8196](https://github.com/user-attachments/assets/b9ca85c9-f610-4176-8954-c0d47f2106b6)
### output voltage= 0.5 v p-p.
## CALCULATIONS:
### GIVEN : power= 50um ,l=180nm,vdd= 1.8v.
### so that P=VI, I=2.7*e-5 after calculation.
### frequency 1k hz, V1=1.8V, V2=0.6V .
## INFERENCE:
### 1.The mosfet will work as amplifier when it is saturation region only so by doing the DC analysis of a given circuit will get the DC operating point.
### 2.In mosfet ,during the saturation region current ID Is directly proportional to the width means id will vary with w/l ratio linearly.so that our task is to find the W value by given values of length,current id ,voltage v1 and v2.
### 3.From doing AC analysis ,we can find the bandwidth,gain from the given graph we can find the values.
### 4.From Transient analysis,we can get the waveform of input and output waveform.we can find the voltage value.mosfet gain will increases with midband freqency range.
### 5. From this we find the Q point (1,644v,2.7e^-5 A),Vout=0.5v,Vin=200mv.
## CIRCUIT-2:
![WhatsApp Image 2025-02-17 at 18 40 01_ad05334f](https://github.com/user-attachments/assets/af1cde04-fec0-4c6b-842a-2c21b0e70c71)
## PROCEDURE:
### 1.Open the ltspice software,merge the library file for getting accurate values of NMOS and PMOS.
### 2.Select the components which are needed to us like for circuit 1 we need PMOS4,1 CMOSN,three voltage sources(1.8v,o.3v,0.6v),ground from the components list.
### 3.Place them all components in  necessory way which is helpfull ,connect  all the components as in  given circuit .
### 4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.
### 5.lets do the DC Analysis first by opting a simulation , we get .op so after placing it we will get the values of it. thet will displayed.
### 6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.
### 7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform( 0.6,50m,1T),after that select the AC simulation from the given options of simulation after giving values of ( Decade,20,01,1T).So we will get a output after placing node to output waveform .
### 8.Here we put the values of l=180nm,w=134u and w=1.08u in CMOSN and CMOSP.
## DC ANALYSIS:
![WhatsApp Image 2025-02-17 at 18 30 36_c5470592](https://github.com/user-attachments/assets/17c8da2f-cbfa-4800-9e6b-33bd0538073f)
id=2.7e^-5A, Vds=1.79v , source voltage = 1.8v,0.9v ,0.3 v 
## AC ANALYSIS:
![WhatsApp Image 2025-02-17 at 18 39 26_3db155da](https://github.com/user-attachments/assets/af3ceaa3-2555-4187-87aa-ce82e2d4f111)
## TRANSIENT ANALYSIS:
### INPUT WAVEFORM:
![WhatsApp Image 2025-02-17 at 18 31 42_32571ea2](https://github.com/user-attachments/assets/beec3c12-29d1-40ef-9f5e-003d3b27c37b)
### OUTPUT WAVEFORM:
![WhatsApp Image 2025-02-17 at 18 31 42_32571ea2](https://github.com/user-attachments/assets/a0028549-2c7b-4872-9c9d-65fcd468b615)
## CALCULATION:
### GIVEN : power= 50um ,l=180nm,vdd= 1.8v.
### so that P=VI, I=2.7*e-5 after calculation.
### frequency 1k hz, V1=1.8V, V2=0.6V .
### W=134u(CMOSP),W=1.08u(CMOSN)
## INFERENCE:
### 1.The mosfet will work as amplifier when it is saturation region only so by doing the DC analysis of a given circuit will get the DC operating point.
### 2.In mosfet ,during the saturation region current ID Is directly proportional to the width means id will vary with w/l ratio linearly.so that our task is to find the W value by given values of length,current id ,voltage v1 and v2.
### 3.From doing AC analysis ,we can find the bandwidth,gain from the given graph we can find the values.
### 4.From Transient analysis,we can get the waveform of input and output waveform.we can find the voltage value.mosfet gain will increases with midband freqency range.
### 5. From this we find the Q point (1.772V,2.7*e^-5A),Vin= 100mv  vout=0.5mv
# THANK YOU
 
