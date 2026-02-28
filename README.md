# Analog_Design_of_1.28-GHz_PLL_system
This project shows the design of a frequency synthesizer PLL system that produces a 1.28 GHz signal with a reference input of 40 MHz

## [1] PLL System Design
- PLL block diagram:
<p align="center">
  <img width="1274" height="353" alt="image" src="https://github.com/user-attachments/assets/eaddff0b-41b7-4847-b4a3-de91239bd2bf" />
</p>

- Typical CP PLL system:
<p align="center">
  <img width="510" height="324" alt="image" src="https://github.com/user-attachments/assets/532d5a7f-5173-4d0e-800e-2e78df805916" />
</p>

### System requirements table:
<div align="center">
  
  <table>
    <tr>
      <th colspan="2">Parameter</th>
      <th>Values</th>
    </tr>
    <tr>
      <td>Supply Power</td>
      <td>V<sub>cc</sub></td>
      <td>1.8 V</td>
    </tr>
    <tr>
      <td>Reference Frequency</td>
      <td>V<sub>ref</sub></td>
      <td>40 MHz</td>
    </tr>
    <tr>
      <td>Output Frequency</td>
      <td>F<sub>out</sub></td>
      <td>1.28 GHz</td>
    </tr>
    <tr>
      <td>Devider</td>
      <td>N</td>
      <td>32</td>
    </tr>
  </table>
  
</div>

### Circuit Simulation on Virtuoso

<p align="center">
  <img width="972" height="424" alt="image" src="https://github.com/user-attachments/assets/773d4f3b-3900-4d4b-b740-b861dd2b1b37" />
</p>

## [2] PLL Circuit Design
### A) PFD:
<p align="center">
  <img width="701" height="626" alt="image" src="https://github.com/user-attachments/assets/993e16e2-18e4-465b-a6e5-20ef7f18af7b" />
</p>

### B) Charge Pump:
<p align="center">
  <img width="661" height="684" alt="image" src="https://github.com/user-attachments/assets/7f61f641-f37c-4026-a158-948130f7db67" />
</p>

### C) Loop Filter:
<div align="center">
  <table align="center">
    <tr>
      <th colspan="2">Parameter</th>
      <th>Value</th>
    </tr>
    <tr>
      <td>Charge Pump Current</td>
      <td>I<sub>CP</sub></td>
      <td>100 µA</td>
    </tr>
    <tr>
      <td rowspan="3">Loop Filter</td>
      <td>R1</td>
      <td>6 kΩ</td>
    </tr>
    <tr>
      <td>C1</td>
      <td>40 pF</td>
    </tr>
    <tr>
      <td>C2</td>
      <td>4 pF</td>
    </tr>
  </table>
</div>

### D) VCO:
Refer to: https://ieeexplore.ieee.org/document/7475300/
<p align="center">
  <img width="979" height="414" alt="image" src="https://github.com/user-attachments/assets/93e8479b-0ae4-4f18-93e9-a67373684b03" />
</p>

### E) Divider:
<p align="center">
  <img width="979" height="279" alt="image" src="https://github.com/user-attachments/assets/e6991827-4d76-4160-aeb2-3ef73ce71a61" />
</p>

## => System Simulation
<p align="center">
  <img width="979" height="394" alt="image" src="https://github.com/user-attachments/assets/a4f5e4d3-7213-4ba4-8245-6440807cb575" />
</p>

---

## References
[1] P. T. Patil, V. Ingale, "Design of a Low Power PLL in 90nm CMOS Technology," 2019 IEEE 5th International Conference for Convergence in Technology (I2CT), pp. 1-4, 2019.
[2] M. D. K. Naik, "Design and Analysis of Efficient Phase Locked Loop," Bachelor’s Thesis, National Institute of Technology, India, 2015.
[3] G. Bhargav, G. Prasad, S. D. Canchi, B. Chanikya, "Design and Analysis of Phase Locked Loop in 90nm CMOS," 2016 Thirteenth International Conference on Wireless and Optical Communications Networks (WOCN), pp. 1-7, 2016.
[4] Roland E. Best, Phase-Locked Loops: Design, Simulation, and Applications, Fifth Edition, McGraw-Hill Education, 2003, pp. 11-16.
[5] Behzad Razavi, Design of Analog CMOS Integrated Circuits, Second Edition, McGraw-Hill Education, 2017, pp. 651-685.
[6] Jeffrey S. Pattavina, "Charge-Pump Phase-Locked Loop – A Tutorial," [Online]. Available: https://www.eetimes.com/charge-pump-phase-locked-loopa-tutorial-part-i/. [Accessed: 30-May-2025].
[7] Sandhiya S, Revathi S, Dr. B. Vinothkumar, "Design of Voltage Controlled Oscillator in 180 nm CMOS Technology," International Research Journal of Engineering and Technology (IRJET), vol. 5, no. 3, pp. 1347-1351, 2018.
[8] Kunjan Devendra Shinde, "Design and implementation of 1 GHz Current Starved Voltage Controlled Oscillator (VCO) for PLL using 90nm CMOS technology," 2015 International Conference on Control, Instrumentation, Communication and Computational Technologies (ICCICCT), 2015.
