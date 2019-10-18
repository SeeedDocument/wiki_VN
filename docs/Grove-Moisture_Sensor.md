---
name: Grove - Moisture Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html
oldwikiname: Grove - Moisture Sensor
prodimagename: Moisture_sensor_.jpg
surveyurl: https://www.research.net/r/grove-moisture-sensor
sku: 101020008
---

![](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/images/Moisture_sensor_.jpg)

Moisture Senor này có thể được sử dụng để phát hiện độ ẩm của đất hoặc phán đoán nếu có nước xung quanh cảm biến, hãy để cây trong vườn của bạn có thể tiếp cận sự giúp đỡ của con người khi khát. Cảm biến này rất dễ sử dụng, bạn chỉ cần chèn vào đất và đọc dữ liệu. Với cảm biến này, bạn có thể thực hiện một dự án nhỏ có thể cho phép nhà máy gửi tin nhắn cho bạn như "Bây giờ tôi đang khát, xin hãy cho tôi một ít nước."

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                   | Ngày phát hành |
|------------------------------|-------------------------------------------|---------------|
| Grove - Moisture Sensor V1.4 | Ban đầu                                   | 06/2014     |


## Đặc điểm

- Cảm biến độ ẩm đất dựa trên đo điện trở suất của đất
- Dễ sử dụng
- Kích thước  module grove 2.0 cm X 6.0 cm 

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Thông số kỹ thuật chính

|Item|Điều kiện|Min|Điển hình|Max|Đơn vị|
|---|---|---|---|---|---|
|Điện áp|-|3.3|-|5|V|
|Dòng điện|-|0|-|35|mA|
|Giá trị đầu ra|Cảm biến trong đất khô<br>Cảm biến trong đất ẩm <br>Cảm biến trong nước|0<br>300<br>700<br>|-|300<br>700<br>950|-|


## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Ý tưởng ứng dụng

- Làm vườn trồng cây
- Cảm biến độ ẩm
- Đo lường tính nhất quán

## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-Moisture Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/img/Moisture_sensor_S.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html)|

- **Bước 2.** Kết nối Grove-Moisture Sensor tới cổng A0 của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/img/Seeeduino_moisture.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Moisture Sensor tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Moisture Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| A0            | Vàng                  |

**Phần mềm**

- **Bước 1.** Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).

```c++
int sensorPin = A0;
int sensorValue = 0;

void setup() {
    Serial.begin(9600);
}
void loop() {
    // read the value from the sensor:
    sensorValue = analogRead(sensorPin);
    Serial.print("Moisture = " );
    Serial.println(sensorValue);
    delay(1000);
}
```

- **Bước 2.** Chúng ta sẽ thấy màn hình hiển thị độ ẩm trên terminal như dưới đây.

```
Moisture = 0
Moisture = 31
Moisture = 48
Moisture = 139
Moisture = 155
Moisture = 124
Moisture = 236
Moisture = 218
Moisture = 215
Moisture = 221
```

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Moisture Sensor tới cổng A0 của Base Shield.

**Step 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Step 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.
!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).


**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Moisture_Sensor/master/img/cc_Moisture_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy nhiệt độ và độ ẩm được hiển thị trên Màn hình Nối tiếp.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi | Grove - Moisture Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/img/Moisture_sensor_S.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html)

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**.  Kết nối Grove - Moisture Sensor tới cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/images/with_hat.jpg)


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

**Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_moisture_sensor.py 0
```


Dưới đây là mã  grove_moisture_sensor.py.

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-
#
# The MIT License (MIT)
#
# Grove Base Hat for the Raspberry Pi, used to connect grove sensors.
# Copyright (C) 2018  Seeed Technology Co.,Ltd.
'''
This is the code for
    - Grove - Moisture Sensor <https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html>`_

Examples:

    .. code-block:: python

        import time
        from grove.grove_moisture_sensor import GroveMoistureSensor

        # connect to alalog pin 2(slot A2)
        PIN = 2

        sensor = GroveMoistureSensor(PIN)

        print('Detecting moisture...')
        while True:
            m = sensor.moisture
            if 0 <= m and m < 300:
                result = 'Dry'
            elif 300 <= m and m < 600:
                result = 'Moist'
            else:
                result = 'Wet'
            print('Moisture value: {0}, {1}'.format(m, result))
            time.sleep(1)
'''
import math
import sys
import time
from grove.adc import ADC

__all__ = ["GroveMoistureSensor"]

class GroveMoistureSensor:
    '''
    Grove Moisture Sensor class

    Args:
        pin(int): number of analog pin/channel the sensor connected.
    '''
    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()

    @property
    def moisture(self):
        '''
        Get the moisture strength value/voltage

        Returns:
            (int): voltage, in mV
        '''
        value = self.adc.read_voltage(self.channel)
        return value

Grove = GroveMoistureSensor


def main():
    from grove.helper import SlotHelper
    sh = SlotHelper(SlotHelper.ADC)
    pin = sh.argv2pin()

    sensor = GroveMoistureSensor(pin)

    print('Detecting moisture...')
    while True:
        m = sensor.moisture
        if 0 <= m and m < 300:
            result = 'Dry'
        elif 300 <= m and m < 600:
            result = 'Moist'
        else:
            result = 'Wet'
        print('Moisture value: {0}, {1}'.format(m, result))
        time.sleep(1)

if __name__ == '__main__':
    main()
```


!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau:
```python

pi@raspberrypi:~/grove.py/grove $ python grove_moisture_sensor.py 0
Detecting moisture...
Moisture value: 0, Dry
Moisture value: 1, Dry
Moisture value: 25, Dry
Moisture value: 3, Dry
Moisture value: 0, Dry
Moisture value: 0, Dry
Moisture value: 0, Dry
Moisture value: 0, Dry
Moisture value: 0, Dry
Moisture value: 1, Dry
^CTraceback (most recent call last):
  File "grove_moisture_sensor.py", line 74, in <module>
    main()
  File "grove_moisture_sensor.py", line 71, in main
    time.sleep(1)
KeyboardInterrupt

```
Bạn có thể sử dụng cảm biến này để phát hiện chất lượng không khí. Nhấn ++ ctrl + c ++ để thoát.

!!!Để ý
         Bạn có thể nhận thấy rằng đối với cổng analog, số pin màn hình có dạng như **A0, A1**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm mô-đun vào đúng cổng, nếu không có thể có xung đột pin.


### Đối với Raspberry Pi (với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove-Moisture Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/img/Moisture_sensor_S.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Moisture Sensor tới cổng **A0** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/img/rpi_moisture.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 3.** Thực hiện các lệnh dưới đây để sử dụng Cảm biến độ ẩm Grove để đo độ ẩm.


```
cd ~/GrovePi/Software/Python
python grove_moisture_sensor.py
```

Đây là code grove_moisture_sensor.py.

```python
# 	Here are suggested sensor values:
# 		Min  Typ  Max  Condition
# 		0    0    0    sensor in open air
# 		0    20   300  sensor in dry soil
# 		300  580  700  sensor in humid soil
# 		700  940  950  sensor in water


import time
import grovepi

# Connect the Grove Moisture Sensor to analog port A0
# SIG,NC,VCC,GND
sensor = 0

while True:
    try:
        print(grovepi.analogRead(sensor))
        time.sleep(.5)

    except KeyboardInterrupt:
        break
    except IOError:
        print ("Error")
```

- **Step 4.** Chúng ta sẽ thấy màn hình hiển thị độ ẩm trên thiết bị đầu cuối như dưới đây.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_moisture_sensor.py
0
90
130
150
160
218
238
```

### Đối với TI LaunchPad

**Phần cứng**

Phác thảo sau đây cho thấy một ứng dụng đơn giản là cảm nhận độ ẩm trong đất. Với điều này, bạn có thể biết cây của mình có cần nước hay không bằng cách quan sát kết quả từ đầu ra của cảm biến

![](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/images/Moisture.jpg)

**Phần mềm**

```c
/*
  Moisture-Sensor
  The following sketch demonstrates a simple application of sensing
  the moisture of the soil. You can know whether a plant needs water
  or not by observing the results that the sensor outputs.
  The circuit:
    * Moisture-Sensor attached to pin 24 (J6 plug on Grove Base BoosterPack)
    * one side pin (either one) to ground
    * the other side pin to +VCC
    * LED anode (long leg) attached to RED_LED
    * LED cathode (short leg) attached to ground
  - NOTE:
    This example code is in the public domain.
    http://seeedstudio.com/wiki/Grove_-_Moisture_Sensor
*/
#include "TM1637.h"
/* Macro Define */
#define CLK 39              /* 4-digital display clock pin */
#define DIO 38              /* 4-digiral display data pin */
#define BLINK_LED RED_LED   /* blink led */
#define MOISTURE_PIN 24     /* pin of moisture sensor */
#define THRESHOLD_VALUE 300 /* threshold for watering the flowers */
#define ON HIGH             /* led on */
#define OFF LOW             /* led off */
#define _handle_led(x) digitalWrite(BLINK_LED, x) /* handle led */

/* Global Varibles */
TM1637 tm1637(CLK, DIO);    /* 4-digital display object */
int analog_value = 0;       /* varible to store the value coming from rotary angle
sensor */
int8_t bits[4] = {0};       /* array to store the single bits of the value */
/* the setup() method runs once, when the sketch starts */
void setup() {
/* Initialize 4-digital display */
    tm1637.init();
    tm1637.set(BRIGHT_TYPICAL);
/* declare the red_led pin as an OUTPUT */
    pinMode(BLINK_LED, OUTPUT);
}
/* the loop() method runs over and over again */
void loop() {
    analog_value = analogRead(MOISTURE_PIN); /* read the value from the sensor */
/* if the value is smaller than threshold, turn on led */
    if(analog_value < THRESHOLD_VALUE) {
        _handle_led(ON);
    } else {
        _handle_led(OFF);
    }
    memset(bits, 0, 4); /* reset array when we use it */
    for(int i = 3; i >= 0; i--) {
/* get single bits of the analog value */
        bits[i] = analog_value % 10;
        analog_value = analog_value / 10;
        tm1637.display(i, bits[i]); /* display by 4-digital display */
    }
    delay(200);
}
```

## FAQs

**Q1: Đầu ra có nghĩa là gì? điện áp hay đếm?**

A1: Đầu ra là giá trị điện áp. Khi sử dụng analogRead (), 5V sẽ được chia cho 1023. Vì vậy, giá trị đầu ra = Vout * 1023/5. Điện áp đầu ra càng cao thì độ ẩm càng cao.

## Nguồn

- [**Eagle&PDF**][Grove - Moisture Sensor v1.4 Schematic](https://github.com/SeeedDocument/Grove_Moisture_Sensor/raw/master/resources/Grove%20-%20Moisture%20Sensor%20v1.4.zip)
- [**Codecraft**][CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Moisture_Sensor/master/res/Grove_Moisture_Sensor_CDC_File.zip)


## Dự án

**Hệ thống giám sát nhà máy sử dụng AWS IoT**: Nếu bạn có kế hoạch cho một kỳ nghỉ, đây là một dự án tuyệt vời để theo dõi nhiệt độ và độ ẩm đất của Nhà máy của bạn bằng cách sử dụng dweet.io và AWS IoT.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/carmelito/plant-monitoring-system-using-aws-iot-6cb054/embed' width='350'></iframe>



## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>