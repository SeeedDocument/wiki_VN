---
name: Grove - LED Bar
category: Display
bzurl: https://seeedstudio.com/Grove-LED-Bar-p-1178.html
oldwikiname: Grove_-_LED_Bar
prodimagename: Grove-LED_Bar-1.jpg
surveyurl: https://www.research.net/r/Grove-LED_Bar
sku: 104030002
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/img/Grove-LED_Bar-1.jpg)

Grove – LED Bar bao gồm một thanh đo LED 10 đoạn và chip điều khiển LED MY9221. Nó có thể được sử dụng làm chỉ số cho thời lượng pin còn lại, điện áp, mực nước, âm lượng nhạc hoặc các giá trị khác yêu cầu hiển thị độ dốc. Có 10 thanh LED trong biểu đồ thanh LED: một màu đỏ, một màu vàng, một màu xanh lục nhạt và bảy thanh màu lục. Mã demo có sẵn để giúp bạn khởi động và chạy nhanh. Nó chiếu sáng các đèn LED liên tục từ đỏ sang xanh lục, do đó toàn bộ biểu đồ thanh được thắp sáng cuối cùng. Bạn muốn đi xa hơn? Đi trước và tạo hiệu ứng của riêng bạn.

<p style=":center"><a href="https://www.seeedstudio.com/s/Grove-LED-Bar-v2.0-p-2474.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

Phiên bản
--------

| Phiên bản sản phẩm              | Thay đổi                                   | Ngày phát hành |
|------------------------------|-------------------------------------------|---------------|
| Grove – LED Bar V1 | Ban đầu                                   | 06/2014     |
| Grove – LED Bar V2 | Cải thiện nguồn điện                                   | 10/2015     |

Đặc tính
--------

-   Điện áp đầu vào: 3.3V/5V
-   Mỗi phân đoạn LED có thể được điều khiển riêng thông qua mã
-   Hiển thị trực quan
-   Tùy chọn nguồn linh hoạt, hỗ trợ 3-5,5DC
-   Mã demo có sẵn
-   Thư viện tương thích Suli

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)


## Các thông số kỹ thuật

| Thông số                                                   | Giá trị  |
|-------------------------------------------------------------|--------------|
| Điện áp hoạt động                                           | 3.3/5V       |
| Nhiệt độ hoạt động                                        | -20℃ to +80℃ |
| Bước sóng phát xạ cực đại-ĐỎ (Dòng 20mA)                  | 630-637nm    |
| Bước sóng phát xạ cực đại-Vàng xanh(Dòng  20mA )       | 570-573nm    |
| Bước sóng phát xạ cực đại-Vàng (Dòng 20mA)             | 585-592nm    |
| Cường độ sáng trên mỗi phân đoạn-ĐỎ (Dòng 20mA)          | 50-70mcd     |
| Cường độ sáng trên mỗi phân đoạn-Vàng xanh(Dòng  20mA ) | 28-35mcd     |
| Cường độ sáng trên mỗi phân đoạn-Vàng(Dòng  20mA )       | 45-60mcd     |
| Phân khúc LED                                                 | 10           |
| Kích thước                                                        | 40mm * 20mm  |


Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


Getting Started
-------------

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-LED Bar |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/img/Grove-LED_Bar-3.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/s/Grove-LED-Bar-v2.0-p-2474.html)|

- **Bước 2.** Kết nối Grove-LED Bar tới cổng **D8** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-LED_Bar/raw/master/img/seeeduino_ledbar.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield,chúng tôi cũng có thể kết nối trực tiếp Grove-LED Bar tới Seeeduino như dưới đây.

| Seeeduino       | Grove-LED Bar |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| D9            | Trắng                   |
| D8            | Vàng                  |

**Phần mềm**

- **Step 1.** Tải xuống  [Grove - LED Bar Library](https://github.com/Seeed-Studio/Grove_LED_Bar) từ Github

- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.

- **Bước 3.** Khởi động lại Arduino IDE. Mở ví dụ “Level” qua đường dẫn : **File --> Examples --> Grove LED Bar --> Level**.

![](https://github.com/SeeedDocument/Grove-LED_Bar/raw/master/img/code.png)

- **Bước 4.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra[ how to upload code](http://wiki.seeedstudio.com/Upload_Code/).

Kết quả sẽ như sau:

![](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/img/LED_Bar_shining.gif)

### Đối với Raspberry Pi

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove-LED Bar |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/img/Grove-LED_Bar-3.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/s/Grove-LED-Bar-v2.0-p-2474.html)|

- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.

- **Step 3.** Kết nối Grove-LED Bar tới cổng **D5** của GrovePi_Plus.

- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-LED_Bar/raw/master/img/rpi_ledbar.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.

- **Bước 2.** Thực hiện theo [Cập nhật Firmware](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/updating-firmware/) để cập nhật firmware mới nhất của GrovePi.


!!!Mẹo
    Trong wiki này, chúng tôi sử dụng đường dẫn **~/ GrovePi/** thay vì **/home/pi/Desktop/GrovePi**, bạn cần đảm bảo Bước 2 và Bước 3 sử dụng cùng một đường dẫn.


!!!Chú ý
    Chúng tôi đề nghị bạn cập nhật chương trình firmware hoặc đối với một số cảm biến bạn có thể gặp lỗi.

- **Bước 3.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Bước 4.** Điều hướng đến thư mục của các bản demo:

```
cd yourpath/GrovePi/Software/Python/
```

Đây là code grove_ledbar.py.

```python
import time
import grovepi
import random

# Connect the Grove LED Bar to digital port D5
# DI,DCKI,VCC,GND
ledbar = 5

grovepi.pinMode(ledbar,"OUTPUT")
time.sleep(1)
i = 0

# LED Bar methods
# grovepi.ledBar_init(pin,orientation)
# grovepi.ledBar_orientation(pin,orientation)
# grovepi.ledBar_setLevel(pin,level)
# grovepi.ledBar_setLed(pin,led,state)
# grovepi.ledBar_toggleLed(pin,led)
# grovepi.ledBar_setBits(pin,state)
# grovepi.ledBar_getBits(pin)

    while True:
        try:
        print "Test 1) Initialise - red to green"
        # ledbar_init(pin,orientation)
        # orientation: (0 = red to green, 1 = green to red)
        grovepi.ledBar_init(ledbar, 0)
        time.sleep(.5)


        print "Test 2) Set level"
        # ledbar_setLevel(pin,level)
        # level: (0-10)
        for i in range(0,11):
            grovepi.ledBar_setLevel(ledbar, i)
            time.sleep(.2)
        time.sleep(.3)

        grovepi.ledBar_setLevel(ledbar, 8)
        time.sleep(.5)

        grovepi.ledBar_setLevel(ledbar, 2)
        time.sleep(.5)

        grovepi.ledBar_setLevel(ledbar, 5)
        time.sleep(.5)


        print "Test 3) Switch on/off a single LED"
        # ledbar_setLed(pin,led,state)
        # led: which led (1-10)
        # state: off or on (0,1)
        grovepi.ledBar_setLed(ledbar, 10, 1)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 9, 1)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 8, 1)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 1, 0)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 2, 0)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 3, 0)
        time.sleep(.5)


        print "Test 4) Toggle a single LED"
        # flip a single led - if it is currently on, it will become off and vice versa
        # ledbar_toggleLed(ledbar, led)
        grovepi.ledBar_toggleLed(ledbar, 1)
        time.sleep(.5)

        grovepi.ledBar_toggleLed(ledbar, 2)
        time.sleep(.5)

        grovepi.ledBar_toggleLed(ledbar, 9)
        time.sleep(.5)

        grovepi.ledBar_toggleLed(ledbar, 10)
        time.sleep(.5)


        print "Test 5) Set state - control all leds with 10 bits"
        # ledbar_setBits(ledbar, state)
        # state: (0-1023) or (0x00-0x3FF) or (0b0000000000-0b1111111111) or (int('0000000000',2)-int('1111111111',2))
        for i in range(0,32):
            grovepi.ledBar_setBits(ledbar, i)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 6) Get current state"
        # state = ledbar_getBits(ledbar)
        # state: (0-1023) a bit for each of the 10 LEDs
        state = grovepi.ledBar_getBits(ledbar)
        print "with first 5 leds lit, the state should be 31 or 0x1F"
        print state

        # bitwise shift five bits to the left
        state = state << 5
        # the state should now be 992 or 0x3E0
        # when saved the last 5 LEDs will be lit instead of the first 5 LEDs
        time.sleep(.5)


        print "Test 7) Set state - save the state we just modified"
        # ledbar_setBits(ledbar, state)
        # state: (0-1023) a bit for each of the 10 LEDs
        grovepi.ledBar_setBits(ledbar, state)
        time.sleep(.5)


        print "Test 8) Swap orientation - green to red - current state is preserved"
        # ledbar_orientation(pin,orientation)
        # orientation: (0 = red to green, 1 = green to red)
        # when you reverse the led bar orientation, all methods know how to handle the new LED index
        # green to red
        grovepi.ledBar_orientation(ledbar, 1)
        time.sleep(.5)

        # red to green
        grovepi.ledBar_orientation(ledbar, 0)
        time.sleep(.5)

        # green to red
        grovepi.ledBar_orientation(ledbar, 1)
        time.sleep(.5)


        print "Test 9) Set level, again"
        # ledbar_setLevel(pin,level)
        # level: (0-10)
        # note the red LED is now at index 10 instead of 1
        for i in range(0,11):
            grovepi.ledBar_setLevel(ledbar, i)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 10) Set a single LED, again"
        # ledbar_setLed(pin,led,state)
        # led: which led (1-10)
        # state: off or on (0,1)
        grovepi.ledBar_setLed(ledbar, 1, 0)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 3, 0)
        time.sleep(.5)

        grovepi.ledBar_setLed(ledbar, 5, 0)
        time.sleep(.5)


        print "Test 11) Toggle a single LED, again"
        # ledbar_toggleLed(ledbar, led)
        grovepi.ledBar_toggleLed(ledbar, 2)
        time.sleep(.5)

        grovepi.ledBar_toggleLed(ledbar, 4)
        time.sleep(.5)


        print "Test 12) Get state"
        # state = ledbar_getBits(ledbar)
        # state: (0-1023) a bit for each of the 10 LEDs
        state = grovepi.ledBar_getBits(ledbar)

        # the last 5 LEDs are lit, so the state should be 992 or 0x3E0

        # bitwise shift five bits to the right
        state = state >> 5
        # the state should now be 31 or 0x1F


        print "Test 13) Set state, again"
        # ledbar_setBits(ledbar, state)
        # state: (0-1023) a bit for each of the 10 LEDs
        grovepi.ledBar_setBits(ledbar, state)
        time.sleep(.5)


        print "Test 14) Step"
        # step through all 10 LEDs
        for i in range(0,11):
            grovepi.ledBar_setLevel(ledbar, i)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 15) Bounce"
        # switch on the first two LEDs
        grovepi.ledBar_setLevel(ledbar, 2)

        # get the current state (which is 0x3)
        state = grovepi.ledBar_getBits(ledbar)

        # bounce to the right
        for i in range(0,9):
            # bit shift left and update
            state <<= 1;
            grovepi.ledBar_setBits(ledbar, state)
            time.sleep(.2)

        # bounce to the left
        for i in range(0,9):
            # bit shift right and update
            state >>= 1;
            grovepi.ledBar_setBits(ledbar, state)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 16) Random"
        for i in range(0,21):
            state = random.randint(0,1023)
            grovepi.ledBar_setBits(ledbar, state)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 17) Invert"
        # set every 2nd LED on - 341 or 0x155
        state = 341
        for i in range(0,5):
            grovepi.ledBar_setBits(ledbar, state)
            time.sleep(.2)

            # bitwise XOR all 10 LEDs on with the current state
            state = 0x3FF ^ state

            grovepi.ledBar_setBits(ledbar, state)
            time.sleep(.2)
        time.sleep(.3)


        print "Test 18) Walk through all possible combinations"
        for i in range(0,1024):
            grovepi.ledBar_setBits(ledbar, i)
            time.sleep(.1)
        time.sleep(.4)

    except KeyboardInterrupt:
        grovepi.ledBar_setBits(ledbar, 0)
        break
    except IOError:
        print "Error"
```

- **Step 5.** Chạy demo.

```
sudo python grove_ledbar.py
```

Nguồn
---------

-   [**Eagle&PDF**][Grove - LED Bar Eagle File](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/res/Grove-LED_Bar_v1.0.zip)
-   [**Library**][Grove - LED Bar Library](https://github.com/Seeed-Studio/Grove_LED_Bar)
-   [**Library**][Suli-compatible Library](https://github.com/Seeed-Studio/LED_Bar_Suli)
-   [**Datasheet**][MY9221 Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/res/MY9221_DS_1.0.pdf)
-   [**More Reading**][Wooden Laser Gun](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)



## Dự án

**Thanh LED Grove v2.0**: Calliope Mini được trang bị hai đầu nối Grove. Trong dự án này, tôi muốn khám phá, làm thế nào để nói chuyện với những phần Seeed Grove này.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/luuc/grove-led-bar-v2-0-c4b74f/embed' width='350'></iframe>

**Grove LED Bar điều khiển với Bean+**: Tìm hiểu những điều cơ bản về việc sử dụng các thành phần Grove phổ biến với LightBlue Bean + mới để bắt đầu xây dựng các dự án của riêng bạn!

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/karel/grove-led-bar-controller-with-the-bean-c3b81e/embed' width='350'></iframe>


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>