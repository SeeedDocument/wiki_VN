---
name: Grove - Temperature Sensor V1.2
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Temperature-Sensor-p-774.html
oldwikiname: Grove - Temperature Sensor V1.2
prodimagename: Grove_Temperature_Sensor_View.jpg
surveyurl: https://www.surveymonkey.com/r/Grove-Temperature_Sensor_V1-2
sku: 101020015
tags: io_3v3, io_5v, plat_duino
---


<p style=":center"><img src="https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_View.jpg" ></p>




Grove - Temperature Sensor sử dụng [Thermistor](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/res/NCP18WF104F03RC.pdf) để phát hiện nhiệt độ môi trường. Điện trở của nhiệt điện trở sẽ tăng khi nhiệt độ môi trường giảm. Đây là đặc điểm mà chúng tôi sử dụng để tính toán nhiệt độ môi trường. Phạm vi có thể phát hiện của cảm biến này là -40 - 125ºC và độ chính xác là ± 1.5ºC

Lưu ý: wiki này cũng hoạt động với Grove - Temperature sensor V1.1, đối với V1.0 vui lòng tham khảo [Grove - Temperature Sensor](http://wiki.seeedstudio.com/Grove-Temperature_Sensor)



<p style=":center"><a href="https://www.seeedstudio.com/Grove-Temperature-Sensor-p-774.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>



## Các thông số kỹ thuật
---
- Điện áp: 3.3 ~ 5V
- Điện trở zero: 100 KΩ
- Sức đề kháng: ±1%
- Nhiệt độ hoạt động: -40 ~ +125 ℃
- Danh nghĩa B-Constant： 4250 ~ 4299K

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)


## Các nền tảng được hỗ trợ
-------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started
---
Sau phần này, bạn có thể thực hiện Grove - Temperature Sensor V1.1/1.2 chỉ với vài bước.

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Temperature Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_View_little.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Temperature-Sensor-p-774.html)|

- **Step 2.** Kết nối Grove - Temperature Sensor tới cổng **A0** của Grove-Base Shield.

- **Step 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Step 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/connect_Arduino.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove_Temperature Sensor tới Seeeduino như dưới đây.

| Seeeduino       | Grove - Temperature Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| A0            | Vàng                  |



#### Phần mềm

- **Bước 1.** Khởi chạy Arduino IDE và nhấp **File>New** để mở một trang mới. Sao chép mã sau vào trang mới và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [How to upload code](http://wiki.seeedstudio.com/Upload_Code/).


```
// Demo code for Grove - Temperature Sensor V1.1/1.2
// Loovee @ 2015-8-26

#include <math.h>

const int B = 4275;               // B value of the thermistor
const int R0 = 100000;            // R0 = 100k
const int pinTempSensor = A0;     // Grove - Temperature Sensor connect to A0

void setup()
{
    Serial.begin(9600);
}

void loop()
{
    int a = analogRead(pinTempSensor);

    float R = 1023.0/a-1.0;
    R = R0*R;

    float temperature = 1.0/(log(R/R0)/B+1/298.15)-273.15; // convert to temperature via datasheet

    Serial.print("temperature = ");
    Serial.println(temperature);

    delay(100);
}
```

**Bước 2.** Mở **Serial Monitor** của Arduino IDE bằng cách click **Tool-> Serial Monitor**. Hoặc ấn ++ctrl+shift+m++ cùng một lúc. Nếu mọi thứ suôn sẻ, bạn sẽ nhận được nhiệt độ.


Kết quả sẽ như sau:

![](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_result.jpg)



### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Chuẩn bị những thứ dưới đây:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Temperature Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_View_little.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Temperature-Sensor-p-774.html)|


- **Bước 2**. Cắm GrovePi_Plus vào Raspberry.
- **Bước 3**. Kết nối temperature sensor tới cổng A0 của Base Hat.
- **Bước 4**. Kết nối Raspberry tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Temperature_Hat.jpg)


!!! Chú ý
    Đối với bước 3, bạn có thể kết nối cảm biến nhiệt độ với **bất kỳ Cổng tương tự** nhưng đảm bảo bạn thay đổi lệnh với số cổng tương ứng.


#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py.

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_temperature_sensor.py 0

```

Đây là code grove_temperature_sensor.py.

```python

import sys
import time
from grove.factory import Factory


def main():
    from grove.helper import SlotHelper
    sh = SlotHelper(SlotHelper.ADC)
    pin = sh.argv2pin()

    sensor = Factory.getTemper("NTC-ADC", pin)

    print('Detecting temperature...')
    while True:
        print('{} Celsius'.format(sensor.temperature))
        time.sleep(1)


if __name__ == '__main__':
    main()

```

!!!Kết quả
    Nếu thành công, bạn có thể thấy kết quả sau:
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_temperature_sensor.py 0
Hat Name = 'Grove Base Hat RPi'
Detecting temperature...
24.7473402633 Celsius
24.7473402633 Celsius
24.7473402633 Celsius
24.7112751977 Celsius
24.7112751977 Celsius
^CTraceback (most recent call last):
  File "grove_temperature_sensor.py", line 53, in <module>
    main()
  File "grove_temperature_sensor.py", line 49, in main
    time.sleep(1)
KeyboardInterrupt

```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.

!!!Chú ý
        Bạn có thể nhận thấy rằng đối với cổng analog, số chân màn hình có dạng như **A1, A0**, tuy nhiên trong lệnh chúng tôi sử dụng tham số **0** và **1**, giống như cổng kỹ thuật số . Vì vậy, hãy chắc chắn rằng bạn cắm module vào đúng cổng, nếu không có thể có xung đột chân.


### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Temperature Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_View_little.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Temperature-Sensor-p-774.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.

- **Bước 3.** Kết nối Grove - Temperature Sensor ranger tới cổng **A0** của GrovePi_Plus.

- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/connect_pi.jpg)



#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.

- **Bước 2.** Theo dõi  [Updating the Firmware](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/updating-firmware/) để cập nhật firmware mới nhất của GrovePi.

!!!Mẹo
    Trong wiki này, chúng tôi sử dụng đường dẫn **~/GrovePi/** thay vì **/home/pi/Desktop/GrovePi**, bạn cần đảm bảo Bước 2 và Bước 3 sử dụng cùng một đường dẫn.

!!!Chú ý
    Chúng tôi đề nghị bạn cập nhật firmware hoặc đối với một số cảm biến bạn có thể gặp lỗi.

- **Bước 3.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

-	**Bước 4.** Thực hiện các lệnh dưới đây để sử dụng Grove - Temperature Sensor để đo nhiệt độ.

```
cd ~/GrovePi/Software/Python
sudo python grove_temperature_sensor.py
```

Đây là code grove_temperature_sensor.py.

```python

# NOTE:
# 	The sensor uses a thermistor to detect ambient temperature.
# 	The resistance of a thermistor will increase when the ambient temperature decreases.
#
# 	There are 3 revisions 1.0, 1.1 and 1.2, each using a different model thermistor.
# 	Each thermistor datasheet specifies a unique Nominal B-Constant which is used in the calculation forumla.
#
# 	The second argument in the grovepi.temp() method defines which board version you have connected.
# 	Defaults to '1.0'. eg.
# 		temp = grovepi.temp(sensor)        # B value = 3975
# 		temp = grovepi.temp(sensor,'1.1')  # B value = 4250
# 		temp = grovepi.temp(sensor,'1.2')  # B value = 4250

import time
import grovepi

# Connect the Grove Temperature Sensor to analog port A0
# SIG,NC,VCC,GND
sensor = 0

while True:
    try:
        temp = grovepi.temp(sensor,'1.2')
        print("temp =", temp)
        time.sleep(.5)

    except KeyboardInterrupt:
        break
    except IOError:
        print ("Error")

```

Kết quả:

```python

pi@raspberrypi:~/GrovePi/Software/Python $ sudo python grove_temperature_sensor.py

('temp =', 25.28652137917777)
('temp =', 25.28652137917777)
('temp =', 25.28652137917777)
('temp =', 25.28652137917777)
('temp =', 25.368489566400115)
('temp =', 25.61468397498203)
('temp =', 27.43501590142614)
('temp =', 27.85285590636829)
('temp =', 27.18509952680688)
('temp =', 26.852756540240193)

```



## Tài liệu tham khảo
---

Nếu bạn muốn biết thuật toán nhiệt độ sắp tới như thế nào, vui lòng tham khảo hình ảnh dưới đây:

![](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/img/Grove_Temperature_Sensor_Basic_Characteristics.jpg)


## Nguồn
---

- **[Zip]** [Grove - Temperature Sensor v1.1 Eagle File](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/res/Grove_-_Temperature_sensor_v1.1.zip)
- **[PDF]** [Grove - Temperature Sensor v1.1.PDF](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/res/Grove_-_Temperature_sensor_v1.1.pdf)
- **[PDF]** [Temperature Sensor datasheet](https://github.com/SeeedDocument/Grove-Temperature_Sensor_V1.2/raw/master/res/NCP18WF104F03RC.pdf)


## Dự án

**Cảm biến nhiệt độ module Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/wjL7xOGqAqg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/vI9pkmiK8EM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>