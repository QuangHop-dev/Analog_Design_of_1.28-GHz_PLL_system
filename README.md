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
      <th colspan="2">Thông số</th>
      <th>Giá trị</th>
    </tr>
    <tr>
      <td>Nguồn cung cấp</td>
      <td>V<sub>cc</sub></td>
      <td>1.8 V</td>
    </tr>
    <tr>
      <td>Tần số tham chiếu</td>
      <td>V<sub>ref</sub></td>
      <td>40 MHz</td>
    </tr>
    <tr>
      <td>Tần số ngõ ra</td>
      <td>F<sub>out</sub></td>
      <td>1.28 GHz</td>
    </tr>
    <tr>
      <td>Bộ chia</td>
      <td>N</td>
      <td>32</td>
    </tr>
  </table>
  
</div>
