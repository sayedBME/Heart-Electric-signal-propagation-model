# Heart-Electric-signal-propagation-model
Charging time of capacitor: T_c=0.69×R_2×C || Discharging time of capacitor: T_d=0.69×R_1×C || Total Pulse time: T=0.69(R_1+R_2)C

Let, Charging resistor R2= R4= R6= 1KΩ 
Capacitor, C2=C4=C6=C = 100 µF

For the SA node, the Number of pulse (70-80) per minute
T=0.857 for 70 Pulses per minute
0.857 = 0.69(R_1+1000)×100×〖10〗^(-6)
R1=11.420 KΩ
 
For the AV node, the Number of pulse (40-50) per minute
T=1.2 for 50 Pulses per minute
1.2 = 0.69(R_1+1000)×100×〖10〗^(-6)
R1=16.391 KΩ

For bundle of his and Purkinje fiber, the Number of pulse (30-40) per minute
T=1.71 for 40 Pulses per minute
1.71 = 0.69(R_1+1000)×100×〖10〗^(-6)
R1=20.739 KΩ

I used 555 timer IC for generating pulses. Three IC were used for SA node, AV node and, Bundle of His, respectively. The frequency of pulses depends on C2 Capacitors and R1, R2 Resistors. The value of R2 resistors remains the same, and R1, R3, and R5 values were calculated according to their pulse number per minute. When the SA node was activated then, it created 70 pulses per minute, and the other two timers followed the frequency by giving SA node circuits output to its CV terminals. After switching off SA node circuits, AV node circuits generate pulses with their intrinsic frequency and the Bundle of His circuit followed the AV node circuit’s frequency. When the AV node circuit was switched off the Bundle of His circuits generate pulses with their intrinsic frequency.
