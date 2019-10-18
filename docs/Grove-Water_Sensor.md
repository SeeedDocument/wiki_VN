---
name: Grove - Water Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Water-Sensor-p-748.html
oldwikiname: Grove_-_Water_Sensor
prodimagename: Grove-Water_Sensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020018 1.jpg
surveyurl: https://www.research.net/r/Grove-Water_Sensor
sku: 101020018
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_linkit, plat_pi, plat_bbg
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/Grove-Water_Sensor_1.png)

Module Water Sensor là một phần của hệ thống Grove. Nó cho biết cảm biến khô, ẩm hoặc ngâm hoàn toàn trong nước bằng cách đo độ dẫn. Các dấu vết cảm biến có điện trở kéo lên yếu 1 MΩ. Các điện trở sẽ kéo giá trị theo dõi cảm biến lên cao cho đến khi một giọt nước rút ngắn dấu vết cảm biến đến dấu vết nối đất. Tin hay không mạch này sẽ hoạt động với các chân I/O kỹ thuật số của Arduino hoặc bạn có thể sử dụng nó với các chân tương tự để phát hiện lượng nước tiếp xúc giữa các dấu vết nối đất và cảm biến.

<p style=":center"><a href="https://www.seeedstudio.com/Grove-Water-Sensor-p-748.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>

## Version

| Phiên bản sản phẩm              | Thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Water Sensor V1.1 | Ban đầu                                                                                                                                                                                    | 07/2014      |


## Đặc điểm


- Giao diện tương thích Grove
- Điện năng tiêu thụ thấp
- Module Grove 2.0cm x 2.0cm 
- Độ nhạy cao
## Ý tưởng ứng dụng

- Phát hiện lượng mưa
- Rò rỉ chất lỏng
- Phát hiện tràn bể

## Các thông số kỹ thuật

<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Mục
</th>
<th scope="col">
Nhỏ nhất
</th>
<th scope="col">
Điển hình
</th>
<th scope="col">
Lớn nhất
</th>
<th scope="col">
Đơn vị
</th>
</tr>
<tr align="center">
<th scope="row">
Điện áp hoạt động
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
V
</td>
</tr>
<tr align="center">
<th scope="row">
Dòng điện
</th>
<td colspan="3">
&lt;20
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<th scope="row">
Nhiệt độ hoạt động
</th>
<td>
10
</td>
<td>
-
</td>
<td>
30
</td>
<td>
℃
</td>
</tr>
<tr align="center">
<th scope="row">
Độ ẩm làm việc (không ngưng tụ)
</th>
<td>
10
</td>
<td>
-
</td>
<td>
90
</td>
<td>
 %
</td>
</tr>
</table>

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

### Đối với Arduino

#### Phần cứng

Kết nối module với mạch cơ bản bằng cách sử dụng bất kỳ chân kỹ thuật số nào. Bạn có thể đạt được giá trị của chân tín hiệu. Khi có nước trên dây dẫn trần, giá trị ở mức THẤP. Nếu không, sẽ ở mức CAO.

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Water Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/Grove-Water_Sensor_small.png)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Water-Sensor-p-748.html)|

- **Bước 2.** Kết nối Water Sensor tới cổng D2 của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/3.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove - Water Sensor tới Seeeduino như dưới đây.

| Seeeduino       | Grove - Water Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| D2            | Vàng                  |

#### Phần mềm
- **Bước 1.** Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải mã lên](http://wiki.seeedstudio.com/Upload_Code/).

```c
#define WATER_SENSOR 2

void setup()
{
  Serial.begin (9600);
  pinMode(WATER_SENSOR, INPUT);
}
void loop()
{
  Serial.println(digitalRead(WATER_SENSOR));
  delay(500);
}

```
- **Bước 2.** Chúng ta sẽ thấy màn hình đầu ra trên terminal như dưới đây.

```c
1
1
0
0
1
1
```

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Water Sensor tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/cc_Water_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã hoàn thành được tải lên, bạn sẽ thấy có nước hay không trong Màn hình Nối tiếp.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Water Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/Grove-Water_Sensor_small.png)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Water-Sensor-p-748.html)

- **Bước 2**. Cắm Grove Base Hat vào Raspberry Pi.
- **Bước 3**. Kết nối Grove - Water Sensor tới cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.
![](https://github.com/SeeedDocument/Grove-Water_Sensor/raw/master/img/with_rpi_basehat.jpg)


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py. 

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3.** Thực hiện lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_water_sensor.py 0
```


Tiếp theo là mã grove_water_sensor.py.

```python

import math
import sys
import time
from grove.adc import ADC


class GroveWaterSensor:

    def __init__(self, channel):
        self.channel = channel
        self.adc = ADC()

    @property
    def value(self):
        return self.adc.read(self.channel)

Grove = GroveWaterSensor


def main():
    if len(sys.argv) < 2:
        print('Usage: {} adc_channel'.format(sys.argv[0]))
        sys.exit(1)

    sensor = GroveWaterSensor(int(sys.argv[1]))

    print('Detecting ...') 
    while True:
        value = sensor.value        
        if sensor.value > 800:
            print("{}, Detected Water.".format(value))
        else:
            print("{}, Dry.".format(value))

        time.sleep(.1)

if __name__ == '__main__':
    main()


```


!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
```python

pi@raspberrypi:~/grove.py/grove $ python grove_water_sensor.py 0
Detecting ...
612, Dry.
749, Detected Water.
829, Dry.
357, Dry.
98, Dry.
352, Dry.
517, Dry.
718, Detected Water.
868, Detected Water.
581, Dry.
90, Dry.
326, Dry.
451, Dry.
666, Dry.
867, Detected Water.
684, Dry.
100, Dry.
^CTraceback (most recent call last):
  File "grove_water_sensor.py", line 71, in <module>
    main()
  File "grove_water_sensor.py", line 62, in main
    value = sensor.value        
  File "grove_water_sensor.py", line 48, in value
    return self.adc.read(self.channel)
  File "/usr/local/lib/python2.7/dist-packages/grove/adc.py", line 66, in read
    return self.read_register(addr)
  File "/usr/local/lib/python2.7/dist-packages/grove/adc.py", line 84, in read_register
    return self.bus.read_word_data(self.address, n)
  File "/home/pi/.local/lib/python2.7/site-packages/smbus2/smbus2.py", line 396, in read_word_data
    ioctl(self.fd, I2C_SMBUS, msg)
KeyboardInterrupt


```

Bạn có thể sử dụng cảm biến này để phát hiện nước. Nhấn ++ ctrl + c ++ để thoát.


!!!Khuyến cáo
        Bạn có thể nhận thấy rằng đối với cổng tương tự, số chân màn hình có dạng như ** A1, A0 **, tuy nhiên trong lệnh chúng tôi sử dụng tham số ** 0 ** và ** 1 **, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm module vào đúng cổng, nếu không có thể có xung đột chân.


### Đối với Raspberry Pi(với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Water Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/Grove-Water_Sensor_small.png)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Water-Sensor-p-748.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove-Water Sensor tới cổng **D2** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/img/7.jpg)
#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Chuyển đến thư mục các bản demo:

```
cd yourpath/GrovePi/Software/Python/
```

-	**Bước 3.** Để xem code

```
nano grove_water_sensor.py
```

```python
import time
import grovepi

# Connect the Grove Water Sensor to digital port D2
# SIG,NC,VCC,GND
water_sensor = 2

grovepi.pinMode(water_sensor,"INPUT")

while True:
    try:
        print grovepi.digitalRead(water_sensor)
        time.sleep(.5)

    except IOError:
        print "Error"
```

-	**Bước 4.** Chạy demo.

```
sudo python grove_water_sensor.py
```

- **Bước 5.** Chúng ta sẽ thấy màn hình hiển thị trên terminal như hình dưới.

```
1
1
0
0
1
```

## Nguồn

- **[Eagle]** [Grove Water Sensor Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/res/Water_sensor.zip)
- **[Library]** [Demo code for Grove Water Sensor](https://github.com/Seeed-Studio/Grove_Water_Sensor)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Water_Sensor/master/res/Grove_Water_Sensor_CDC_File.zip)

<!-- This Markdown file was created from http://wiki.seeedstudio.com/Grove-Water_Sensor/ -->

## Dự án 

**Cây trồng thông minh: Triển khai IoT trong nông nghiệp thông thường!**:Nhiệm vụ của chúng tôi với thiên nhiên là bảo quản nó, thiết kế và thực hiện các công nghệ và phương pháp giám sát với sự trợ giúp của IoT thông qua Helium.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/gabogiraldo/smart-crops-implementing-iot-in-conventional-agriculture-3674a6/embed' width='350'></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>