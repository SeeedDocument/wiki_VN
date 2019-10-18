---
name: Grove - Rotary Angle Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html
oldwikiname: Grove_-_Rotary_Angle_Sensor
prodimagename: Grove-Rotary_Angle_Sensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020017 1.jpg
surveyurl: https://www.research.net/r/Grove-Rotary_Angle_Sensor
sku: 101020017
tags: grove_analog, io_3v3, io_5v, plat_duino, plat_linkit, plat_bbg, plat_wio, plat_pi
---

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rotary.jpg)

The rotary angle sensor produces analog output between 0 and Vcc (5V DC with Seeeduino) on its D1 connector. The D2 connector is not used. The angular range is 300 degrees with a linear change in value. The resistance value is 10k ohms, perfect for Arduino use. This may also be known as a “potentiometer ”.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

Có một sản phẩm khác, Grove - Cảm biến góc quay (P). Không có nghĩa là gì? Đây là phiên bản dành cho bảng điều khiển gắn trên máy tính bảng. Đây là phiên bản chị em của Grove - Cảm biến góc quay. Chúng giống hệt nhau ngoại trừ bộ kết nối Grove được di chuyển ra phía sau để bạn có thể dễ dàng sử dụng nó như một thiết bị giao diện người gọn gàng và không có dây.

<table>
    <tr>
        <td>
            <img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/Grove-Rotary_Angle_Sensor-P-.jpg">
        </td>
        <td>
            <img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/GroveRotaryP_02.jpg">
        </td>
    </tr>
</table>

<p style=":center"><a href="http://www.seeedstudio.com/depot/grove-rotary-angle-sensorp-p-1242.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm                   | Thay đổi                              | Ngày phát hành |
|-----------------------------------|--------------------------------------|---------------|
|Grove-Rotary Angle Sensor(P) V1.1  | Ban đầu                              | 01/2013    |   
|Grove-Rotary Angle Sensor V1.2     | Ban đầu                              | 05/2014    |    


## Đặc điểm

-   Giao diện Grove
-   Dễ sử dụng
-   Module cơ bản Grove 

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật


<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Item
</th>
<th scope="col">
Min
</th>
<th scope="col">
Điển hình
</th>
<th scope="col">
Max
</th>
<th scope="col">
Đơn vị
</th>
</tr>
<tr align="center">
<th scope="row">
Điện áp
</th>
<td>
4.75
</td>
<td>
5.0
</td>
<td>
5.25
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Góc quay
</th>
<td>
0
</td>
<td>
~
</td>
<td>
300
</td>
<td>
°
</td>
</tr>
<tr align="center">
<th scope="row">
Kích thước
</th>
<td colspan="3">
19x19x30.1
</td>
<td>
mm
</td>
</tr>
</table>

## Nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


### Đối với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-Rotary Angle Sensor |Grove-LED|
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rorary_s.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/grove_led.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html)|[Get One Now](https://www.seeedstudio.com/Grove-LED-p-767.html)|

- **Step 2.** Kết nối Grove-Rotary Angle Sensor tới **A0** của Grove-Base Shield.
- **Step 3.** Kết nối Grove-LED tới **D3** của Grove-Base Shield. 
- **Step 4.** Cắm Grove - Base Shield vào Seeeduino.
- **Step 5.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/seeeduino_rotary.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Rotary Angle Sensor và  Grove-Led tới Seeeduino như dưới đây. Grove-Led phải được kết nối tới cổng PWM. Đối với Seeeduino, chúng là D3,5,6,9,10,11.

| Seeeduino | Grove-Rotary Angle Sensor | Seeeduino | Grove-LED |
|-----------|---------------------------|-----------|-----------|
| 5V        | Đỏ                       | 5V        | Đỏ       |
| GND       | Đen                     | GND       | Đen     |
| NC        | Trắng                     | NC        | Trắng     |
| A0        | Vàng                    | D3        | Vàng    |

**Phần mềm**

- **Bước 1.** Vui lòng sao chép mã dưới đây vào Arduino IDE và tải lên arduino. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).


```c++
/*macro definitions of Rotary angle sensor and LED pin*/

#define ROTARY_ANGLE_SENSOR A0
#define LED 3  //the Grove - LED is connected to PWM pin D3 of Arduino
#define ADC_REF 5 //reference voltage of ADC is 5v.If the Vcc switch on the seeeduino
                    //board switches to 3V3, the ADC_REF should be 3.3
#define GROVE_VCC 5 //VCC of the grove interface is normally 5v
#define FULL_ANGLE 300 //full value of the rotary angle is 300 degrees

void setup()
{
    Serial.begin(9600);
    pinMode(ROTARY_ANGLE_SENSOR, INPUT);
    pinMode(LED,OUTPUT);   
}

void loop()
{   
    float voltage;
    int sensor_value = analogRead(ROTARY_ANGLE_SENSOR);
    voltage = (float)sensor_value*ADC_REF/1023;
    float degrees = (voltage*FULL_ANGLE)/GROVE_VCC;
    Serial.println("The angle between the mark and the starting position:");
    Serial.println(degrees);

    int brightness;
    brightness = map(degrees, 0, FULL_ANGLE, 0, 255);
    analogWrite(LED,brightness);
    delay(500);
}

```

- **Bước 2.** Điều chỉnh Grove-Rotary Angle Sensor và chúng ta sẽ thấy Grove-LED thay đổi độ sáng.

### Với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Rotary Angle Sensor tới cổng A0, và kết nối Grove - Red LED tới cổng D3 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/cc_Rotary_Angle_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, độ sáng của đèn LED sẽ thay đổi tùy theo góc của cảm biến và giá trị góc được hiển thị trong Serial Monitor.

### Với Raspberry Pi (với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Rotary Angle Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rorary_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor--p-1242.html)|


- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối cảm biến quay với cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/Rotary_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng tương tự nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Step 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_rotary_angle_sensor.py 0

```

Dưới đây là mã  grove_rotary_angle_sensor.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveRotaryAngleSensor(ADC):
    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()
    
    @property
    def value(self):
        return self.adc.read(self.channel)


Grove = GroveRotaryAngleSensor


def main():
    if len(sys.argv) < 2:
        print('Usage: {} adc_channel'.format(sys.argv[0]))
        sys.exit(1)

    sensor = GroveRotaryAngleSensor(int(sys.argv[1]))

    while True:
        print('Rotary Value: {}'.format(sensor.value))
        time.sleep(.2)


if __name__ == '__main__':
    main()

```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_rotary_angle_sensor.py 0
Rotary Value: 932
Rotary Value: 931
Rotary Value: 931
Rotary Value: 931
Rotary Value: 933
Rotary Value: 931
Rotary Value: 742
Rotary Value: 666
Rotary Value: 666
Rotary Value: 549
Rotary Value: 520
Rotary Value: 499
Rotary Value: 430
Rotary Value: 430
Rotary Value: 321
Rotary Value: 286
Rotary Value: 205
Rotary Value: 127
Rotary Value: 88
Rotary Value: 0
Rotary Value: 0
Rotary Value: 0
Rotary Value: 0
Rotary Value: 0
Rotary Value: 0
Rotary Value: 0
^CTraceback (most recent call last):
  File "grove_rotary_angle_sensor.py", line 66, in <module>
    main()
  File "grove_rotary_angle_sensor.py", line 62, in main
    time.sleep(.2)
KeyboardInterrupt


```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

!!!Để ý
         Bạn có thể nhận thấy rằng đối với cổng analog, số pin màn hình có dạng như **A0, A1**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm mô-đun vào đúng cổng, nếu không có thể có xung đột pin.



### Đối với Raspberry Pi (với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus |  Grove-Rotary Angle Sensor |Grove-LED|
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rorary_s.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/grove_led.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html)|[Get One Now](https://www.seeedstudio.com/Grove-LED-p-767.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Rotary Angle Sensor tới **A0** của GrovePi_Plus.
- **Bước 4.** Kết nối Grove-LED tới **D5** của GrovePi_Plus.
- **Bước 5.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rpi_rotary.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Bước 3.** Thực hiện các lệnh dưới đây để theo dõi độ ồn.


```python
cd ~/GrovePi/Software/Python
python grove_rotary_angle_sensor.py
```

Đây là code grove_rotary_angle_sensor.py.

```python
import time
import grovepi

# Connect the Grove Rotary Angle Sensor to analog port A0
# SIG,NC,VCC,GND
potentiometer = 0

# Connect the LED to digital port D5
# SIG,NC,VCC,GND
led = 5

grovepi.pinMode(potentiometer,"INPUT")
grovepi.pinMode(led,"OUTPUT")
time.sleep(1)

# Reference voltage of ADC is 5v
adc_ref = 5

# Vcc of the grove interface is normally 5v
grove_vcc = 5

# Full value of the rotary angle is 300 degrees, as per it's specs (0 to 300)
full_angle = 300

while True:
    try:
        # Read sensor value from potentiometer
        sensor_value = grovepi.analogRead(potentiometer)

        # Calculate voltage
        voltage = round((float)(sensor_value) * adc_ref / 1023, 2)

        # Calculate rotation in degrees (0 to 300)
        degrees = round((voltage * full_angle) / grove_vcc, 2)

        # Calculate LED brightess (0 to 255) from degrees (0 to 300)
        brightness = int(degrees / full_angle * 255)

        # Give PWM output to LED
        grovepi.analogWrite(led,brightness)

        print("sensor_value = %d voltage = %.2f degrees = %.1f brightness = %d" %(sensor_value, voltage, degrees, brightness))
    except KeyboardInterrupt:
        grovepi.analogWrite(led,0)
        break
    except IOError:
        print ("Error")

```

- **Step 4.** Điều chỉnh Grove-Rotary Angle Sensor và chúng ta sẽ thấy Grove-LED thay đổi độ sáng.



### Với TI LaunchPad

**Đọc chiết áp (Cảm biến góc quay)**

Ví dụ này cho thấy cách đọc đầu ra tương tự đến từ module chiết áp Grove. Chúng tôi sẽ kết hợp một vài module Grove trong ví dụ này! Bằng cách xoay núm điều chỉnh chiết áp, chúng tôi sẽ hiển thị giá trị đọc tương tự trên màn hình kỹ thuật số Grove 4.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/Angle_sensor.jpg)

```
/*
    Rotary Angle Sensor
    Demonstrates analog input by reading an analog sensor on J16 of the Grove Base BoosterPack. The speed of the red LED on the LaunchPad will change depending on the position of the potentiometer knob. This example will also display the analog reading value on the Grove 4-digital display.

    The circuit:
    * Potentiometer attached to pin 24 (J6 on Grove Base BoosterPack)
    * center pin of the potentiometer to the analog pin
    * one side pin (either one) to ground
    * the other side pin to VCC (3.3V)

    * Note: Because of unstable of the voltage, the value of the rotary angle sensor
            varies slightly from run to run even you don't touch it.  

    Created by Oliver Wang

    This example code is in the public domain.

    http://www.seeedstudio.com/wiki/GROVE_-_Starter_Kit_v1.1b#Grove_-_Rotary_Angle_Sensor
    */

#include "TM1637.h"

/* Macro Define */
#define CLK               39                  /* 4-digital display clock pin */
#define DIO               38                /* 4-digital display data pin */
#define ROTARY_ANGLE_P    24               /* pin of rotary angle sensor */

/* Global Variables */
TM1637 tm1637(CLK, DIO);                  /* 4-digital display object */
int analog_value = 0;                     /* variable to store the value coming from rotary angle sensor */

int8_t bits[4] = {0};                     /* array to store the single bits of the value */

/* the setup() method runs once, when the sketch starts */
void setup() {

    /* Initialize 4-digital display */
    tm1637.init();
    tm1637.set(BRIGHT_TYPICAL);

}

/* the loop() method runs over and over again */
void loop() {   

    analog_value = analogRead(ROTARY_ANGLE_P);      /* read the value from the sensor */
    memset(bits, 0, 4);                             /* reset array when we use it */
    for(int i = 3; i >= 0; i--) {
        /* get single bits of the analog value */
        bits[i] = analog_value % 10;
        analog_value = analog_value / 10;  
        tm1637.display(i, bits[i]);                 /* display by 4-digital display */
    }
    delay(100);
}
```


## Nguồn

-  **[Eagle&PDF]** [Grove-Rotary Angle Sensor v1.2 Schematic File](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/res/Grove%20-%20Rotary%20Angle%20Sensor%20v1.2.zip)
-  **[Eagle&PDF]** [Grove - Rotary Angle Sensor(P) v1.1 Schematic File](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/res/Grove%20%20-%20Rotary%20Angle%20Sensor(P)%20v1.1.zip)
-  **[Library]** [Github repository for Rotary Angle Sensor](https://github.com/Seeed-Studio/Grove_Rotary_Angle_Sensor)
-  **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/res/Grove_Rotary_Angle_Sensor_CDC_File.zip)

## Dự án

**Sử dụng Grove-Rotary Angle Sensor(P) để điều khiển Grove LED**: Sử dụng Arduino / Genuino 101 để điều khiển độ sáng của đèn LED thông qua cảm biến góc quay Grove (P).

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/user50338573/using-grove-rotary-angle-sensor-p-to-control-grove-led-725e32/embed' width='350'></iframe>

**Module Rotary Angle Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/31RaX7JGv5s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/xx7hMoFQohY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>