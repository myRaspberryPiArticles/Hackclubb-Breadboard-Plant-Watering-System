# Hackclub _Breadboard_ Plant Watering System
For a Hackclub YSWS program, called Breadboard, I made and coded a machine based on Arduino that detects humidity of the air, temperature and soil moisture! It also has a LCD (16x2) and RGB LED module to visually show the data!

My project achieves detecting all of this through the DHT11 sensor, and a water moisture sensor, that both act as inputs to give back to the Arduino. You can see all this working [here](https://breadboard.hackclub.com/share/215).

I made it to help keep your plants in good conditions, remember to water them and also check if you need to change the watering schedules based on external conditions. My plants always end up going dry or wilting, so I figured I can make something simple yet reliable, to help keep them green and healthy!

## Pictures

<img width="324" height="348" alt="Screenshot 2026-07-18 at 17 49 40" src="https://github.com/user-attachments/assets/92ba5f92-3072-432d-8c9f-64e6d2aa498b" />
<img width="324" height="348" alt="Screenshot 2026-07-18 at 17 49 31" src="https://github.com/user-attachments/assets/7836a9c6-3eef-44aa-82ce-6c97eed02f05" />
<img width="861" height="486" alt="Screenshot 2026-07-18 at 17 49 14" src="https://github.com/user-attachments/assets/5b39e579-24b2-4c61-b2cc-ad31d115d6c6" />
<img width="861" height="486" alt="Screenshot 2026-07-18 at 17 49 10" src="https://github.com/user-attachments/assets/ebbb129c-eb6e-461f-b667-6306b521fb58" />
<img width="861" height="486" alt="Screenshot 2026-07-18 at 17 48 53" src="https://github.com/user-attachments/assets/c694c236-483b-483e-9eba-bd72e53b2212" />
<img width="890" height="439" alt="Screenshot 2026-07-18 at 17 36 31" src="https://github.com/user-attachments/assets/09cbca97-648c-4ad2-ad63-605bdddd1628" />


## What gave me the idea

After looking over the parts list that is available, I decided to use the Arduino kit for the amount of sensors it has. I wanted to make something that can be used in day to day life that helps solve a problem, and that it why I chose this idea. I spotted the soil moisture sensor, and I do have previous experience with these, so I decided to make something around this.

I didn't want my project to be a simple one that can be made quickly and effortlessly, as the result would not be as good. Therefore I added many more components and had an advanced code with LCD view switching, live updating, number formatting and specific outputs.

## How it all combines

I originallly had many files with code for each seperate component to test it's ability. I had:

- Temperature sensor - printed out values of temperature and humidity onto the LCD
- Water sensor - printed out soil moisture value onto the LCD as well as a description like 'Low water', 'High Water', etc
- RGB LED - tested the RGB LED and allowed the user to set it to any colour value they would like
- Buttons - tested buttons and printed out a message like 'Button 1 pressed!' onto the LCD

After each component reliably worked, I was able to combine them, by putting functions into the 'Buttons' code that changed views, or the RGB LED into the soil moisture/water sensor code to change based on the value.

## Parts list/BOM

| Header 1 (Left-Aligned) |
| :--- |
| Arduino |
| DHT11 |
| Water moisture sensor |
| RGB LED Module |
| 16x2 LCD |
| LCD I2C converter |
| x2 Push buttons |
| Large breadboard |
