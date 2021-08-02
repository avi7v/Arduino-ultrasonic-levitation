![image](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/6.jpeg)
<h1>Ultrasonic Levitation<h1>
  <h4>Asier Marzo and Bruce Drinkwater of Bristol developed a sonic tractor beam in 2015 that could lift, rotate, and move objects in numerous directions using ultrasound. That system created acoustic holograms that could trap and manipulate objects in mid-air using a grid of 64 off-the-shelf, small loudspeakers controlled by a programmable array of transducers. He says that medical imaging tools could be used to catch and move kidney stones, among other things. This was previously impossible due to the extremely short wavelengths used to obtain high-resolution photos. “Now that we can trap particles larger than half a wavelength,” Marzo explains, “you could use the same system that you use for imaging to trap particles.” <h4>

<h4> I opted to use six ultrasonic transducers instead of two after sketching a few concepts on paper because the main components of the levitation are the transducers, elements that transform the electrical input into acoustic waves. I intended to create a structure that traps expanded polystyrene (EPS) particles at its nodes. I had to figure out how to arrange the transducers in space to optimize trapping forces while minimizing parasitic reflections. The transducer that I bought operates at 40kHz.    <h4>

<h4> Arduino is an open-source electronics platform that uses simple hardware and software to make it easy to use. Arduino boards can take inputs - such as light from a sensor, a finger on a button, or a Twitter message - and convert them to outputs - such as turning on an LED, triggering a servo, or publishing anything online. By providing a set of instructions to the board's microcontroller, you may tell it what to do. <h4> 

<h4>The L293D IC is a common Motor Driver IC that allows a DC motor to rotate in any direction. This IC has 16 pins and is used to operate a set of two DC motors in any direction at any time. It means that we can control two DC motors with an L293D IC. This IC can also run small and quiet large motors. <h4>
  
  Things you need:
  * ardiono uno
  * ultrasonic sensors (T) 
  * L298 motor driver
  * 9V battery
  * jumper wires
  
  
  1. if you have the ultrasonic as a sensor, you have to desolder or disassemble the ultrasonic. The HC-SR04 has transmitter and receiver. The T transducer are better pick for use as an actual transmitter. 3D print the holder from [here](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/MicroLev-Bottom.stl).
  ![image](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/4.jpg)
  
  2. Find the polarity of the transmitter. The transducers have polarity, so it's critical that they're glued in the base with the same polarity. Do not trust the manufacturer's marks; they are completely unreliable. there are many wasy to find the polarity but I have used DMM to find by watching this [video](https://www.youtube.com/watch?v=0HaKv3aJQWA&t=7s). 
  3. Connect the wires and solder the transmitter. <br>
  
![photo](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/1.jpg)
![p](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/3.jpg)

  4. connect the arduino the the computer and open arduino IDE to upload the code. The coding is quite basic, consisting of only a few lines. We are making high or low (0 / 1) and generating an oscillating signal of 40Khz to Arduino A0 and A1 output pins using this small code with the help of a timer and interrupt routines. [download](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/Ultrasonic_levitation.ino)
  ![image](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/5.jpg)
  5. Re-upload and double-check all of the wiring. I used my phone voice recorder to listen for sound to see whether the ultrasonics were working. Instead of polystyrene, I used [Aerogel](http://www.buyaerogel.com/) to levitate it so that it could be illuminated by UV light.
  ![image](https://github.com/avi7v/Arduino-ultrasonic-levitation/blob/main/2.jpeg)
  
  
  

  
  
