
# BPSK Modulation Scheme

### Brief explanation
#### BPSK runs 2 shift phases seperated by 180 degerees on the carrier to represent '0' and '1',this limits its bit rate to only #### 1 bit/symbol but it also makes it very immune to noise as it requires a geat deal of distortion before the demodulator
#### fails to recover the original signal.

### Instructions to reproduce the figures
* Random integer generator 
    * set M-ary number to 2
### Scatter plots
![](Scatter_Plots/BPSK1.PNG?raw=true)
![](Scatter_Plots/BPSK2.PNG?raw=true)





### BER performance figure

![](Ber_figures/BPSK_BER.png?raw=true)

## using raised cosine filters

![](Scatter_Plots/BPSK1_cosine.PNG?raw=true)
![](Scatter_Plots/BPSK2_cosine.PNG?raw=true)
### BER performance figure
![](Ber_figures/BPSK_BER_COSINE.png?raw=true)

# QPSK Modulation Scheme

### Brief explanation
#### QPSK uses four shift phases which means it can transmit twice the bit rate of BPSK in the same bandwidth,it is equivelant #### to QAM-4 with respect to the resulting modulated signal and bit rate.However it is less immune to noise than BPSK and 
#### requires a more complex circuit. 
### Instructions to reproduce the figures
* Random integer generator 
    * set M-ary number to 4
### Scatter plots
![](Scatter_Plots/QPSK1.PNG?raw=true)
![](Scatter_Plots/QPSK2.PNG?raw=true)

## using raised cosine filters

![](Scatter_Plots/QPSK1_cosine.PNG?raw=true)
![](Scatter_Plots/QPSK2_cosine.PNG?raw=true)


### BER performance figure


![](Ber_figures/QPSK_BER.png?raw=true)

## using raised cosine filters

![](Scatter_Plots/QPSK1_cosine.PNG?raw=true)
![](Scatter_Plots/QPSK2_cosine.PNG?raw=true)
### BER performance figure
![](Ber_figures/QPSK_BER_COSINE.png?raw=true)
# FSK Modulation Scheme

### Brief explanation
#### Frequency shift key modulation represents the digital information as variations in the frequency of the carrier signal , a #### high frequency represents '1' and a low frequency represents '0'.
### Instructions to reproduce the figures
* Random integer generator 
    * set M-ary number to 8
### Scatter plots
![](Scatter_Plots/FSK1.PNG?raw=true)
![](Scatter_Plots/FSK2.PNG?raw=true)

## using raised cosine filters

![](Scatter_Plots/FSK1_cosine.PNG?raw=true)
![](Scatter_Plots/FSK2_cosine.PNG?raw=true)


### BER performance figure


![](Ber_figures/FSK_BER.png?raw=true)

## using raised cosine filters

![](Scatter_Plots/FSK1_cosine.PNG?raw=true)
![](Scatter_Plots/FSK2_cosine.PNG?raw=true)
### BER performance figure
![](Ber_figures/FSK_BER_COSINE.png?raw=true)
# QAM-16 Modulation Scheme

### Brief explanation
#### As an AM modulation Scheme ,QAM transmits information by changing the amplitude of the carrier wave. It can send a number #### of signals which are out of phase in the same bandwidth, however since the mean energy is the same for all bit rates , the #### higher the bit rate , the easier it becomes for the signal to be distorted by noise.  
### Instructions to reproduce the figures
* Random integer generator 
    * set M-ary number to 16
* Rectangular QAM Modulator Baseband
    * M-ary number = 16
    * Normalization method = average power
### Scatter plots
![](Scatter_Plots/QAM16_1.PNG?raw=true)
![](Scatter_Plots/QAM16_2.PNG?raw=true)



### BER performance figure


![](Ber_figures/QAM16_BER.png?raw=true)

## using raised cosine filters

![](Scatter_Plots/QAM16_1_cosine.PNG?raw=true)
![](Scatter_Plots/QAM16_2_cosine.PNG?raw=true)
## using raised cosine filters
![](Ber_figures/QAM16_BER_COSINE.png?raw=true)
# QAM-64 Modulation Scheme

### Brief explanation
QAM-64 functions like QAM-16 but a higher bit rate and consequently a higher bit rate error.
### Instructions to reproduce the figures
* Random integer generator 
    * set M-ary number to 64
* Rectangular QAM Modulator Baseband
    * M-ary number = 64
    * Normalization method = average power
### Scatter plots
![](Scatter_Plots/QAM64_1.PNG?raw=true)
![](Scatter_Plots/QAM64_2.PNG?raw=true)
## using raised cosine filters

![](Scatter_Plots/QAM64_1_cosine.PNG?raw=true)
![](Scatter_Plots/QAM64_2_cosine.PNG?raw=true)

### BER performance figure

![](Ber_figures/QAM64_BER.png?raw=true)
## using raised cosine filters

![](Scatter_Plots/QAM64_1_cosine.PNG?raw=true)
![](Scatter_Plots/QAM64_2_cosine.PNG?raw=true)
### BER performance figure
![](Ber_figures/QAM64_BER_COSINE.png?raw=true)
### General 
    * sample time = 1
    * tick Frame-based output
    * samples per frame = 100
* AWGN channel
    * EbNo (dB) : EbNo
* Error Rate Calculation
    * output data: port
### using raised cosine filter
* In raised cosine trnsmit/receive set rolloff factor to 0.5 and filter span to 2
* In Error rate calculation set receive delay to 2
