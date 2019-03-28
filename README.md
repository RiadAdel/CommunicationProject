# CommunicationProject
## Steps of BER performance figure:
1. Add "to workspace" block to your diagram, name it "ber", and connect its input with the BER output.
2. Change the AWGN channel Eb/No value to the variable "EbNo".
3. Open bertool from matlab commandline, to open the ber analysis tool.
4. from theoretical choose the modulation type and change the range to (-10:10) then click plot.
5. then from Monte Carlo choose your modulation file and write your BER var name (here is "ber") then Run.

## Steps of Scatter figure:
- All what you need for scatter figure is to use "constellation diagram" component and connect its input with the output of the signal after modulation, and another constellation diagram to connect it with the signal after AWGN channel.
- when you run the simulation the scatter figures with appear automatically.

#### parameters changes from one modulation to another:
  1. Size set at Random Integer Generator: this number should be = 2^(number of bit/symbo)
  2. Number of bits/symbo at AWGN
  
## 1. BPSK
  - it's a phase-shift keying (**PSK**) modulation that use two phases with difference 180 degree, so it can handle the noise due to the big difference in phase.
  - it modulates at 1 bit/symbo so it's slow and not working with high data-rate applications.
<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/BPSK/Before%20Noise.PNG" width="400" title="modulated signal before noise"/> <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/BPSK/After%20Noise.PNG" width="400" title="modulated signal after noise"/>

<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/BPSK/BPSK.jpg" title="BER bs Eb/No"/>

## 2. QPSK
  - it's also a **PSK** modulation but QPSK uses four points on the constellation diagram (*four phases*)
  - it modulates at 2 bit/symbo
  
<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QPSK/before.png" width="400" title="modulated signal before noise"/> <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QPSK/after.png" width="400" title="modulated signal after noise"/>

<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QPSK/QPSK.jpg" title="BER bs Eb/No"/>

## 3. 16 QAM
  - Quadrature Amplitude Modulation, utilises both amplitude and phase components to provide a form of modulation that is able to provide high levels of spectrum usage efficiency.
  - it modulates at 4 bit/symbo
  
<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-16/before.png" width="400" title="modulated signal before noise"/> <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-16/after.png" width="400" title="modulated signal after noise"/>

<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-16/QAM16.jpg" title="BER bs Eb/No"/>

## 4. 64 QAM
  - Same as 16 QAM but with higher modulation rate.
  - it modulates at 6 bit/symbo

<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-64/before.png" width="400" title="modulated signal before noise"/> <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-64/after.png" width="400" title="modulated signal after noise"/>

<img src="https://github.com/RiadAdel/CommunicationProject/blob/master/QAM-64/QAM64.jpg" title="BER bs Eb/No"/>

## 5. FSK
  - Frequency-shift keying modulation that use a discrete frequency changes of a carrier signal to transmit the digital informations.
  
  <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/FSK/before.png" width="400" title="modulated signal before noise"/> <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/FSK/after.png" width="400" title="modulated signal after noise"/>
  
  <img src="https://github.com/RiadAdel/CommunicationProject/blob/master/FSK/FSK.jpg" title="BER bs Eb/No"/>
