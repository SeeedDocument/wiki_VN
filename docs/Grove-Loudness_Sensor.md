---
name: Grove - Loudness Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Loudness-Sensor-p-1382.html
oldwikiname: Grove_-_Loudness_Sensor
prodimagename: LoudnessSensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/Loudness Sensor.jpg
surveyurl: https://www.research.net/r/Grove-Loudness_Sensor
sku: 101020063
tags: grove_analog, io_3v3, io_5v, plat_duino, plat_linkit, plat_bbg, plat_pi
---

![](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/Loudness%20Sensor_new.jpg)

Grove - Loudness Sensor được thiết kế để phát hiện âm thanh của môi trường. Dựa trên bộ khuếch đại LM2904 và micrô tích hợp, nó khuếch đại và lọc tín hiệu tần số cao nhận được từ micrô và phát ra một bao phủ dương. Điều này được sử dụng để thu thập tín hiệu Arduino. Giá trị đầu ra phụ thuộc vào mức độ đầu vào âm thanh. Để tránh nhiễu tín hiệu không cần thiết, tín hiệu đầu vào sẽ trải qua hai lần lọc bên trong module. Có một chiết áp vít cho phép điều chỉnh thủ công để đạt được đầu ra.
<iframe width="800" height="450" src="https://www.youtube.com/embed/EhZ7uDvoALE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p style=":center"><a href="http://www.seeedstudio.com/Grove-Loudness-Sensor-p-1382.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

## Phiên bản

| Phiên bản sản phẩm              | Thay đổi                                   | Ngày phát hành |
|------------------------------|-------------------------------------------|---------------|
|Grove-Loudness Sensor V0.9b   | Ban đầu                                   | 12/ 2012      |     


## Đặc điểm

-   Giao diện Grove
-   Dễ sử dụng
-   Yếu tố Grove cơ bản

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật

| Tham số             | Giá trị            |
|-----------------------|------------------------|
| Điện áp               | 3.5~10 VDC             |
| Tần số hoạt động     | 50~2000 Hz             |
| Độ nhạy           | -48~66 dB              |
| Tỷ lệ tín hiệu trên tạp âm | >58 dB                 |
| Phạm vi tín hiệu đầu ra   | Tín hiệu tương tự (0-1023) |


## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove-Loudness Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/LoudnessSensor_s.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Loudness-Sensor-p-1382.html)|

- **Bước 2.** Kết nối Grove-Loudness Sensor tới cổng **A0** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/seeeduino_loudness.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield,chúng tôi cũng có thể kết nối trực tiếp Grove-Loudness Sensor tới Seeeduino như dưới đây.

| Seeeduino |  Grove-Loudness Sensor |
|-----------|-----------------|
| 5V        | Đỏ             |
| GND       | Đen           |
| NC        | Trắng           |
| A0        | Vàng          | 

**Phần mềm**

- **Bước 1.** Vui lòng sao chép mã dưới đây vào Arduino IDE và tải lên arduino. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).


```
int loudness;

void setup()
{
    Serial.begin(9600);
}

void loop()
{
    loudness = analogRead(0);
    Serial.println(loudness);
    delay(200);
}

```

- **Bước 2.** Mở serial để theo dõi đầu ra. Nó sẽ là một thay đổi đáng kể khi thổi vào cảm biến.

![](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/seeeduino_serial.png)



### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi | Grove - Loudness Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/LoudnessSensor_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Loudness-Sensor-p-1382.html)

- **Bước 2**. Cắm Grove Base Hat vào Raspberry Pi.
- **Bước 3**. Kết nối Grove - Loudness Sensor tới cổng A0 của the Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.
![](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/withrpi_basehat.jpg)


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. s 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_loudness_sensor.py 0
```


Dưới đây là mã grove_water_sensor.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveLoudnessSensor:

    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()

    @property
    def value(self):
        return self.adc.read(self.channel)

Grove = GroveLoudnessSensor


def main():
    if len(sys.argv) < 2:
        print('Usage: {} adc_channel'.format(sys.argv[0]))
        sys.exit(1)

    sensor = GroveLoudnessSensor(int(sys.argv[1]))

    print('Detecting loud...')
    while True:
        value = sensor.value
        if value > 10:
            print("Loud value {}, Loud Detected.".format(value))
            time.sleep(.5)

if __name__ == '__main__':
    main()


```
!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau:
```python

pi@raspberrypi:~/grove.py/grove $ python grove_loudness_sensor.py 0
Detecting loud...
Loud value 15, Loud Detected.
Loud value 11, Loud Detected.
Loud value 250, Loud Detected.
Loud value 429, Loud Detected.
Loud value 203, Loud Detected.
Loud value 16, Loud Detected.
Loud value 11, Loud Detected.
^CTraceback (most recent call last):
  File "grove_loudness_sensor.py", line 68, in <module>
    main()
  File "grove_loudness_sensor.py", line 65, in main
    time.sleep(.5)
KeyboardInterrupt


```

Bạn có thể sử dụng cảm biến này để phát hiện tiếng ồn. Ấn ++ctrl+c++ để thoát.

!!!Để ý
    Bạn có thể nhận thấy rằng đối với cổng analog, số pin màn hình có dạng như **A0, A1**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm mô-đun vào đúng cổng, nếu không có thể có xung đột pin.


### Đối với Raspberry Pi (với GrovePi_Plus)

**Phần cứng**

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove-Loudness Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/LoudnessSensor_s.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](http://www.seeedstudio.com/Grove-Loudness-Sensor-p-1382.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Loudness Sensor tới cổng **A0** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/img/rpi_loudness.jpg)

**Phần mềm**

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Bước 3.** Thực hiện các lệnh dưới đây để có giám sát tiếng ồn.


```python
cd ~/GrovePi/Software/Python
python grove_loudness_sensor.py
```

Đây là grove_loudness_sensor.py.

```python
import time
import grovepi

# Connect the Grove Loudness Sensor to analog port A0
# SIG,NC,VCC,GND
loudness_sensor = 0

while True:
    try:
        # Read the sound level
        sensor_value = grovepi.analogRead(loudness_sensor)

        print("sensor_value = %d" %sensor_value)
        time.sleep(.5)

    except IOError:
        print ("Error")
```

- **Bước 4.** Chúng ta sẽ thấy trạng thái tiếng ồn như bên dưới.

```python
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_loudness_sensor.py
sensor_value = 135
sensor_value = 23
sensor_value = 196
sensor_value = 258
sensor_value = 98
sensor_value = 131
```

## Các câu hỏi thường gặp

- Hỏi 1: Sự khác biệt giữa Grove-Loudness sensor và Grove - Sound Sensor?
    - Trả lời 1: Grove-Loudness sensor có chiết áp vít để điều chỉnh mức tăng đầu ra.

## Nguồn

- **[Eagle&PDF]** [Grove - Loudness Sensor Schematic](https://github.com/SeeedDocument/Grove-Loudness_Sensor/raw/master/res/Grove%20-%20Loudness%20Sensor%20Eagle%20File_v0.9b.zip)
- **[Datasheet]** [LM2904DR Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Loudness_Sensor/master/res/LM2904DR.pdf)

## Dự án

**Bộ giám sát môi trường năng lượng mặt trời**: Một bộ nguồn mở sử dụng năng lượng mặt trời để theo dõi chất lượng không khí, mức âm thanh, độ ẩm và nhiệt độ.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/taifur/solar-powered-environmental-monitoring-kit-b1d03d/embed' width='350'></iframe>

**Mật mã Da Vinci**: Công việc kết hợp nghệ thuật và điện tử. Phần nghệ thuật tạo nên bộ xương và bao gồm 11 lớp ván sợi mật độ trung bình.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/coding-with-da-vince/the-da-vinci-code-3b91a8/embed' width='350'></iframe>


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>