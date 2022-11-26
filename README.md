- VLSM pada Cisco Packet Tracer

1. Pembuatan Topologi

![](https://lh6.googleusercontent.com/dCbyHDdULqiuvqitjrGkf48Q21BI5irl7tSCyVzGQ9UF0b5lP0-w4jWPUYS1eF5cXSLczgsmjhCkKcNrk4Xr1URVPVgbC3T_aEtv6flFZD4bkS_SzYmMvZ6EozBqoc26rQeDfRtCJnYWpOQ5uxfe7xcteqURzJNiO087n726diEvYExm207tttMPazlFuQ)

2. Pembagian Subnet

![](https://lh6.googleusercontent.com/sdZLGVpT93H36FEB16E3jRTPiIRZUbjf94wNDaX_jikZ_g79KohOv1emCBD6867Ua020mWZa7jMLFPt8nr7lB_V7CUbIet6Itc5TajvS0s_E-KIBf6D1so44jJ2CrFwoMhpeBsIEOmF3-Zdp9wG3MTRZ7WLW5uDZvrfC52b79_ZWvrDaT1c0O5jbqW73yQ)

  


3. Perhitungan dan Persebaran IP

|        |           |         |
| ------ | --------- | ------- |
| Subnet | Jumlah IP | Netmask |
| A1     | 1000      | /22     |
| A2     | 2         | /30     |
| A3     | 50        | /26     |
| A4     | 2         | /30     |
| A5     | 2         | /30     |
| A6     | 2         | /30     |
| A7     | 270       | /23     |
| A8     | 2         | /30     |
| A9     | 120       | /25     |
| A10    | 2         | /30     |
| A11    | 120       | /25     |
| A12    | 70        | /25     |
| A13    | 2         | /30     |
| A14    | 250       | /24     |
| A15    | 2         | /30     |
| A16    | 500       | /23     |
| A17    | 210       | /24     |
| A18    | 2         | /30     |
| Total  | 2608      | /20     |

4. Subnet besar yang kami bentuk memiliki NID 10.42.0.0 dengan netmask /20. Kemudian, kami mulai dengan perhitungan pembagian IP dengan membuat pohon IP seperti gambar berikut:

![](https://lh6.googleusercontent.com/pph-WXn6Q9eUbkDs4Gqoj49m7d8OxPexvr_D7A4m6dfHK8ckJmVS3JCXlGiW9oyOtzw-eu8xImNRNE8qCEeD-8daFy_Kipwe7_w-DZkReK_buWL3rVccg0kYRXGY_lISFKXFv4ETo9wSDLKJQIjqY5uQBWVv3Tuv2OmiGG8kyfVxlDmcNwlFhAlrjHzJMg)

5. Dengan demikian, kami membagi alamat IP yang memungkin sesuai dengan topologi seperti berikut ini

|        |           |         |             |                           |              |
| ------ | --------- | ------- | ----------- | ------------------------- | ------------ |
| Subnet | Jumlah IP | Netmask | Address     | Assignable IP             | Broadcast    |
| A10    | 2         | /30     | 10.42.0.0   | 10.42.0.1 - 10.42.0.2     | 10.42.0.3    |
| A13    | 2         | /30     | 10.42.0.4   | 10.42.0.5 - 10.42.0.6     | 10.42.0.7    |
| A15    | 2         | /30     | 10.42.0.8   | 10.42.0.9 - 10.42.0.10    | 10.42.0.11   |
| A18    | 2         | /30     | 10.42.0.12  | 10.42.0.13 - 10.42.0.14   | 10.42.0.15   |
| A2     | 2         | /30     | 10.42.0.16  | 10.42.0.17 - 10.42.0.18   | 10.42.0.19   |
| A4     | 2         | /30     | 10.42.0.20  | 10.42.0.21 - 10.42.0.22   | 10.42.0.23   |
| A5     | 2         | /30     | 10.42.0.24  | 10.42.0.25 - 10.42.0.26   | 10.42.0.27   |
| A6     | 2         | /30     | 10.42.0.28  | 10.42.0.29 - 10.42.0.30   | 10.42.0.31   |
| A8     | 2         | /30     | 10.42.0.32  | 10.42.0.33 - 10.42.0.34   | 10.42.0.35   |
| A3     | 50        | /26     | 10.42.0.64  | 10.42.0.65 - 10.42.0.126  | 10.42.0.127  |
| A12    | 70        | /25     | 10.42.0.128 | 10.42.0.129 - 10.42.0.254 | 10.42.0.255  |
| A11    | 120       | /25     | 10.42.1.0   | 10.42.1.1 - 10.42.1.126   | 10.42.1.127  |
| A9     | 120       | /25     | 10.42.1.128 | 10.42.1.129 - 10.42.1.254 | 10.42.1.255  |
| A17    | 210       | /24     | 10.42.2.0   | 10.42.2.1 - 10.42.2.254   | 10.42.2.255  |
| A14    | 250       | /24     | 10.42.3.0   | 10.42.3.1 - 10.42.3.254   | 10.42.3.255  |
| A7     | 270       | /23     | 10.42.4.0   | 10.42.4.1 - 10.42.5.254   | 10.42.5.255  |
| A16    | 500       | /23     | 10.42.6.0   | 10.42.6.1 - 10.42.7.254   | 10.42.7.255  |
| A1     | 1000      | /22     | 10.42.8.0   | 10.42.8.1 - 10.42.11.254  | 10.42.11.255 |
