# Haresh-U-Capstone-Project

DE 2025-2026 Capstone Project - R/C Plane

## **Introduction**

I pursued this project with intent to update the quality of current R/C airplanes for hobbyists, by including quality-of-life features such as altitude hold and auto-landing. I wanted to make an R/C plane that accomodated these features. Unfortionately, I wan't able to get all the way to a fully functioning airplane, but I was able to make good progress and will continue this project throughout this year.

  I go into more detail about the project in my [digital notebook](https://docs.google.com/document/u/1/d/1Xd8hyVqAFlKc2oIBXLoqVHdMWL5ACztB0SyBCPcDpvg/edit?tab=t.0).
  
## **Parts Used**

For the electrical circuit, the main powerhouse of the airplane would be the HolyBro Kakute H743 Wing. This flight controller is capable of using a software called [ArduPilot](https://ardupilot.org/) which takes care of most of the software. Ardupilot has many features that tie more towards the fully autonomous flight, but it can still be used for assisted R/C flight.

The other components consist of the usual things that r/c airplanes have like servos, a motor, and battery. However, for additional features such as the ones listed in the introduction, other components are needed like a GPS and airspeedometer to detect height, position and airspeed.

![Wiring_Diagram-2](https://github.com/user-attachments/assets/8858ce65-cbf9-4194-929f-40ed9af732df)

## **Testing Servos with a Raspberry Pi testbed**

<img width="430" height="310" alt="image" src="https://github.com/user-attachments/assets/555179d2-8d30-43dd-bda3-a42adacf6668" />

While I was waiting for parts to arrive, I wanted to test my 180 degree and 360 degree servos. To do so, I used a Raspberry Pi 5 and a PWM module (Adafruit PCA9865) and a 5V 3A power supply. This is how the system would interact with the servo:

<img width="342" height="194" alt="image" src="https://github.com/user-attachments/assets/2fe8ab6c-f62d-4fb7-adb5-e6b2ce193665" />

## **Code for testing servos with raspberry Pi**

I go more in depth in my digital notebook but to summarize, I installed certain libraries that allow for control of the servo throught the PWM module.

The main code uses loops to swap between 180 and 0 degrees, to test that all possible angles work for the servo. Additionally, the lower and higher limit of the pulse was set to 500 and 2500 because those are the limits for the specific SG90 servos that I am using.

REMEMBER TO ADD CODE

## **Future Plans**

I intend to use a ultrasonic sensor and controller to control the servos


