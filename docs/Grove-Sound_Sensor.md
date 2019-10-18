---
name: Grove - Sound Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Sound-Sensor-p-752.html
oldwikiname: Grove_-_Sound_Sensor
prodimagename: page.jpg
surveyurl: https://www.surveymonkey.com/r/SoundSensor
sku: 101020023
tags: io_3v3, io_5v, plat_duino, plat_linkit, plat_bbg, plat_wio, plat_pi, plat_linkit
---

![](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/page_small_1.jpg)

Grove - Sound Sensor có thể phát hiện cường độ âm thanh của môi trường. Thành phần chính của mô-đun là một micrô đơn giản, dựa trên bộ khuếch đại LM386 và micrô điện tử. Đầu ra của mô-đun này là tương tự và có thể dễ dàng lấy mẫu và kiểm tra bởi Seeeduino.

<iframe width="800" height="450" src="https://www.youtube.com/embed/EhZ7uDvoALE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p style=":center"><a href="http://www.seeedstudio.com/Grove-Sound-Sensor-p-752.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>


## Đặc điểm

* Dễ dùng
* Cung cấp tín hiệu đầu ra tương tự
* Dễ dàng tích hợp với các module Logic ở phía đầu vào của mạch Grove

!!!Cảnh báo
     Cảm biến âm thanh này được sử dụng để phát hiện xem có âm thanh vòm hay không, vui lòng không sử dụng mô-đun để thu thập tín hiệu âm thanh. Ví dụ, bạn có thể sử dụng nó để làm đèn điều khiển âm thanh, nhưng không phải là một thiết bị ghi âm.

## Thông số kỹ thuật

|Item|Giá trị|
|-----|------|
|Diện áp hoạt động| 3.3/5 V |
|Dòng hoạt động(Vcc=5V)|4~5 mA|
|Điện áp Gain(V=6V, f=1kHz)|26 dB|
|Độ nhạy của micrô(1kHz)|52-48 dB|
|Trở kháng micro|2.2k Ohm|
|Tần số micrô|16-20 kHz|
|Micrô S / N Radio|54 dB|

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.




## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

|Seeeduino V4.2| Base Shield|Grove-Sound Sensor|
|--------------|------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/page_small_1.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Sound-Sensor-p-752.html)|

- **Bước 2.** Kết nối Grove-Sound Sensor tới **A0** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/1_connect.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Sound Sensor tới Seeeduino như dưới đây.

| Seeeduino     | Grove-Sound Sensor      |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| A1            | Trắng                   |
| A0            | Vàng                  |

**Phần mềm**

- **Bước 1.** Vui lòng sao chép mã dưới đây vào Arduino IDE và tải lên arduino. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải mã lên](http://wiki.seeedstudio.com/Upload_Code/).

```c
// test code for Grove - Sound Sensor
// loovee @ 2016-8-30

const int pinAdc = A0;

void setup()
{
    Serial.begin(115200);
    //Serial.println("Grove - Sound Sensor Test...");
}

void loop()
{
    long sum = 0;
    for(int i=0; i<32; i++)
    {
        sum += analogRead(pinAdc);
    }

    sum >>= 5;

    Serial.println(sum);
    delay(10);
}

```

- **Step 2.** Nhấn **Serial > Plotter** để có được đường cong thay đổi của cảm biến. Vui lòng tạo tiếng ồn để xem sự thay đổi của giá trị.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Sound_Sensor/master/images/sound_raw.png)

### Với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Sound Sensor tới A0 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Sound_Sensor/master/img/cc_Sound_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy giá trị của âm thanh hiển thị trên Serial Monitor.

### Với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Sound Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/page_small_1.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-Sound-Sensor-p-752.html)|



- **Step 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**. Kết nối Grove - Sound Sensor tới A0 của Base Hat.
- **Step 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/Sound_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng tương tự nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.

- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Step 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_sound_sensor.py 0

```

Dưới đây là mã  grove_sound_sensor.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveSoundSensor:

    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()

    @property
    def sound(self):
        value = self.adc.read(self.channel)
        return value

Grove = GroveSoundSensor


def main():
    if len(sys.argv) < 2:
        print('Usage: {} adc_channel'.format(sys.argv[0]))
        sys.exit(1)

    sensor = GroveSoundSensor(int(sys.argv[1]))

    print('Detecting sound...')
    while True:
        print('Sound value: {0}'.format(sensor.sound))
        time.sleep(.3)

if __name__ == '__main__':
    main()


```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_sound_sensor.py 0 
Detecting sound...
Sound value: 499
Sound value: 525
Sound value: 529
Sound value: 493
Sound value: 457
Sound value: 457
Sound value: 503
Sound value: 537
Sound value: 606
Sound value: 614
Sound value: 661
^CTraceback (most recent call last):
  File "grove_sound_sensor.py", line 67, in <module>
    main()
  File "grove_sound_sensor.py", line 64, in main
    time.sleep(.3)
KeyboardInterrupt

```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

!!!Để ý
         Bạn có thể nhận thấy rằng đối với cổng analog, số chân màn hình có dạng như **A1, A0**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm mô-đun vào đúng cổng, nếu không có thể có xung đột chân.



### Với Raspberry Pi (Với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus|Grove-Sound Sensor|Grove-Blue LED|
|--------------|-------------|-----------------|----------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Sound_Sensor/master/images/gs_1.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/groveblue%20led.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](http://www.seeedstudio.com/Grove-Sound-Sensor-p-752.html)|[Get One Now](https://www.seeedstudio.com/Grove---Blue-LED-p-1139.html)|

- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.


- **Bước 3.** Kết nối Grove-Sound Sensor tới cổng **A0** của GrovePi_Plus , và kết nối Grove-Blue LED tới **D5** của GrovePi_Plus

- **Bước 4.** CKết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/img/2_connect.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.

- **Bước 2.**  Thực hiện theo [Cập nhật Firmware](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/updating-firmware/) để cập nhật firmware mới nhất của GrovePi.

!!!Mẹo
    Trong wiki này, chúng tôi sử dụng đường dẫn **~/ GrovePi/** thay vì **/home/pi/Desktop/GrovePi**, bạn cần đảm bảo Bước 2 và Bước 3 sử dụng cùng một đường dẫn.

!!!Chú ý
    Chúng tôi đề nghị bạn cập nhật chương trình firmware hoặc đối với một số cảm biến bạn có thể gặp lỗi.

- **Bước 3.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Step 4.** Điều hướng đến thư mục của các bản demo:

```
cd yourpath/GrovePi/Software/Python/
```

Here is the grove_sound_sensor.py code.

```python

#!/usr/bin/env python
#
# GrovePi Example for using the Grove Sound Sensor and the Grove LED
#
# The GrovePi connects the Raspberry Pi and Grove sensors.  You can learn more about GrovePi here:  http://www.dexterindustries.com/GrovePi
#
# Modules:
#	 http://www.seeedstudio.com/wiki/Grove_-_Sound_Sensor
#	 http://www.seeedstudio.com/wiki/Grove_-_LED_Socket_Kit
#
# Have a question about this example?  Ask on the forums here:  http://forum.dexterindustries.com/c/grovepi
#
'''
## License
The MIT License (MIT)
GrovePi for the Raspberry Pi: an open source platform for connecting Grove Sensors to the Raspberry Pi.
Copyright (C) 2017  Dexter Industries
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
'''

import time
import grovepi

# Connect the Grove Sound Sensor to analog port A0
# SIG,NC,VCC,GND
sound_sensor = 0

# Connect the Grove LED to digital port D5
# SIG,NC,VCC,GND
led = 5

grovepi.pinMode(sound_sensor,"INPUT")
grovepi.pinMode(led,"OUTPUT")

# The threshold to turn the led on 400.00 * 5 / 1024 = 1.95v
threshold_value = 400

while True:
    try:
        # Read the sound level
        sensor_value = grovepi.analogRead(sound_sensor)

        # If loud, illuminate LED, otherwise dim
        if sensor_value > threshold_value:
            grovepi.digitalWrite(led,1)
        else:
            grovepi.digitalWrite(led,0)

        print("sensor_value = %d" %sensor_value)
        time.sleep(.5)

    except IOError:
        print ("Error")
```

- **Step 5.** Chạy demo.


```
sudo python grove_sound_sensor.py
```

## Nguồn

- [**Eagle**][Schematic and PCB in Eagle format](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/resources/Grove%20-%20Sound%20Sensor.zip)
- [**PDF**][Schematic in PDF format](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/res/Grove%20-%20Sound%20Sensor%20v1.6%20Schematic.pdf)
- [**PDF**][PCB in PDF format](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/res/Grove%20-%20Sound%20Sensor%20v1.6%20PCB.pdf)
- [**Datasheet**][LM386.PDF](https://github.com/SeeedDocument/Grove_Sound_Sensor/raw/master/res/LM386.pdf)
- [**Codecraft**][CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Sound_Sensor/master/res/Grove_Sound_Sensor_CDC_File.zip)

## Dự án

**Tạo cảm biến Wi-Fi IoT đa tác vụ**: Hướng dẫn này giới thiệu cách tạo cảm biến kết nối internet, đồng thời tận dụng các tính năng đa tác vụ độc đáo của Energia & TI LaunchPad.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/adrianf/create-a-multi-tasking-iot-wi-fi-sensor-9d7fdf/embed' width='350'></iframe>


**Máy đo âm thanh LED sử dụng Wio-Link và Node-Red**: Cảm biến âm thanh SeeedStudio Grove và dải đèn LED gắn vào Wio-Link được điều khiển bởi luồng Node-Red.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/potnik/led-sound-meter-using-wio-link-and-node-red-259e02/embed' width='350'></iframe>

**Sound sensor Grove module**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/N19VfMYyn60" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/NfFlz8KEFxw" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>