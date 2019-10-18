---
name: Grove - 4-Digit Display
category: Display
bzurl: https://seeedstudio.com/Grove-4-Digit-Display-p-1198.html
oldwikiname: Grove_-_4-Digit_Display
prodimagename: Grove-4_digit_display.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/4-Digital Display.jpg
surveyurl: https://www.research.net/r/Grove-4-Digit_Display
sku: 104030003
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_pi, plat_wio
---

[![](https://raw.githubusercontent.com/SeeedDocument/Grove-4-Digit_Display/master/img/Grove-4_digit_display.jpg)](http://www.seeedstudio.com/depot/grove-4digital-display-p-1198.html)

 Module Grove - hiển thị 4 chữ số là module 12 chân. Trong module này, chúng tôi sử dụng TM1637 để giảm số lượng chân điều khiển xuống còn 2. Có nghĩa là, nó điều khiển cả nội dung và độ chói thông qua chỉ 2 chân kỹ thuật số của Arduino hoặc Seeeduino. Đối với các dự án yêu cầu hiển thị dạng số alpha, đây có thể là một lựa chọn tốt.

<p style=":center"><a href="https://www.seeedstudio.com/grove-4digital-display-p-1198.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>


## Phiên bản

| Phiên bản sản phẩm              | Các thay đổi                                   | Ngày phát hành |
|------------------------------|-------------------------------------------|---------------|
|Grove - 4-Digit Display V1.0  | Ban đầu                                   | 05/2012      |     

## Đặc tính

-   Hiển thị chữ số đỏ 4 chữ số
-   Giao diện tương thích Grove (3.3V / 5V)
-   8 mức độ chói có thể điều chỉnh

!!!Lời khuyên
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

##  Các thông số kỹ thuật

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
3.3
</td>
<td>
5.0
</td>
<td>
5.5
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Dòng điện
</th>
<td>
0.2
</td>
<td>
27
</td>
<td>
80
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<th scope="row">
Kích thước
</th>
<td colspan="3">
42x24x14
</td>
<td>
mm
</td>
</tr>
<tr align="center">
<th scope="row">
Khối lượng tịnh
</th>
<td colspan="3">
7±1
</td>
<td>
g
</td>
</tr>
</table>

## Ý tưởng ứng dụng

-   Hiển thị thời gian
-   Đồng hồ bấm giờ
-   Hiển thị đầu vào của cảm biến

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-4-Digit Display |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/500px-Grove_-_4_digit_display_s.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/grove-4digital-display-p-1198.html)|

- **Bước 2.** Kết nối Grove-4-Digit Display tới cổng **D2** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/seeeduino_digital_led.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-4-Digit Display tới Seeeduino như dưới đây. Chúng tôi cũng có thể cắm Grove-4-Digit Display đến cổng kỹ thuật số Grove khác.

| Seeeduino |  Grove-4-Digit Display |
|-----------|-----------------|
| 5V        | Đỏ             |
| GND       | Đen           |
| D3        | Trắng (DIO)     |
| D2        | Vàng(CLK)     | 

!!!cảnh báo
     Màn hình Grove-4-Digit bao gồm 4 chân, GND, VCC, DIO, CLK. Chúng tôi có thể kết nối DIO và CLK với bất kỳ pin kỹ thuật số nào. Nó không phải là giao thức I2C.

**Phần mềm**


- **Bước 1.** Tải xuống  [Grove-4-Digit Display Library](https://github.com/Seeed-Studio/Grove_4Digital_Display/archive/master.zip) và [TimerOne Library](https://code.google.com/p/arduino-timerone/downloads/detail?name=TimerOne-v9.zip&can=2&q=).
- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.
- **Bước 3.** Thực hiện theo các hướng dẫn bên dưới để chọn mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra[how to upload code](http://wiki.seeedstudio.com/Upload_Code/). There are 3 examples as below.
    - Hiển thị đồng hồ
    - Lưu lượng số
    - Đồng hồ bấm giờ

![](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/arduino_example.jpg)

- **Bước 4.** Chúng ta sẽ thấy Màn hình Grove-4-Digit được bật.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - 4-Digit Diaplsy tới cổng D2 của Base Shield

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** ết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/4-Digit_Display.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy số chảy từ 0 đến 9.


### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - 4 Digit Display |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/500px-Grove_-_4_digit_display_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/grove-4digital-display-p-1198.html)|

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**. Kết nối 4-digit display tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/Digit_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


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
python grove_4_digit_display.py 12 13

```

Dưới đây là mã grove_4_digit_display.py.

```python

import sys
import time
from grove.gpio import GPIO


charmap = {
    '0': 0x3f,
    '1': 0x06,
    '2': 0x5b,
    '3': 0x4f,
    '4': 0x66,
    '5': 0x6d,
    '6': 0x7d,
    '7': 0x07,
    '8': 0x7f,
    '9': 0x6f,
    'A': 0x77,
    'B': 0x7f,
    'b': 0x7C,
    'C': 0x39,
    'c': 0x58,
    'D': 0x3f,
    'd': 0x5E,
    'E': 0x79,
    'F': 0x71,
    'G': 0x7d,
    'H': 0x76,
    'h': 0x74,
    'I': 0x06,
    'J': 0x1f,
    'K': 0x76,
    'L': 0x38,
    'l': 0x06,
    'n': 0x54,
    'O': 0x3f,
    'o': 0x5c,
    'P': 0x73,
    'r': 0x50,
    'S': 0x6d,
    'U': 0x3e,
    'V': 0x3e,
    'Y': 0x66,
    'Z': 0x5b,
    '-': 0x40,
    '_': 0x08,
    ' ': 0x00
}

ADDR_AUTO = 0x40
ADDR_FIXED = 0x44
STARTADDR = 0xC0
BRIGHT_DARKEST = 0
BRIGHT_DEFAULT = 2
BRIGHT_HIGHEST = 7


class Grove4DigitDisplay(object):
    colon_index = 1

    def __init__(self, clk, dio, brightness=BRIGHT_DEFAULT):
        self.brightness = brightness

        self.clk = GPIO(clk, direction=GPIO.OUT)
        self.dio = GPIO(dio, direction=GPIO.OUT)
        self.data = [0] * 4
        self.show_colon = False

    def clear(self):
        self.show_colon = False
        self.data = [0] * 4
        self._show()

    def show(self, data):
        if type(data) is str:
            for i, c in enumerate(data):
                if c in charmap:
                    self.data[i] = charmap[c]
                else:
                    self.data[i] = 0
                if i == self.colon_index and self.show_colon:
                    self.data[i] |= 0x80
                if i == 3:
                    break
        elif type(data) is int:
            self.data = [0, 0, 0, charmap['0']]
            if data < 0:
                negative = True
                data = -data
            else:
                negative = False
            index = 3
            while data != 0:
                self.data[index] = charmap[str(data % 10)]
                index -= 1
                if index < 0:
                    break
                data = int(data / 10)

            if negative:
                if index >= 0:
                    self.data[index] = charmap['-']
                else:
                    self.data = charmap['_'] + [charmap['9']] * 3
        else:
            raise ValueError('Not support {}'.format(type(data)))
        self._show()

    def _show(self):
        with self:
            self._transfer(ADDR_AUTO)

        with self:
            self._transfer(STARTADDR)
            for i in range(4):
                self._transfer(self.data[i])

        with self:
            self._transfer(0x88 + self.brightness)

    def update(self, index, value):
        if index < 0 or index > 4:
            return

        if value in charmap:
            self.data[index] = charmap[value]
        else:
            self.data[index] = 0

        if index == self.colon_index and self.show_colon:
            self.data[index] |= 0x80

        with self:
            self._transfer(ADDR_FIXED)

        with self:
            self._transfer(STARTADDR | index)
            self._transfer(self.data[index])

        with self:
            self._transfer(0x88 + self.brightness)


    def set_brightness(self, brightness):
        if brightness > 7:
            brightness = 7

        self.brightness = brightness
        self._show()

    def set_colon(self, enable):
        self.show_colon = enable
        if self.show_colon:
            self.data[self.colon_index] |= 0x80
        else:
            self.data[self.colon_index] &= 0x7F
        self._show()

    def _transfer(self, data):
        for _ in range(8):
            self.clk.write(0)
            if data & 0x01:
                self.dio.write(1)
            else:
                self.dio.write(0)
            data >>= 1
            time.sleep(0.000001)
            self.clk.write(1)
            time.sleep(0.000001)

        self.clk.write(0)
        self.dio.write(1)
        self.clk.write(1)
        self.dio.dir(GPIO.IN)

        while self.dio.read():
            time.sleep(0.001)
            if self.dio.read():
                self.dio.dir(GPIO.OUT)
                self.dio.write(0)
                self.dio.dir(GPIO.IN)
        self.dio.dir(GPIO.OUT)

    def _start(self):
        self.clk.write(1)
        self.dio.write(1)
        self.dio.write(0)
        self.clk.write(0)

    def _stop(self):
        self.clk.write(0)
        self.dio.write(0)
        self.clk.write(1)
        self.dio.write(1)

    def __enter__(self):
        self._start()

    def __exit__(self, exc_type, exc_val, exc_tb):
        self._stop()


Grove = Grove4DigitDisplay


def main():
    if len(sys.argv) < 3:
        print('Usage: {} clk dio'.format(sys.argv[0]))
        sys.exit(1)

    display = Grove4DigitDisplay(int(sys.argv[1]), int(sys.argv[2]))

    count = 0
    while True:
        t = time.strftime("%H%M", time.localtime(time.time()))
        display.show(t)
        display.set_colon(count & 1)
        count += 1
        time.sleep(1)


if __name__ == '__main__':
    main()

```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, màn hình 4 chữ số sẽ hiển thị thời gian hiện tại.


Bạn có thể thoát khỏi chương trình này bằng cách nhấn ++ ctrl + c ++.


### Đối với Raspberry Pi (với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove-4-Digit Display |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/500px-Grove_-_4_digit_display_s.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/grove-4digital-display-p-1198.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-4-Digit Display tới cổng **D5** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/image/rpi_digital_led.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.

- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Bước 3.** Thực hiện các lệnh dưới đây để có được giá trị.


```python
cd ~/GrovePi/Software/Python
python grove_4_digit_display.py
```

Đây là mã grove_4_digit_display.py.

```python
# NOTE: 4x red 7 segment display with colon and 8 luminance levels, but no decimal points

import time
import grovepi

# Connect the Grove 4 Digit Display to digital port D5
# CLK,DIO,VCC,GND
display = 5
grovepi.pinMode(display,"OUTPUT")

# If you have an analog sensor connect it to A0 so you can monitor it below
sensor = 0
grovepi.pinMode(sensor,"INPUT")

time.sleep(.5)

# 4 Digit Display methods
# grovepi.fourDigit_init(pin)
# grovepi.fourDigit_number(pin,value,leading_zero)
# grovepi.fourDigit_brightness(pin,brightness)
# grovepi.fourDigit_digit(pin,segment,value)
# grovepi.fourDigit_segment(pin,segment,leds)
# grovepi.fourDigit_score(pin,left,right)
# grovepi.fourDigit_monitor(pin,analog,duration)
# grovepi.fourDigit_on(pin)
# grovepi.fourDigit_off(pin)

while True:
    try:
        print ("Test 1) Initialise")
        grovepi.fourDigit_init(display)
        time.sleep(.5)

        print ("Test 2) Set brightness")
        for i in range(0,8):
            grovepi.fourDigit_brightness(display,i)
            time.sleep(.2)
        time.sleep(.3)

        # set to lowest brightness level
        grovepi.fourDigit_brightness(display,0)
        time.sleep(.5)

        print ("Test 3) Set number without leading zeros")
        leading_zero = 0
        grovepi.fourDigit_number(display,1,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,12,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,123,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,1234,leading_zero)
        time.sleep(.5)

        print ("Test 4) Set number with leading zeros")
        leading_zero = 1
        grovepi.fourDigit_number(display,5,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,56,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,567,leading_zero)
        time.sleep(.5)
        grovepi.fourDigit_number(display,5678,leading_zero)
        time.sleep(.5)

        print ("Test 5) Set individual digit")
        grovepi.fourDigit_digit(display,0,2)
        grovepi.fourDigit_digit(display,1,6)
        grovepi.fourDigit_digit(display,2,9)
        grovepi.fourDigit_digit(display,3,15) # 15 = F
        time.sleep(.5)

        print ("Test 6) Set individual segment")
        grovepi.fourDigit_segment(display,0,118) # 118 = H
        grovepi.fourDigit_segment(display,1,121) # 121 = E
        grovepi.fourDigit_segment(display,2,118) # 118 = H
        grovepi.fourDigit_segment(display,3,121) # 121 = E
        time.sleep(.5)

        grovepi.fourDigit_segment(display,0,57) # 57 = C
        grovepi.fourDigit_segment(display,1,63) # 63 = O
        grovepi.fourDigit_segment(display,2,63) # 63 = O
        grovepi.fourDigit_segment(display,3,56) # 56 = L
        time.sleep(.5)

        print ("Test 7) Set score")
        grovepi.fourDigit_score(display,0,0)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,0)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,1)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,2)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,3)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,4)
        time.sleep(.2)
        grovepi.fourDigit_score(display,1,5)
        time.sleep(.5)

        print ("Test 8) Set time")
        grovepi.fourDigit_score(display,12,59)
        time.sleep(.5)

        print ("Test 9) Monitor analog pin")
        seconds = 10
        grovepi.fourDigit_monitor(display,sensor,seconds)
        time.sleep(.5)

        print ("Test 10) Switch all on")
        grovepi.fourDigit_on(display)
        time.sleep(.5)

        print ("Test 11) Switch all off")
        grovepi.fourDigit_off(display)
        time.sleep(.5)

    except KeyboardInterrupt:
        grovepi.fourDigit_off(display)
        break
    except IOError:
        print ("Error")

```

- **Bước 4.** Chúng ta sẽ thấy Grove-4-Digit Display như bên dưới.

```python
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_4_digit_display.py 
Test 1) Initialise
Test 2) Set brightness
Test 3) Set number without leading zeros
Test 4) Set number with leading zeros
Test 5) Set individual digit
Test 6) Set individual segment
Test 7) Set score
Test 8) Set time
Test 9) Monitor analog pin
Test 10) Switch all on
Test 11) Switch all off
```


### Đối với TI LaunchPad

Hiển thị số (4-Digital-Display)

Ví dụ này trình bày cách hiển thị một số số bằng cách sử dụng Grove-4-Digital Display.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-4-Digit_Display/master/img/4_digital_display.jpg)

```
/*
 * TM1637.cpp
 * A library for the 4 digit display
 */
#include "TM1637.h"
#define CLK 39 //pins definitions for TM1637 and can be changed to other ports
#define DIO 38
TM1637 tm1637(CLK,DIO);
void setup()
{
    tm1637.init();
    tm1637.set(BRIGHT_TYPICAL);//BRIGHT_TYPICAL = 2,BRIGHT_DARKEST = 0,BRIGHTEST = 7;
}
void loop()
{
    int8_t NumTab[] = {0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15};//0~9,A,b,C,d,E,F
    int8_t ListDisp[4];
    unsigned char i = 0;
    unsigned char count = 0;
    delay(150);
    while(1)
    {
        i = count;
        count ++;
        if(count == sizeof(NumTab)) count = 0;
        for(unsigned char BitSelect = 0;BitSelect < 4;BitSelect ++)
        {
            ListDisp[BitSelect] = NumTab[i];
            i ++;
            if(i == sizeof(NumTab)) i = 0;
        }
        tm1637.display(0,ListDisp[0]);
        tm1637.display(1,ListDisp[1]);
        tm1637.display(2,ListDisp[2]);
        tm1637.display(3,ListDisp[3]);
        delay(300);
    }
}
```

## Nguồn

- **[Eagle&PDF]** [Grove-4-Digit Display V1.0 Schematic](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/resource/Grove%20-%204-Digit%20Display%20V1.0%20eagle%20files.zip)
- **[Library]** [4-Digit Display library](https://raw.githubusercontent.com/SeeedDocument/Grove-4-Digit_Display/master/res/DigitalTube.zip)
- **[Library]** [TimerOne library](https://code.google.com/p/arduino-timerone/downloads/detail?name=TimerOne-v9.zip&can=2&q=)
- **[Library]** [Four-Digit Display Suli Library](https://github.com/Seeed-Studio/Four_Digit_Display_Suli)
- **[Library]** [CodeCraft Code](https://github.com/SeeedDocument/Grove_4_Digit_Display/raw/master/resource/4-Digit%20Display.zip)
- **[Datasheet]** [TM1637 datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-4-Digit_Display/master/res/TM1637_datasheet.pdf)
- **[More Reading]** [The Wooden Laser Gun](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)

![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Lotus/master/img/gun.jpg)

Lấy cảm hứng từ OVERWATCH, chúng tôi đã tạo ra một đồ chơi Súng Laser bằng gỗ rất thú vị cho vui trong ngày này!

Súng Laser bằng gỗ và Mục tiêu súng đều dựa trên một bảng Arduino có tên là Seeeduino Lotus. Bộ phát laser trên Súng Laser được điều khiển để bắn xung laser để "kích hoạt" Mục tiêu súng. Và có 3 cảm biến ánh sáng trên Gun Target để phát hiện xung laser. Có vẻ rất đơn giản phải không? Nếu bạn quan tâm đến dự án của chúng tôi, hãy làm một cái cho chính bạn hoặc con bạn! Thật đáng để dành một ngày DIY nó như một món quà Xmas.

## Dự án

**Đồng hồ báo thức MSP430 với các mô-đun Grove**: Tạo đồng hồ báo thức của riêng bạn bằng LaunchPad MSP430F5529 và Module SeeedStudio Grove.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/carlosventura/alarm-clock-with-grove-modules-e4e9f1/embed' width='350'></iframe>

**Đồng hồ - Grove Hiển thị 4 chữ số bằng Photon**:　Đồng hồ đầu tiên của bạn với 4 thành phần, dựa trên Grove và TM1637

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ingo-lohs/clock-grove-4-digit-display-using-photon-7c4369/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>