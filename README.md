# Problem_Schematic_IP5306

I made the schematic to use the IP5306 only to charge lithium cells.

![image](https://github.com/user-attachments/assets/c38bcb2c-2f94-4363-8660-290b9789c6c2)


However, it turned out that every time I connected and disconnected the 5V charger from the chip, the IP5306 burned out.

After a lot of brainstorming, I contacted LCSC, where I bought the chips, and they told me that I couldn't leave the output floating. So I just added a capacitor to VOUT and the IC stabilized.

I also noticed that some chips keep blinking indefinitely, indicating charging. To solve this, just add a resistor between the BAT pin and the battery voltage.

![image](https://github.com/user-attachments/assets/a00e5738-7aec-4966-adbc-9474634acd65)

I recommend adding a battery protection layer, for example with DW01A and 8205A.
![image](https://github.com/user-attachments/assets/419b2de3-5b07-499f-b85d-ba096ac7126e)
