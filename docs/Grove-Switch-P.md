---
name: Grove - Switch(P)
category: Sensor
bzurl: https://seeedstudio.com/Grove-Switch(P)-p-1252.html
oldwikiname: Grove_-_Switch(P)
prodimagename: GroveSwitchP_01.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/GroveSwitchP.jpg
surveyurl: https://www.research.net/r/Grove-Switch-P
sku: 101020004
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_linkit, plat_pi, plat_bbg
---

![](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/switch_p.jpg)

Grove – Switch là một slide SPDT nhỏ, rất phù hợp cho các tình huống của ON ON / OFF. Đó là một chuyển đổi đáng tin cậy về chất lượng xây dựng tuyệt vời mà chúng tôi áp dụng nó trên nhiều bảng của chúng tôi. Bạn nên dự trữ một số cho hệ thống tạo mẫu Grove của bạn.

“P” có nghĩa là gì? “P” là chữ viết tắt của “panel mount” trong sản phẩm.

<p style=":center"><a href="http://www.seeedstudio.com/Grove-Switch(P)-p-1252.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                   | Ngày phát hành |
|------------------------------|-------------------------------------------|---------------|
|Grove-Switch(P) V1.0          | Ban đầu                                   | 07/2012      |     


## Đặc tính

-   Giao diện Grove
-   Dễ sử dụng
-   Yếu tố Grove cơ bản

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật

| Tham số             | Giá trị    |
|-----------------------|----------------|
| Điện áp hoạt động     | 3.3/5V         |
| Vòng đời      | 10,000 cycles  |
| Lực hoạt động       | 200 ± 50gf     |
| Nhiệt độ hoạt động | -20℃ to +80℃   |
| Kích thước                | 20mm x 20mm      |


## Các nền tảng được hỗ trợ

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

| Seeeduino V4.2 | Base Shield|  Grove-Switch(P) |Grove - Purple LED (3mm)|
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/SwitchP_s.jpg)|![](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/grove_led_s.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Switch(P)-p-1252.html)|[Get One Now](https://www.seeedstudio.com/Grove-Purple-LED-%283mm%29-p-1143.html)|

- **Step 2.** Kết nối Grove-Switch(P) tới cổng **D2** của Grove-Base Shield.
- **Step 3.** Kết nối Grove-LED tới cổng **D6** của Grove-Base Shield.
- **Step 4.** Cắm Grove - Base Shield vào Seeeduino.
- **Step 5.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/seeeduino_switch_led.jpg)

!!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Switch(P) và Grove - Purple LED (3mm) tới Seeeduino như dưới đây.

| Seeeduino | Grove-Switch(P) | Seeeduino | Grove - Purple LED (3mm) |
|-----------|-----------------|-----------|--------------------------|
| 5V        | Đỏ             | 5V        | Đỏ                      |
| GND       | Đen           | GND       | Đen                    |
| NC        | Trắng           | NC        | Trắng                    |
| D2        | Vàng          | D6        | Vàng                   |

**Phần mềm**

- **Bước 1.** Vui lòng sao chép mã dưới đây vào Arduino IDE và tải lên arduino. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải code lên](http://wiki.seeedstudio.com/Upload_Code/).


```
const int switchPin = 2;     // the number of the pushbutton pin
const int ledPin =  6;      // the number of the LED pin

int switchState = 0;         // variable for reading the pushbutton status

void setup() {
    // initialize the LED pin as an output:
    pinMode(ledPin, OUTPUT);
    // initialize the switch pin as an input:
    pinMode(switchPin, INPUT);
    Serial.begin(9600);
}

void loop(){
    // read the state of the switch value:
    switchState = digitalRead(switchPin);

    if (switchState == HIGH) {
        //turn LED on:
        digitalWrite(ledPin, HIGH);
        Serial.println("switch high!");
    }
    else {
        //turn LED off:
        digitalWrite(ledPin, LOW);
        Serial.println("switch low");
    }
}

```

- **Bước 2.** Khi chúng ta chuyển sang mức cao và đèn LED sẽ sáng. Chúng ta cũng có thể thấy đầu ra nối tiếp như dưới đây.

```
switch high!
switch high!
switch high!
```

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Switch P |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/SwitchP_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-Switch(P)-p-1252.html)|


- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Switch tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/Switch_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ và độ ẩm với **bất kỳ Cổng GPIO nào** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


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
python grove_switch.py 12

```

Đây là code grove_switch.py.

```python


import time
from grove.gpio import GPIO


class GroveTiltSwitch(GPIO):
    def __init__(self, pin):
        super(GroveTiltSwitch, self).__init__(pin, GPIO.IN)

    @property
    def state(self):
        return super(GroveTiltSwitch, self).read()


Grove = GroveTiltSwitch


def main():
    import sys

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    swicth = GroveTiltSwitch(int(sys.argv[1]))


    while True:
        if swicth.state is 1:
            print("on")
        else:
            print("off")
        time.sleep(1)


if __name__ == '__main__':
    main()


```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_switch.py 12
off
off
on
off
on
on
off
^CTraceback (most recent call last):
  File "grove_switch.py", line 70, in <module>
    main()
  File "grove_switch.py", line 66, in main
    time.sleep(1)
KeyboardInterrupt


```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.



### Đối với Raspberry Pi (với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove-Switch(P) |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/SwitchP_s.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](http://www.seeedstudio.com/Grove-Switch(P)-p-1252.html)|


- **Step 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-Switch(P) tới cỏng **D3** của GrovePi_Plus.
- **Step 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/img/rpi_switch.jpg)

**Phần mềm**

- **Step 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Step 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Step 3.** Thực hiện các lệnh dưới đây để theo dõi trạng thái chuyển đổi.


```python
cd ~/GrovePi/Software/Python
python grove_switch.py
```

Đây là mã grove_switch.py.

```python
import time
import grovepi

# Connect the Grove Switch to digital port D3
# SIG,NC,VCC,GND
switch = 3

grovepi.pinMode(switch,"INPUT")

while True:
    try:
        print(grovepi.digitalRead(switch))
        time.sleep(.5)

    except IOError:
        print ("Error")
```

- **Bước 4.** Chúng ta sẽ thấy trạng thái chuyển đổi như dưới đây.

```python
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_switch.py 
1
1
0
0
0
```

## Nguồn

- **[Eagle&PDF]** [Grove-Switch(P) Schematic](https://github.com/SeeedDocument/Grove-Switch-P/raw/master/res/Grove-Switch-P-Eagle_File_v1.0.zip)

## Dự án

**Sử dụng công tắc để mở và đóng rơle**: Bạn sẽ tìm hiểu giá trị của một công tắc, với chức năng Cao và Thấp. Ngoài ra, bạn sẽ học cách sử dụng rơle làm cơ cấu chấp hành. 

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/sodaqmoja/using-a-switch-to-open-and-close-a-relay-3329ec/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>