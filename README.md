# Wireless Charger Project
## Determining whether the distance between your device and the wireless charging machine is reasonable in terms of efficiency or not using arduino, labview and hrsc04 ultrasonic distance sensor.


Wireless charging has been around since the late 19th century, when electricity pioneer Nikola Tesla demonstrated magnetic resonant coupling – the ability to transmit electricity through the air by creating a magnetic field between two circuits, a transmitter and a receiver.

After years of unhandiness, today, there are many wireless charging technologies in use, all aimed at cutting cables to everything from smartphones and laptops to kitchen appliances and cars. Even the furnitures are designed including this technology. 

The principle can be explained as; mainly, a magnetic loop antenna (copper coil) is used to create an oscillating magnetic field, which can create a current in one or more receiver antennas. If the appropriate capacitance is added so that the loops resonate at the same frequency, the amount of induced current in the receivers increases. This is resonant inductive charging or magnetic resonance; it enables power transmission at greater distances between transmitter and receiver and increases efficiency. Coil size also affects the distance of power transfer. The bigger the coil, or the more coils there are, the greater the distance a charge can travel. 



<img width="350" alt="foto2" src="https://user-images.githubusercontent.com/79105577/171506748-c2880be2-de97-4726-b97d-f5bdeea9fe6d.png">


The project was first designed on breadboard with HRsc04 ultrasonic sensor and arduino. Arduino code was written in arduino ıde program. 
### Arduino codes are given in WirelessChargerProjectArduinoCodes file in this repo. 
Lcd is used to display the results. The circuit is shown at the issue below.

breadboard: https://github.com/Beyzaelif/WirelessChargerProject/issues/1


For labview demonstration part for the project Linx and NI Visa was downloaded to read the data from the serial port of the computer. The circuit is shown at the  below issue. 

labview: https://github.com/Beyzaelif/WirelessChargerProject/issues/2

At this application a while loop is used. Data was taken from the serial port of the computer via Linx. For this to occur Arduino was identified to program first. There was a selection for the pin numbers in case the user wants to change the pins. From the linx library's digital => read section pulse width was used to get the data as micro seconds. In this library there is no peripheral to read the distance data directly so the datasheet for the HRSC04 sensor was used. As you can see from the link below there is a calculation to convert the data of microsec to distance. The principle is also shown in the below issue. 

datasheet: https://github.com/Beyzaelif/WirelessChargerProject/issues/3


After converting the data to distance a comparision block was used to determine if the distance is higher than 20 cm or not. According to the result the output was differing as "the distance is (more/less) than 20 cm". The other output was a led which turns on when you need to get your phone closer to the charging device in order to achieve at least %50 of effiency. After the designing stage of the front panel the program has run and the results are shown in the issue below.


application: https://github.com/Beyzaelif/WirelessChargerProject/issues/4

Thank you for checking my project up! 

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

 !!Quick reminder, photos can be also download to READme files as: ![Screenshot (20)](https://user-images.githubusercontent.com/79105577/171654504-e4bde42b-8d2d-4336-804f-2da87be645e8.png) but I wanted my project to look more orginized so I used issues.



















