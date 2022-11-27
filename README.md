# Jarkom-Modul-4-ITA05-2022

---

| Nama                            |    NRP     |
| ------------------------------- | :--------: |
| Muhammad Hanif Fatihurrizqi     | 5027201068 |
| Abadila Barasmara Bias Dewandra | 5027201052 |
| Fadly Rachman Drajad Juliantono | 5027201038 |


- VLSM pada Cisco Packet Tracer

1. Pembuatan Topologi

![](https://lh6.googleusercontent.com/erNODoJoKMD0IL9rsfEU8BqW1NiQkvV06AcUOGFU0VYc5UON4tUmoWghCuIt2Quaw6_UXN-7SKThplXv6nX6CZBD97qMj5psRighuFjCegEk0HZU5rt50hGASPthRntrPXPW74ofVuOawGaI7hcMLVfWyHHE1OwkiNJNwqL3PqQl1S3vVi6gTjiRbE1wfQ)

2. Pembagian Subnet

![](https://lh5.googleusercontent.com/37YxLFqmeYwwdKCqgNa7hGYplhDqqcL9YRtgvSMHtYSvhmjSsCPK5jo4XsMq5iWD6J1sivQAdDeq1TBQqn-pMFEPPE-qGkV-YnUlS_tZPuPRhG7vC8ApYTHC8qzB2PiSs7at1cOnUkmPijbufxtdIDdELJwZ_qlhnG49gyx9ClSuu86dcjr9YKeRHIveTQ)

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

![](https://lh4.googleusercontent.com/JdnzToprGuNOb6fsc4OVmjO6nh_RwQCkNX8wdbnjj4j8LZAcZTi8n2tEpdKZR2mqQPrq34sFwqh98pxTpsbhS5shoRgqNzo399RH1GWr0Enw_eucVi-G4fueSbMWYSbzO0W2l_MBEtydKd_y0KH60myj7zYdBkb2deWnsJm0FRNXnT92jkjJsX6-qyQlfA)

5. Dengan demikian, kami membagi alamat IP sesuai dengan urutan yang memungkin sesuai dengan topologi seperti berikut ini

|        |           |         |             |                           |              |                 |
| ------ | --------- | ------- | ----------- | ------------------------- | ------------ | --------------- |
| Subnet | Jumlah IP | Netmask | Address     | Assignable IP             | Broadcast    | Subnet Netmask  |
| A10    | 2         | /30     | 10.42.0.0   | 10.42.0.1 - 10.42.0.2     | 10.42.0.3    | 255.255.255.252 |
| A13    | 2         | /30     | 10.42.0.4   | 10.42.0.5 - 10.42.0.6     | 10.42.0.7    | 255.255.255.252 |
| A15    | 2         | /30     | 10.42.0.8   | 10.42.0.9 - 10.42.0.10    | 10.42.0.11   | 255.255.255.252 |
| A18    | 2         | /30     | 10.42.0.12  | 10.42.0.13 - 10.42.0.14   | 10.42.0.15   | 255.255.255.252 |
| A2     | 2         | /30     | 10.42.0.16  | 10.42.0.17 - 10.42.0.18   | 10.42.0.19   | 255.255.255.252 |
| A4     | 2         | /30     | 10.42.0.20  | 10.42.0.21 - 10.42.0.22   | 10.42.0.23   | 255.255.255.252 |
| A5     | 2         | /30     | 10.42.0.24  | 10.42.0.25 - 10.42.0.26   | 10.42.0.27   | 255.255.255.252 |
| A6     | 2         | /30     | 10.42.0.28  | 10.42.0.29 - 10.42.0.30   | 10.42.0.31   | 255.255.255.252 |
| A8     | 2         | /30     | 10.42.0.32  | 10.42.0.33 - 10.42.0.34   | 10.42.0.35   | 255.255.255.252 |
| A3     | 50        | /26     | 10.42.0.64  | 10.42.0.65 - 10.42.0.126  | 10.42.0.127  | 255.255.255.192 |
| A12    | 70        | /25     | 10.42.0.128 | 10.42.0.129 - 10.42.0.254 | 10.42.0.255  | 255.255.255.128 |
| A11    | 120       | /25     | 10.42.1.0   | 10.42.1.1 - 10.42.1.126   | 10.42.1.127  | 255.255.255.128 |
| A9     | 120       | /25     | 10.42.1.128 | 10.42.1.129 - 10.42.1.254 | 10.42.1.255  | 255.255.255.128 |
| A17    | 210       | /24     | 10.42.2.0   | 10.42.2.1 - 10.42.2.254   | 10.42.2.255  | 255.255.255.0   |
| A14    | 250       | /24     | 10.42.3.0   | 10.42.3.1 - 10.42.3.254   | 10.42.3.255  | 255.255.255.0   |
| A7     | 270       | /23     | 10.42.4.0   | 10.42.4.1 - 10.42.5.254   | 10.42.5.255  | 255.255.254.0   |
| A16    | 500       | /23     | 10.42.6.0   | 10.42.6.1 - 10.42.7.254   | 10.42.7.255  | 255.255.254.0   |
| A1     | 1000      | /22     | 10.42.8.0   | 10.42.8.1 - 10.42.11.254  | 10.42.11.255 | 255.255.252.0   |

Cheatsheet : 

![](https://lh6.googleusercontent.com/1hFjcenolrlcWXJzvxFWzL4Db4nvoIXukp2g2xDYz9htOrrQfW4kMTjMnVR5-6vyVAD6JV-OTAI5aV6eCxGZNvsqLbeNLt6OG-Sb-D52dH1SxjbRs6mJCRd-SEoNK_kvMWbAtZRw8H5j9xccZm-wfjo9g7tDuiIpCcqiXQbkg2bOB_p43uP-vnzr03ptFQ)

6. Konfigurasi 

Tiap masing-masing interface akan di set IP sesuai dengan tabel pembagian yang telah kami buat.

1. The Resonance (Sebagai Router)

- The Resonance mengarah ke The Beast melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/HMCVrU05fKkpvV4zjSJ6Gd3vyDEcvoDedvKwJl5rRfSNVMgpKZNcXgo02W3KlwfP2ZeaA_Hm49Pnm3mLr90PiP_0GD4GEeLlC6NT4b4RzDLSApR2NugvLyj_k3DL6Y9339YKvO11Msjv7vxzbu1eOedFQ2pd5tYsdwaSmfPyowAaiqYONMngsA-pc_L7rQ)

- The Resonance mengarah ke Router The Magical melalui Eth 1/1 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/FV-BbOmU8QtaYkWD9jxNLmOO1xIH-qCqgZcvQYX6bI4layzKKXaB5oj99PpkN0yGKyw1DLNNDjeNP3atLdjz0A4oh5i63Oh7ughaQX2vmZkftaffDCA-gAfQT00-ywWx1lciNjaoJA_zuzfXb7ooT7CYcCCHXI9F5cVTAaK5jToQPsV-fI08zh6gdoaoZw)

  
  
  


- The Resonance mengarah ke Router The Order melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/d4WYOlYvUlOzspCxqqZDYBAOICbmRgaHSyFzAdeSxq2bIRwxYtlgzHs2eYHXbSVoBzqDSldTOtx0ekSXtvDRkGBvQGC8-NBVltoaCTs9GsSo00nSst9Ya_URyvCrk2wfokE4Zq3ctCt-qxpib02Pafi7SUAJFZ52b5vGvEMTi-eSY14Op8VFxqTPABUs1w)

- The Resonance mengarah ke Router The Instrument melalui Eth 1/2 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/G5wS56OOJs1uxfj9eWMcVVEHtsfrAQqvEehLr89l1t90vnascLXbs_Z3SciLMO_clPuoNoa6ecUl3SInY87l0Wzetk9jUfPfiTL9joLohJzziKtvLcz8YnZCL4E2NKCApao1EjlxrimqezaG3RqFIWp1eg7AH9nwcrmvjTPEQFjSBo_kAuqWl2PVFEoDbw)

  
  


2. The Beast (Sebagai Server)

- The Beast mengarah ke Router The Resonance melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/Bf3Ul2MdfX7ZPyUeidqdHUiTjURGLIFU7rbRUVMghDFFImIVMD9wmRIm59eOZnjhZbPuKJQjvHXBfRr9G7IU-o7UurwdeDk2kXiBuACs6FMHLbAa5_VIhcZ2xrGMnNWu3WQkR0ZP3DX1v7vBTVyanz9wiAvCH1q2mba_t32A1fl4mKq0aXNypGktyWJokQ)

3. The Order (Sebagai Router)

- The Order mengarah ke Router The Resonance melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/3qASeLqxtDuryG1NiSWlNrZDs2jNMlmksb3v9o4YhRdKvBfKctqKsVvtY5SM_iFVlydwojQVHeNvcd3bhamf6VzDhZt5edWBwxyvqafjFcRr8qA_L2aXjmF4oRaSO0VO6-U-yd5tSSAKoqWKgBSTpQWp8BCwV-c0MhsRze7C5ZLfaxcDyV3iqr5Ms-A6CA)

  
  
  
  
  
  
  
  
  
  
  
  


- The Order mengarah ke Client Ashaf melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh3.googleusercontent.com/tbi7lZdr7pgrfH9Q43OYWKihy399kz3bzenGd50LjzZ2OwIEjnkrSz92OeoO3TnfHV-wGe-K0PEwxfvWiRa9SjV7mkNKNTQaC_qWhUGZZjjKZkl6_IP8vgKX2fh4hqusN1gWWRtdjEW_ZLN6RDjuUgObTgl91V7PoeZLXc88w-KK6TBEMq7f9emKly_7mQ)

- The Order mengarah ke Router The Minister melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/znGw1nclxdOUd0F7r3BaB7XMlNDaFg1PRrc4WTLAj4pMGeAog7Slb5H705JoIdPKFL7gmXl_hE0l87SuKVfk9gJeglC_VM3lozkiJzeiQNfJSXedOzO3xEK_8iZXnWm18t2XmZYQZHsQVQTXS0XovGR27UVw35lgkbmxf9nFg5yB2C3s2wUayCFkCc3lYQ)

  
  
  


4. Ashaf (Sebagai Client)

- Ashaf mengarah ke Router The Order melalui Fa 1/1 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/8GdkEAiPJpMKc3xM-FT3i4Sgo3YQv4yOCty5K4CDWyPFVQht3Om7lD8wgBzfmu9Y8pKR518R2X1xPkF0xia58_VqpylxjFGKB-C3GDR817_Gl52msHAtEwOgWZdwpbpBi5PI37grlfIc7YjWA9dbejucZwfKqvFpe4aKF_R7MmBniFn0G7CWtOA6_-DArw)

5. The Minister (Sebagai Router)

- The Minister mengarah ke Router The Order melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/PpmOfNd2Uus4Ktua_5PA8z6gQ8FdSgGRZHGnH3z3_yiBUKk0io-m6NdLbs6gGtyGqagStlpPknpTkYRv2Sdee_e4uDSPB-Ycjr2clEeQ0TaTAdXVzJHgb8zksSwoNBsnV3I7UDEnyo-XYAKMx_bBZWhh_VmaTfV_gtSjH3HieIvd4emmL44Zz-J6nVql2g)

  
  
  
  
  


- The Minister mengarah ke Client Guideau  melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/HS1gGu3x4RhNzt0ZXggVvITJqFRc_FrMbQCNJ4rfijw4MX3VMLlz19zSnOPaLOWo_GCYBOecrEKBqq6qlknKVvA7A6yPhks0Ajm66xGX3JYPNNnVNccdWsnYRcQJdC5DHPFKdDCjlpyIyu5lHnoIqKP5UnlqTtQTsTiyxfx6yTDdB82ofmbaeTB62w-egQ)

- The Minister mengarah ke Router The Dauntless melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/6YXQ2Q4bu1QcTvCI38_-NmwmaH5oROc3vU3UEjyiKN0ZfXyywKganPr4rnpGoamFqH-lU4b-eL0RRa3pgSHg0HOksg6fCtlyU3OHyqmHp7geV71O5jkySTiky0SRNTBTzBc55EOKJuvhKVXV7ZssT06dqBnC2uT-k5lnzUHUPvQZtfZzzjvLPUlaEG6ejg)

  
  


6. Guideau (Sebagai Client)

- Guideau mengarah ke Router The Minister melalui Fa 0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/eMqMrMd8H2yxddc88XtwboDzER9QfbaU3P7XaClU05JMREF5bQ-iK1K1twhrrb6GWGa9n8VcsOrhx6JNjPSK6lC2Ogja7G0YVTTYwjrHMAcfzUGvk8IRScHnZeF5OkjGQEpOfBhYHBilgJ3ETPlbZWEIGCZqgFPLyhBjXeuAvk2EwwToPGcirYdtbCQPxA)

7. The Dauntless (Sebagai Router)

- The Dauntless mengarah ke Router The Minister melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/Xfi7BsTgPaKrNtG0CNuDvM3SnFletBdPRLgz87DyzJYNhTAGzDLvDYrChLGqXOzG7vheklkKKODvWCvK7-xx0fhW9QUA8n7TcYOQ-MeZJ8TFX63aA5GjnkDppVvjR901SqqW-AWBTVzImuFAmg3JA4lC8Zsd0dbYh0m4_cP3rpJV2N-1wtUQFdncpLJUjw)

  
  
  


- The Dauntless mengarah ke Switch yang meneruskan ke Client Phanora dan Client Johan melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/BSyN9RQlMm63zitlV3777S4JPSkhRleUs6ZJwgyIjwaonapQKSFULZXH7FKO7Y9G_kWRF-L_ebeWSMIQhO2PegGS5T9Gp2-0Oly5P0XqSaR82txAgMqwx9QbRLEayJBThB5ZxKxJ40VvL_veU0zGr60ubr1AYa4pnV33UV2FyrksoLjRtTZL1sAF6EF4_w)

8. Phanora (Sebagai Client)

- Phanora mengarah ke Router The Dauntless melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/SMFv1-bbUjiM3Y03HmIe274TNZp6Zdr6-aeNUFHoni6gH-fjcjmZnoThA3ByCdEzZmB5ECiqYrZFfNXQikFtD8wA4D2szQQ4BzZw4mzQd6a_oa21zdngz5rtAdIrR3GqegfLI2uhd55cCpHLO7uHUuoWeiIypUl4v5lURfLxqi5PvK_aGBgRx3BuPizHAA)

  
  
  
  
  


9. Johan (Sebagai Client)

- Johan mengarah ke Router The Dauntless melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh3.googleusercontent.com/14dqEMdeolvlQMhu2hzqeIe6hpONDL_vZCxBdBsg_3Eo-n1OAHh28epnXx53hgLacP9YFSdvhF6tskPjX2Bt934ADVT9llREiE-4UvGrj3zwJv4L5wFvx-5L6KdoiA40lO_fHGKawqFcmyeVCKroDsEPnxE52-OvTpCP0gwSo5q1GkgHsnNr2oJt27-cJw)

10. The Magical (Sebagai Router)

- The Magical mengarah ke Router The Resonance melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/j9vqnh_RcxmmSyqwMBjZTHHEaSj5UcRSzAEZyMp5evRiH69dJLy0CSxHh7SkiAJ8dFn9ma7y9RLXQhKdOZTXByvRN0ci-5nxGAB5S2S8tu2w425WzSPE8750zZREaC45uLZM_w3lyd_63Thk5tl_JkkIVKBw83MqfzUk55FotQTrgTYtKrZxrqcaFXcEgg)

  
  
  
  
  


- The Magical mengarah ke Switch yang meneruskan ke Client Haines dan Client Corvekt melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/kBkHM0kbb0CcIvSYcF39pH5rVpABfxc351TTkLNlc9gt6j2I_khthTluRGEPJBdJZBaJ9BE1HRykD3WFD9J6KS6WFbrLU5Tu-RofJmI31GqxZjPHdJ1UMIqnpgca4QQG2ZvTihmvDmKvr_j7AH6cph4pewVJR_DwmAFwUQ3FLa_U9JcG7uV2AZ567d_kig)

11. Haines (Sebagai Client)

- Haines mengarah ke Router The Magical melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/ex_bwxCaYEJev-zOTkuvUguMbmrdZREDkerVbZOnm4m3I7t8ujmK6sprOyPIw5uBu8ouca-whBnZ_JRqSVjI73ombDJOTTeN6IuR6J9QlfFDKCruj-iG-h8iK9eNc9aG6Cktq07p71zc0at3F_4YdvWLsy29QmToQOhkbZtUlEQm1mEuI2lv8YSQ6SljtQ)

  
  
  
  
  
  
  


12. Corvekt (Sebagai Client)\\

- Corvekt mengarah ke Router The Magical melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/Kw73BU69F_whEomTcgpY0Oxka38InIwtKunEGfd9FN95XBnUYx6IZRECnLBM5-YYhIfKxpPGChUR8k7ZsMqTuES0k46euJrEuqQAtArO4eb5iHSSL8SS1CrzmHvxxOu6VbJM5C8i6XfuIuuSY1Oglftwj4ObG6T3bRWCQgsxWRbq1fdG9qmqlRUW11nVng)

13. The Instrument (Sebagai Router)

- The Instrument mengarah ke Router The Resonance melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/x-slyAAW6xqsA0bxMcZOmqkUrcIc3G1AJd0V5CFwVoDceiH_8y3FA_-28XUALw8Rz1E5HzaLlu0341EoG4EiMSIr-shIHO3Aykc6NnFh1rUDjQgUbK7PxJGR6qzJMWyoJ4U9OHDNIYYVEyv6hs3Z43sktn4Xo8QXLzxDU42CPirSk17cmYmoVTGQ5-fs2A)

  
  
  
  


- The Instrument mengarah ke Client Matt Cugat melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/l7TodUu0neJ3-FqCAiBJ72FRPhxNshYABqJd7l5y8HpUfkejua2NsFrYRQscIlJRU9_4LlBMY1DNn_b86QMvNHY4YH1B0RSMY8QWhVsZljgSQmdxPkXnotL2Me-XC-qASJqq8GqVfp0H3NYK0h4oZ5sxkNQIv5Gs0TewYS4pxU566Ss8i3M0mAqLcrp_YQ)

- The Instrument mengarah ke Router The Profound melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/JLddAbHX1U3zsuIDkx41NIH67bksbDBWiJSqHuT-JBaXxWlHf-QhFFvahlN0ZO3p1JKNH_exRs4VpKtkex3xhaz5u2j88eFaazcrZTPrpbHV_u9YeJf-0qqSPX0riI8TapZR75Pf1e-DlLCqpndSE1EixrHxpbUeUz8nT5jxXUMoc9VSraAzzcIc37WrOA)

  


- The Instrument mengarah ke Router The Firefist melalui Eth 1/1 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/C6zSsbhzk90d2uj6BWVRiox5DjNdSBC0nOx0G54ZKoVFeEgNVILITGFpJC4tNKxEv4iDIbS4XRalcTgnkGKnuUZbkCzqX95FH2rZtvbvJTpapbk41CTKh9U7y7uhW1zPhtDnIGx_s2sLl1NIxdh7VUGUH4jPezuUDdDxt8PA3-FYZro9YBnTrRWa4YIqSA)

14. Matt Cugat (Sebagai Client)

- Matt Cugat mengarah ke Router The Instrument melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/9EGoAnKd6_EUalDjJA35AxWRYxOKIjrIQIyYLcOHf2xFlHKhox7NCwlXAAED3dHTrKWWGHGAoRHu8U4YRlctvTocERgrvAr8-M7lQVwMGp0DqaNSVE_FUfKBOjYeqMN0tEnnJjO9ztYQ9VNewtZ8qYEfVzvMW_hsAw0m_NVBZQ0f3CK1BGiu9fzWDJo67A)

  
  
  
  
  
  


15. The Profound (Sebagai Router)

- The Profound mengarah ke Router The Instrument melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh3.googleusercontent.com/7eK3PXdSlCQrH9-ZoaM2P04hvDmiom-FI2M1Q18v2FrbKKBRljNMlGFEtu0kzNmeYr0WfDm3GWjXxTX3cJDB8AKqS0R0icfBwQQ90Il8Sh2LrXfyLTOgKzY-OIs_Ma4-MhYYRG84oRLIB_eO1YgN9fieF7dwYctVMLI9nlA9Sf6HVLayYr73t0HTtKHmMg)

- The Profound mengarah ke Client Spendrow melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh3.googleusercontent.com/wRgL4mPJaiCRWf7PnVpmWxanV6HPbV_aa6G8Nr7TF9HHaWwfXXCJbxKGTC0IpxTj__N299Qwkfnbp2OhyULpC1CxeTCjPQJSbiU40uIS7JO73WXOl3f8_6bPIj1krXxZAiht1FeNm0k8DMbehVTs9qlrjgBatglxImAyahAMnhMTyzpdUHBrPBpbJk9pcg)

  


- The Profound mengarah ke Client Helga melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/UGAHsq3h-AvcuzT2R6EpMvs4KbL4pQrt8v1UU4QDHqwe-5d6fRq5I8XnFrB0QgmwqOuFVlKe-Vl_LaDuJJfEV90_qfKM4uuOqLpxKvtBBsFbWBVg4zipBxxOzHBFLv9gm4jDUtzE-NaiuyRAhUxGpiNPjTDYUucg4H7qXBJXZsvgKxKLQfK_iZO4g51fXQ)

16. Spendrow (Sebagai Client)

- Spendrow mengarah ke Router The Profound melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/ilVr0O8pNDDNwot2WOhTAipBg-JEH5WgySPRxMyxGQlhSlmwg6GaICSS_xUQQlB6ffa1VZ1FJIR1GmLRMd7AjqWP60qu673LZp3ymfghV-f8tDiOP5g4B7bDNJb69weo-TXiO1fzMdhbzTvF15akU9TNmqzb1H1YMy5OMbvOmOdLBBJPoKkhgSdCvR2xbA)

  
  
  
  
  
  
  
  
  
  
  


17. Helga (Sebagai Client)

- Helga mengarah ke Router The Profound melalui Fa0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/-f5hfBxcSKtqAUDnyauiGspZ7REp-_yOOnoorhYU6H0FirKrkvApbrVW_WZtdXKjfXbJMEuPLLl70sT__Zbwp8wM3s5vk7k26n1PcWX-iihMpmorB-f0-s4DcrxyfaCURiV4dyVZqkOqJ1Ozw6WQ5xwBFUvJVcCWzob2iyk5SNBowaF1j4q2yDMPVdD05w)

18. The Firefist (Sebagai Router)

- The Firefist mengarah ke Router The Instrument melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/5SpqkxyXmGXr_nhb9eJa15Q3szGAJ6wjnwremNXjYNXyoEft2a_55o3HhV7FXk3FyOADRR4CSXTZ2YLuAmYUgzGFKz0x6KiYHV6Ol6BiXfUZXD4x6hoxSGN-eo_wCgvTlAufFpUtabMHmqCsFXpbS8Kc8hat4NX1BYLNJvJBZUybEnJndOgQF8mNdBaqEA)

  
  
  


- The Firefist mengarah ke Switch yang meneruskan ke Client Keith dan Router The Queen melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/fGCHMMTnmjmHrX5P0nDgb8ieDS8wrF3hpXn0JuuX3EYprVgE48mLedIv8kmh1UPRf9q0NPwWuccQ8gQ2tXMUi-r9gQ5VVvctREAavL6630CettuY_XIqDvNe3Z-d0BYMAQ1csFqyJ1_FNRundMjokebMyC29E3Hfk4FDP-r7utGzyGeLON-qWXoB6dgifw)

- The Firefist mengarah ke Client Oakleave melalui Eth 1/0 dengan konfigurasi seperti berikut

![](https://lh5.googleusercontent.com/CQYlg6yU3fiaUmJSLQRVEZrHjUqKBEuzidlZ1axQziMh0F13kTw6iNdrAZgi221VgnLDFX_p2JYrv8KLxh4EGIqkQzqj64kBFvLqeAkGe_QMuuPpZ-nAfKdAuWVcD5l4mNsWW9JyBIgYg2evaF44OKtMWfnNTquacT9E3L_9pb9_GyRxM7d2BdFeQCd9gA)

  


19. Oakleave (Sebagai Client)

- Oakleave mengarah ke Router The Firefist melalui Fa 0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/R_znd1gkc2J81bagRDDiZU27yxqVQ-osZVv76lVhM6tn1HmQpaPys_ALD9j6Bmhw1F3P8pBQ11FOxmo99czITSCUWvnjCuvTLGceTlOMd8SWdliXjaph4Cazw1jbilF1QPH2LXFjhA0c65xsylDqrSg7c-Fc5OVRHdtIBTGeJAjg22K7Fej1rPAuRWWIgQ)

20. Keith (Sebagai Client)

- Keith mengarah ke Switch yang meneruskan ke The Firefist dan Router The Queen melalui Fa 0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/a47TCnJ1A0ZqyBEmDHP6mKNk8KQFVRuIQBzupQjJSM35w50KtRjBccdKJJIlqblGNIlMhvOzMGZ12fzk0bs0YVWjPrBj4cnR91OCZOeLofOM8ZpUmc9KgyqfHV3ThkCe4coYn68LBZU2h6sBJwxZCWHuyRZdNQgfMuaPxDaA1DoylbFBw5KT08BYYFtTog)

  
  
  
  
  
  
  
  
  
  


21. The Queen (Sebagai Router)

- The Queen mengarah ke Switch yang meneruskan ke Router The Firefist dan Client Keith melalui Fa 0/0 dengan konfigurasi seperti berikut

![](https://lh6.googleusercontent.com/6Fx27H4Ypc5kL6IUar7hI-FRyZSx43Ka0RYFoN9DqSajbaf3cP9vnavDB0dGTNi7jV4rAM9sBsJmZ-VN5XK2vW4OQBTA6doAAwwPguDjDkIsPXLpEGh-ccbNzbKedVy0ikCgbKakIjxgjgZIEQOGQRCQ1Q7FF2MqNNDxmG7UDYUytDYJgXP4N66wCd5rXw)

- The Queen mengarah ke Switch yang meneruskan ke Server The Witch melalui Fa 0/1 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/u6TnjQs3MzNDYaqV8V9lUtLUJQTjMkm0hoqwilwmlBB7nEWsd_wXmwr6-BTdCXlgp0_gk9WlvMEwp7zIisWrAuorF7wbEz-aVHmECyFqF_axF7qPiMOsxGQZVYSI6WoPKmCzxPehO26ymaChuybBWO7lNVTLwiWyGBVjYVNVgmoK3V771hKpd9LTiz6ZtA)

  


22. The Witch (Sebagai Server)

- The Witch mengarah ke Router The Queen melalui Fa 0 dengan konfigurasi seperti berikut

![](https://lh4.googleusercontent.com/V6KRhrQpe1evhTvkOK6Sr_stQVJsKG84gjuak5bykqWFOl3zHm99sUUmd5FcsJB9l3IqV0_byXobmQcpPfgjup_0U11_dSFj03Kj-vLlX3Uc-hZeunWk-mxtt0R_BmyJ3pylTts7iBKz-Oueu9-x_dxyAHNcgeFHU5KSJupALQT0tM2Ii4UXRjPOadH5nA)

7. Uji Client

- Giudeau (1000 host)

![](https://lh6.googleusercontent.com/iziKFRt22GLBdUW7hVFAYeU0GN_kRnbWUN_7K8MnLf2xFkqobDwwgOwbBmVTIfZVzFzt9LlIkwh8hj4_INRMgFeCAWkif_k843SGoZOdI0VBTpqiJYYgNL_XpGxDsNDyv-MOWfmFf4TEplLILMG6eeRnGEh6YBEd-_uDU92uPdXj7-3JZe_OnV11mJIcAg)

- Ashaf (50 host)

![](https://lh5.googleusercontent.com/DKfqXr8uPMrEg_i4P2sxT-Xg2n6wxD6Te0hIDXpHLdT2-03lHYlzrUDm4Zjo5Pt__zlP9KaJAO1o4hWt2Zs1m1UsYxAakc-N1N63YoXR1SsjGiccocbszp6HSjmeTI6-UcvI9LcLaOVgz03v6XSmFRnR7ZJynVfvOm7WIUg1uPHYrxavWS05oC6WOA1JBA)

- The Beast

![](https://lh4.googleusercontent.com/VH3WhRW1sSKlMLTFQtaWEMzaUXsmh6gBegGlNUMRaAwwXa8sy-ibi6smGYMA8NlVsl43oWzKw8-FpFTdTDKYnEZcK9kgMBWnLp7hU7Crbru3qe5Qqt8HJCB99gjENWCkzsTWzkp2I8xpBA5Rud1iWX6SNkYLxUUAtBkT4yxa8MtSwbNcbjyZFGXrGiNYyg)

- Phanora (150 host)

![](https://lh5.googleusercontent.com/IS1jQoI4A0SF5Jhw65yqY7arWkQ0PmUvyc8iFcPPWMaY3yOe8kX9UPjuhkvy1XTo8uE4sPwiXZcda53ISgWj3E9pAT0AuRyE9FYIivBRJBSanRYgJvXLPjggJfSoOJR5Z48sgUZj3oFnqA4qKEQB9DSfD16KkJD613wMcD3JI7ZnySuGPcbXPvotX8_u1w)

- Johan (100 host)

![](https://lh4.googleusercontent.com/r0Cztc6DlQDw_HuW255JsyUNKp7nu6el1-HSb8cwsec8iznogz8j9egBrELBjkPPMnGC9xJehdoRyi16KoE0fdUL7srkcxL-t1YgDTZinGvdWkDDN2R_gT4s7I_4Ndro7ZgkByWp_yt2dFDoeQAuTyH3jMOymGJsoSBXvRjX53aOJnoxhWnIzRPirZlsxA)

- Haines (70 host)

![](https://lh3.googleusercontent.com/C6Ge5Gz8oY8Gqg0ySc3P1sv5bjUUtsG8FPpGaaLC7zZSIRSLaO36NzwS83HCUZZDnjUwiMCNlx2JaESD4WwSHyq6are22yLd8nq5xKWUoj7FD3h_DbYI4RuKckw0T1Sbh3_W0DCJeojxcX5Y0FXjGzbQ5c2BefnPNjNL9hhcXHcNEBUM7LPgwd2zgzl2sQ)

- Corvekt (200 host)

![](https://lh3.googleusercontent.com/ThJHLh6jpsxtEJKNQtg1aDwt-2enfx7477UuvHaa0A49m8aoxiGxhFY4u9DspwZRduvMigIkMOOw6cgynmW4JwgBY7Axfrbtk-yjl84ohfvsV-Xng_ZSvItFH5IU-WYcFcVxndpw8OIGXYSWUXdXow9B2CglF5CicyCBvR7IrXsoa3SU6tGmRVKrpPMa1A)

- Matt Cugat (120 host)

![](https://lh4.googleusercontent.com/TPa2_IE5TbnLarqOIMxtw5RprJbzog6X6-QG8hzfHGX4JghwIXg1O8rd1dLC5Hbk37toTcbGg-OsxnKiE0W6-92QK0BoUXYi1pnmyST6A8SXAwWQjE9cWCWlQaOSClT6oCXwuMsfhciulJMAynt0qKRpmlIYJS61PMRt6pMz2e9pJjuwWr_cGFDeqbap2Q)

- Spendrow (120 host)

![](https://lh6.googleusercontent.com/VKPCRAgnXa93LcjFRxgLERMFXUsQsubvl829uXj2hhiZ3nKulyXArOZC5YohrEw9oiKE_dpQGzD8fCYrVx-1GuZhN_NFDO-Xk8W5df4QUYAGrUDiiFKi7CNBmCAD96ybb9mSXHIcbhk7oXLYaoBGMbvRsM-jXu1xSU6nDtOHsPPjILKv7pLSit54Khs4IQ)

- Helga (70 Host)

![](https://lh6.googleusercontent.com/qAefkxi6fBejpAHpFpDGF1gqNXQr6in3WviBSJnyPPKfvmWIrhf1_AqztFYRhGyHPh1DXFqLcrw2Zpf-tprJ5EExcPzSZ0-uFnZ2Fa68SadFtjnmuv-BO677Ocn_kzNfNj5ortW37DpV1J6BdZXcx0lzmOB3G9ShGFZpgbRoSYxno29UmvmL2LK4MXMHHw)

- Keith (210 host)

![](https://lh4.googleusercontent.com/D03Uku1N15JKg4cNP3-tO2chwsk8q_dMnpZHxieiEJRn3DvP3RrwHhekzDXmpe4SjkslaOEBGRRVZIpi0-JF7_j_H5vaWzTzEBVAAfv55ji35M6_X-GEF2FtiKyJELj9vayqyOHwBu8ic2ylmU95hAGbKVRMUAJgY17K63daYJrN5WF2VHZqxyxT3NjExw)

- The Witch

![](https://lh4.googleusercontent.com/4Yzz3wR880kf9S4wYpsKBPA8LwnmxGkHFeeVb_d-MeuLZeeOoZHVRJB5dYwH8m7xsQwnCOpc3hvzh6R6LOq-s3R__wWdkChWJIbwgggCObIPtWSXQD72A-EyNG6ogWGcclVWoeRtsD7YA3uAQ1FRrECC5zSkm8ZlDQtik_toPtVLT56yiH8fbIo0kflbWw)

- Oakleave (500 Host)

![](https://lh4.googleusercontent.com/_xP6Ji9rVQ_ppisiLHlWq84PYfj84fStmqx3tCFhnNCjIVUoRK8uTK8HDSDJtdogv9D6YOXqt9lNRtN3hHtA-MLw1SFRpnbSwEteu13HJIDqXgs733WpOWxM26nzLAPs4pTNa-x-x97ZZ9o_7jqvXqwpOPOwuFY3a2SLHA-RhAsKzBvKbeA3_lAYLbWNBw)


- CIDR pada GNS3

1. Pembuatan Topologi

![](https://lh4.googleusercontent.com/6nr4MfG6kntSsNfuj9NzsqRnQQOGuHsT739jcCrp9Wg7OWM-X0XntdPJY5IAiEB2yy3nHCOQmT7pNroqih4AE-SqkAB6stQoxjAsYgYnf-sH-OdmXM0kZi8QvWPg8FKo4AbDsgnGuaGVFZU49RiwE681P454e_j9zflvy3eS9gitz7acXq8FYmE9_UZhag)

