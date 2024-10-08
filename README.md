# UPDATE Multiwii-2.3-with-BMP280 (August 14th, 2024)
Multiwii brushed quadcopter with bmp280 module

<h1>ATTENTION: THIS PROJECT IS ONLY WORKS with LADYBIRD Board</h1>
<p>See in config.h to choose board LADYBIRD. All files are configured. You dont need to change anything., but about how to <a href="#activate">activate and deactivate baro</a>.</p>

<p>All wiring and schematic is based on: <a href="https://github.com/ArduJimmy/ArduJimmy-Brushed-QuadX-With-Flysky">Multiwii 2.3 Brushed QuadX</a></p>

<img src="https://github.com/ArduJimmy/Multiwii-2.3-with-BMP280/blob/main/BMP280.png" alt="Multiwii with bmp280"/>

<h3>BMP280 WIRING with MPU6050</h3>
<ul>
  <li>Use 3.3v Breakout Module or AMS1117 3.3v for MPU6050 and BMP280</li>\
  <li>VCC Output off 3.3v breakout to VCC MPU6050 and BMP280</li>
  <li>GND 3.3v breakout to GND MPU6050 and GND BMP280</li>
  <li>GND 3.3v breakout ALSO connect to GND Arduno board</li>
  <li>SCL mpu6050 and SCL bmp280 connected to A5 arduino board</li>
  <li>SDA mpu6050 and SDA bmp280 connected to A4 arduino board</li>  
</ul>

<p>Here's the wiring:</p>
<img src="https://github.com/ArduJimmy/Multiwii-2.3-with-BMP280/blob/main/schematic%20diagram%20bmp280.png"/>

<h3><b>UPDATE!</b> TESTED!</h3>
<p>This package (multiwii 2.3 with BMP280) has been already tested. Baro feature has worked successfully in multiwii 2.3</p>


<p>I will post the video for test flight using baro later here.</p>

<h3 id="activate">HOW TO</h3>
<p><b>How to activate barometer in your drone</b>: Change the value 0 to 1 in <b>def.h</b> file. Otherwise, it will show error in multiwiiConf-GUI.</p>
<ul>
  <li>ACTIVATE: #define BMP280_CONNECTED 1</li>
  <li>DEACTIVATE: #define BMP280_CONNECTED 0</li>  
</ul>

<p>See this illustration</p>
<img src="https://github.com/ArduJimmy/Multiwii-2.3-with-BMP280/blob/main/activate-deactivate%20bmp280%20in%20multiwii%202.3.PNG"/>

<p><b>in MultiwiiConf GUI</b>: Click on angle (MID and HIGH)</p>
<img src="https://github.com/ArduJimmy/Multiwii-2.3-with-BMP280/blob/main/multiwiiconf_GUI%20for%20bmp280.PNG"/>

<h3>CALIBRATE BMP280 (HOW TO TEACH your drone with its BARO feature)</h3>
<ul>
  <li>Arm your drone, go fly with it and then activate AUX1</li>
  <li>Keep your drone stable by checking th drone direction (tends to roll or to pitch). When it tends to roll, use your manual trim of your TX to fix it. Do it the same as pitch trim when you see your drone tends to left or right.</li>
  <li>When the drone stable enough, deactivate Aux1 in your flysky TX</li>
  <li>Land your drone then DISARM quickly</li>
  <li>Done</li>
</ul>

<p>DEMO: <a href="https://www.youtube.com/watch?v=OaMo1lwZqmA">Click Here"></a></p>
