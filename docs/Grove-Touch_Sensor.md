---
name: Grove - Touch Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Touch-Sensor-p-747.html
oldwikiname: Grove_-_Touch_Sensor
prodimagename: Grove-Touch_Sensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020037 1.jpg
surveyurl: https://www.research.net/r/Grove-Touch_Sensor
sku: 101020037
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_linkit, plat_pi, plat_bbg
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Touch_Sensor/master/img/surface.jpg)

Grove - Touch Sensor cho phép bạn thay thế nhấn bằng cảm ứng. Nó có thể phát hiện sự thay đổi điện dung khi một ngón tay ở gần. Điều đó có nghĩa là bất kể ngón tay của bạn chạm trực tiếp vào miếng đệm hay chỉ ở gần miếng đệm, Grove - Touch Sensor sẽ cho đầu ra ở mức CAO.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Touch-Sensor-p-747.html)

## Các thông số kỹ thuật

- Điện áp hoạt động: 2.0 - 5.5V
- Dòng hoạt động(Vcc=3V):1.5 - 3.0μA
- Dòng hoạt động(VDD=3V):3.5 - 7.0μA
- Thời gian đáp ứng đầu ra: 60 - 220mS
- Chipset được sử dụng: TTP223-BA6

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


**Tính năng tùy chọn**

| AHLB                     | TOG         | LPMB       | MOTB         | SLRFTB          | RST       | Q           | OPDO            |
|--------------------------|-------------|------------|--------------|-----------------|-----------|-------------|-----------------|
| Đầu ra hoạt động Cao / Thấp | Chế độ Toggle | Chế độ Power| Max. On Time | Chiều dài lấy mẫu | Chân RESET| Đầu ra CMOS | Chế độ xả mở |
| V                        | V           | 0          | 1            | 1               | X         | V           | X               |
| Hoạt động cao              | Không sử dụng    | THẤP        | Vô hạn     | 1.6 ms       | N/A       | Hiện tại     | N/A             |

## Getting Started


### Đối với Arduino

Bản demo này sẽ chỉ cho bạn cách bật / tắt đèn LED.

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-Touch_Sensor |Grove-LED|
|--------------|-------------|-----------------|-----|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/45d_small.jpg)|![enter image description](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/45d_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Touch-Sensor-p-747.html)|[Get One Now](https://www.seeedstudio.com/Grove-Red-LED-p-1142.html)|

- **Bước 2.** Kết nối Grove-Touch_Sensor tới cổng **D2** của Grove-Base Shield.
- **Bước 3.** Kết nối Grove-LED tới cổng **D3** của Grove-Base Shield.
- **Bước 4.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 5.** Kết nối Seeeduino tới PC qua một cáp USB.



![with_ardu](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/with_ardu.jpg)

#### Phần mềm
 - **Bước 1.** Vui lòng sao chép và dán code dưới vào một sketch mới.
```c
const int TouchPin=2;
const int ledPin=3;

void setup() {
    pinMode(TouchPin, INPUT);
    pinMode(ledPin,OUTPUT);
}

void loop() {
    int sensorValue = digitalRead(TouchPin);
    if(sensorValue==1)
    {
        digitalWrite(ledPin,HIGH);
    }
    else
    {
        digitalWrite(ledPin,LOW);
    }
}
```
**Bước 2.** Giám sát LED bật và tắt.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Touch Sensor tới cổng D2, và kết nối Grove - Red LED tới cổng D3 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Step 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Touch_Sensor/master/image/cc_Touch_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã được tải lên, đèn LED sẽ sáng khi bạn chạm vào Cảm biến cảm ứng.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Touch Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/45d_small.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-Touch-Sensor-p-747.html)|



- **Bước 2**. Cắm Grove Base Hat vào Raspberry
- **Bước 3**. Kết nối cảm biến cảm ứng với cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi với PC thông qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/Touch_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến cảm ứng với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.

#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện lệnh dưới đây để chạy code.

```
cd grove.py/grove
python grove_touch_sensor.py 12

```

Tiếp theo là mã grove_touch_sensor.py.

```python

import time
from grove.gpio import GPIO


class GroveTouchSensor(GPIO):
    def __init__(self, pin):
        super(GroveTouchSensor, self).__init__(pin, GPIO.IN)
        self._last_time = time.time()

        self._on_press = None
        self._on_release = None

    @property
    def on_press(self):
        return self._on_press

    @on_press.setter
    def on_press(self, callback):
        if not callable(callback):
            return

        if self.on_event is None:
            self.on_event = self._handle_event

        self._on_press = callback

    @property
    def on_release(self):
        return self._on_release

    @on_release.setter
    def on_release(self, callback):
        if not callable(callback):
            return

        if self.on_event is None:
            self.on_event = self._handle_event

        self._on_release = callback

    def _handle_event(self, pin, value):
        t = time.time()
        dt, self._last_time = t - self._last_time, t

        if value:
            if callable(self._on_press):
                self._on_press(dt)
        else:
            if callable(self._on_release):
                self._on_release(dt)

Grove = GroveTouchSensor


def main():
    import sys

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    touch = GroveTouchSensor(int(sys.argv[1]))

    def on_press(t):
        print('Pressed')
    def on_release(t):
        print("Released.")

    touch.on_press = on_press
    touch.on_release = on_release

    while True:
        time.sleep(1)


if __name__ == '__main__':
    main()


```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_touch_sensor.py 12
Pressed
Released.
Pressed
Released.
Pressed
Released.
Pressed
Released.
^CTraceback (most recent call last):
  File "grove_touch_sensor.py", line 110, in <module>
    main()
  File "grove_touch_sensor.py", line 106, in main
    time.sleep(1)
KeyboardInterrupt

```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây

<!--false link-->
| Raspberry pi | GrovePi_Plus | Grove-Touch_Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/45d_small.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](http://www.seeedstudio.com/Grove-Touch-Sensor-p-747.html)|


- **Step 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-Touch_Sensor  tới cổng **D2** của GrovePi_Plus.
- **Step 4.** Kết nối Raspberry tới PC qua cáp USB.

![with_rpi](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/with_rpi.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 3.** Thực hiện các lệnh bên dưới để sử dụng cảm biến này, vui lòng thay đổi cổng thành từ D4 sang D2.


```bash
python grove_touch_sensor.py
```

```Python
#!/usr/bin/env python
#
# GrovePi Example for using the Grove Touch Sensor (http://www.seeedstudio.com/wiki/Grove_-_Touch_Sensor)
#
# The GrovePi connects the Raspberry Pi and Grove sensors.  You can learn more about GrovePi here:  http://www.dexterindustries.com/GrovePi
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

# Connect the Grove Touch Sensor to digital port D2
# SIG,NC,VCC,GND
touch_sensor = 2

grovepi.pinMode(touch_sensor,"INPUT")

while True:
    try:
        print(grovepi.digitalRead(touch_sensor))
        time.sleep(.5)

    except IOError:
        print ("Error")

```
Đây là kết quả:

![](https://github.com/SeeedDocument/Grove-Touch_Sensor/raw/master/img/rpi_result.jpg)


## Nguồn


-  **[Eagle]** [Grove-Touch_Sensor Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Touch_Sensor/master/res/Touch_sensor_Eagle_File.zip)
-  **[PDF]** [TTP223](https://raw.githubusercontent.com/SeeedDocument/Grove-Touch_Sensor/master/res/TTP223.pdf)
-  **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Touch_Sensor/master/resource/Grove_Touch_Sensor_CDC_File.zip)


## Dự án 

**Sử dụng Grove Touch Sensor để điều khiển Grove LED**: Cách kết nối và sử dụng Grove Touch Sensor để điều khiển bộ kit Grove LED.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/user50338573/using-grove-touch-sensor-to-control-grove-led-56a5ed/embed' width='350'></iframe>

**Cảm biến module Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/VFKYYG_hNUE" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/vPkf4czFQsY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


## Hỗ trợ kỹ thuật

Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>