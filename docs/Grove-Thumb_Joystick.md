---
name: Grove - Thumb Joystick
category: Sensor
bzurl: https://seeedstudio.com/Grove-Thumb-Joystick-p-935.html
oldwikiname: Grove_-_Thumb_Joystick
prodimagename: Bgjoy1.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/bgjoy1.jpg
surveyurl: https://www.research.net/r/Grove-Thumb_Joystick
sku: 101020028
tags: grove_analog, io_3v3, io_5v, plat_duino,plat_pi
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Bgjoy1.jpg)

Grove - Thumb Joystick là một module tương thích Grove rất giống với cần điều khiển 'tương tự' trên bộ điều khiển PS2 (PlayStation 2). Trục X và Y là hai chiết áp ~ 10k điều khiển chuyển động 2D bằng cách tạo tín hiệu tương tự. Cần điều khiển cũng có một nút ấn có thể được sử dụng cho các ứng dụng đặc biệt. Khi module ở chế độ làm việc, nó sẽ xuất ra hai giá trị tương tự, đại diện cho hai hướng. So với một phím điều khiển thông thường, các giá trị đầu ra của nó bị giới hạn trong phạm vi nhỏ hơn (tức là 200 ~ 800), chỉ khi được nhấn, giá trị X sẽ được đặt thành 1023 và MCU có thể phát hiện hành động nhấn.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Thumb-Joystick-p-935.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove - Thumb Joystick V1.1 | Ban đầu                                                                                                                                                                                    | 10/2016      |

## Các thông số kỹ thuật

| Item                                | Min  | Điển hình | Max  | Đơn vị |
|-------------------------------------|------|---------|------|------|
| Điện áp hoạt động                     | 4.75 | 5.0     | 5.25 | V    |
| Giá trị đầu ra tương tự（toạ độ X） | 206  | 516     | 798  | \    |
| Giá trị đầu ra tương tự （toạ độ Y） | 203  | 507     | 797  | \    |

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

#### Thuyết minh
Grove - Thumb Joystick là một thiết bị tương tự phát ra tín hiệu tương tự từ 0 đến 1023. Điều đó đòi hỏi chúng ta phải sử dụng cổng tương tự của Arduino để đọc.

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Thumb Joystick |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Bgjoy1_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Thumb-Joystick-p-935.html)|

- **Bước 2.** Kết nối module tới **A0/A1** của Grove - Base Shieldby sử dụng cáp Grove 4 chân.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Grove-Thumb_Joystick.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Thumb Joystick tới Seeeduino như dưới đây.

| Seeeduino       | Grove - Thumb Joystick |
|-----------------|-------------------------|
| 5V              | Đỏ                     |
| GND             | Đen                   |
| A1              | Trắng                   |
| A0              | Vàng                  |

#### Phần mềm

- **Bước 1.** Sao chép và dán code sau vào sketch mới.

```c
/*
  Thumb Joystick demo v1.0
  by:http://www.seeedstudio.com
  connect the module to A0&A1 for using;
*/

void setup()
{
    Serial.begin(9600);
}

void loop()
{
    int sensorValue1 = analogRead(A0);
    int sensorValue2 = analogRead(A1);

    Serial.print("The X and Y coordinate is:");
    Serial.print(sensorValue1, DEC);
    Serial.print(",");
    Serial.println(sensorValue2, DEC);
    Serial.println(" ");
    delay(200);
}
```

- **Bước 2.** Bạn có thể kiểm tra các giá trị của tín hiệu tương tự đầu ra bằng cách mở Màn hình nối tiếp.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Grove-Thumd_Joystick_Result.jpg)

Giá trị đầu ra từ cổng tương tự của Arduino có thể được chuyển đổi thành điện trở tương ứng bằng cách sử dụng công thức: R = (float) (1023-sensorValue) \ * 10 / sensorValue.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Thumb Joystick tới cổng A0 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/cc_Thumb_Joystick.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã được tải lên, bạn sẽ thấy toạ độ của X và Y sẽ được hiển thị trên Màn hình Nối tiếp.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Thumb Joystick |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Bgjoy1_small.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Thumb-Joystick-p-935.html)|



- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Thumb Joystick  tới cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Thumb_Hat.jpg)


!!!Chú thích
     Đối với bước 3, bạn có thể kết nối phím điều khiển ngón tay cái với **bất kỳ cổng tương tự nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_thumb_joystick.py 0

```
!!!Chú ý
    Bạn có thể loại bỏ chương trình với ++ python grove_thumb_joystick.py pin ++, trong đó chân có thể là một trong {0, 2, 4, 6} trong nhóm ADC và kết nối thiết bị với khe tương ứng {A0, A2, A4, A6} .

Dưới đây là code  grove_thumb_joystick.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveThumbJoystick:

    def __init__(self, channelX, channelY):
        self.channelX = channelX
        self.channelY = channelY
        self.adc = ADC()

    @property
    def value(self):
        return self.adc.read(self.channelX), self.adc.read(self.channelY)

Grove = GroveThumbJoystick


def main():
    from grove.helper import SlotHelper
    sh = SlotHelper(SlotHelper.ADC)
    pin = sh.argv2pin()

    sensor = GroveThumbJoystick(int(pin), int(pin + 1))

    while True:
        x, y = sensor.value
        if x > 900:
            print('Joystick Pressed')
        print("X, Y = {0} {1}".format(x, y))
        time.sleep(.2)

if __name__ == '__main__':
    main()


```
!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_thumb_joystick.py 0
Hat Name = 'Grove Base Hat RPi'
X, Y = 506 484
X, Y = 484 484
X, Y = 506 484
X, Y = 506 487
Joystick Pressed
X, Y = 999 485
X, Y = 310 736
X, Y = 681 484
Joystick Pressed
X, Y = 999 277
Joystick Pressed
X, Y = 999 487
X, Y = 506 484
X, Y = 501 486
X, Y = 509 484
X, Y = 511 486
X, Y = 510 485
^CTraceback (most recent call last):
  File "grove_thumb_joystick.py", line 69, in <module>
    main()
  File "grove_thumb_joystick.py", line 66, in main
    time.sleep(.2)
KeyboardInterrupt

```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

!!!Để ý
        Bạn có thể nhận thấy rằng đối với cổng analog, số pin màn hình có dạng như **A1, A0**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm module vào đúng cổng, nếu không có thể có xung đột chân.




### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Thumb Joystick |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Bgjoy1_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Thumb-Joystick-p-935.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Thumb Joystick ranger tới cổng **A0** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Thumb_Joystick/raw/master/img/Pi_Joystick%20connection.jpg)

#### Phần mềm

- **Bước 1.** Điều hướng đến thư mục của các bản demo:

```
cd yourpath/GrovePi/Software/Python/

```

- **Bước 2.**  Để thấy code

```
nano grove_thumb_joystick.py   # "Ctrl+x" to exit #
```

```python
import time
import grovepi

# Connect the Grove Thumb Joystick to analog port A0

# GrovePi Port A0 uses Arduino pins 0 and 1
# GrovePi Port A1 uses Arduino pins 1 and 2
# Don't plug anything into port A1 that uses pin 1
# Most Grove sensors only use 3 of their 4 pins, which is why the GrovePi shares Arduino pins between adjacent ports
# If the sensor has a pin definition SIG,NC,VCC,GND, the second (white) pin is not connected to anything

# If you wish to connect two joysticks, use ports A0 and A2 (skip A1)

# Uses two pins - one for the X axis and one for the Y axis
# This configuration means you are using port A0
xPin = 0
yPin = 1
grovepi.pinMode(xPin,"INPUT")
grovepi.pinMode(yPin,"INPUT")

# The Grove Thumb Joystick is an analog device that outputs analog signal ranging from 0 to 1023
# The X and Y axes are two ~10k potentiometers and a momentary push button which shorts the x axis

# My joystick produces slightly different results to the specifications found on the url above
# I've listed both here:

# Specifications
#     Min  Typ  Max  Click
#  X  206  516  798  1023
#  Y  203  507  797

# My Joystick
#     Min  Typ  Max  Click
#  X  253  513  766  1020-1023
#  Y  250  505  769
while True:
    try:
        # Get X/Y coordinates
        x = grovepi.analogRead(xPin)
        y = grovepi.analogRead(yPin)

        # Calculate X/Y resistance
        Rx = (float)(1023 - x) * 10 / x
        Ry = (float)(1023 - y) * 10 / y

        # Was a click detected on the X axis?
        click = 1 if x >= 1020 else 0

        print "x =", x, " y =", y, " Rx =", Rx, " Ry =", Ry, " click =", click
        time.sleep(.5)

    except IOError:
        print "Error"
```

- **Bước 3.** Chạy demo.

```
sudo python grove_thumb_joystick.py
```

- **Bước 4.** Chúng ta sẽ thấy màn hình đầu ra trên terminal như dưới đây.

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/pi_result.png)|

Nguồn
---------

- **[Eagle]** [Grove-Thumb Joystick Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/res/Eagle_Design_Files.zip)
- **[Datasheet]** [Analog Joystick Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/res/Analog_Joystick_Datasheet.jpg)
- **[PDF]** [Joystick Schematic PDF File](https://github.com/SeeedDocument/Grove-Thumb_Joystick/raw/master/res/Joystick.pdf)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/res/Grove_Thumb_Joystick_CDC_File.zip)

## Dự án 

**Máy chủ âm nhạc Raspberry pi**: Bước đầu tiên đến dự án Raspberry Pi.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/kishima7/raspberry-pi-music-server-f5a0ae/embed' width='350'></iframe>

**Xây dựng bộ điều khiển Minecraft tùy chỉnh**: Xây dựng bộ điều khiển Minecraft tùy chỉnh với GrovePi.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/dexterindustries/build-a-custom-minecraft-controller-d55d9c/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>