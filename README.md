<h1> Arduino Ultrasonic Levitation <h1>
  
<h4> I opted to use six ultrasonic transducers instead of two after sketching a few concepts on paper because the main components of the levitation are the transducers, elements that transform the electrical input into acoustic waves. I intended to create a structure that traps expanded polystyrene (EPS) particles at its nodes. I had to figure out how to arrange the transducers in space to optimize trapping forces while minimizing parasitic reflections. <h4>
  
  Things you need:
  * ardiono uno
  * ultrasonic sensors (T) 
  * L296N 
  * 9V battery
  * jumper wires
  
  
  1. if you have the ultrasonic as a sensor, you have to desolder or disassemble the ultrasonic. The HC-SR04 has transmitter and receiver. The T transducer are better pick for use as an actual transmitter. 
  2. Find the polarity of the transmitter. The transducers have polarity, so it's critical that they're glued in the base with the same polarity. Do not trust the manufacturer's marks; they are completely unreliable. there are many wasy to find the polarity but I have used DMM to find by watching this [video](https://www.youtube.com/watch?v=0HaKv3aJQWA&t=7s). 
  3. Connect the wires and solder the transmitter. <br>
  
![photo](https://i1.wp.com/makezine.com/wp-content/uploads/2018/09/Schematic.jpg?resize=620%2C518&ssl=1)
  
  4. connect the arduino the the computer and open arduino IDE to upload the code
