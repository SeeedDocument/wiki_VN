---
name: Grove - Temperature&Humidity Sensor
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Temp&Humi-Sensor-p-745.html
oldwikiname: Grove_-_Temperature&Humidity_Sensor
prodimagename: Grove-TempAndHumiSensor.jpg
bzprodimageurl: https://statics3.seeedstudio.com/images/101020011 1.jpg
surveyurl: https://www.research.net/r/Grove-TemperatureAndHumidity_Sensor
sku: 101020011
---

![](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/main.jpg)

Cảm biến Nhiệt độ & Độ ẩm này cung cấp đầu ra số được hiệu chuẩn trước. Một phần tử cảm biến điện dung duy nhất đo độ ẩm tương đối và nhiệt độ được đo bằng nhiệt điện trở hệ số âm (NTC). Nó có độ tin cậy tuyệt vời và ổn định lâu dài. Xin lưu ý rằng cảm biến này sẽ không hoạt động ở nhiệt độ dưới 0 độ.


<p style=":center"><a href="https://www.seeedstudio.com/Grove-Temperature-Humidity-Sensor-DHT1-p-745.html" target="_blank"><img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/get_one_now_small.png" width="210" height="41"  border=0 /></a></p>



## Đặc tính
--------

-   Đo độ ẩm và nhiệt độ tương đối
-   Bù nhiệt độ toàn dải Hiệu chuẩn
-   Tín hiệu kĩ thuật số
-   Sự ổn định lâu dài
-   Khoảng cách truyền dài (> 20m)
-   Sự tiêu thụ ít điện năng

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Ý tưởng ứng dụng
------------------

-   Sản phẩm tiêu thụ
-   Trạm thời tiết
-   Điều chỉnh độ ẩm
-   Điều hòa


## Các thông số kỹ thuật
--------------

### Thông số kỹ thuật chính

| Items        |   Min                  |
|--------------|------------------------|
| Kích thước PCB     | 2.0cm*4.0cm            |
| Giao diện    | 2.0mm pitch pin header |
| Cấu trúc IO | SIG,VCC,GND,NC         |
| ROHS         | YES                    |

### Đặc tính điện tử

<table border="1">
<tr>
<th>
Items
</th>
<th>
Điều kiện
</th>
<th>
Min
</th>
<th>
Thông thường
</th>
<th>
Max
</th>
<th>
Đơn vị
</th>
</tr>
<tr align="center">
<td>
VCC
</td>
<td>
-
</td>
<td>
3.3
</td>
<td>
-
</td>
<td>
5
</td>
<td>
Volts
</td>
</tr>
<tr align="center">
<td>
Đo dòng cung cấp
</td>
<td>
-
</td>
<td>
1.3 
</td>
<td>
- 
</td>
<td>
2.1
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<td>
Dòng cung cấp trung bình
</td>
<td>
-
</td>
<td>
0.5
</td>
<td>
-
</td>
<td>
1.1
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<td rowspan="2">
Dải đo
</td>
<td>
Độ ẩm
</td>
<td>
20%
</td>
<td>
-
</td>
<td>
90%
</td>
<td>
RH
</td>
</tr>
<tr align="center">
<td>
Nhiệt độ
</td>
<td>
0
</td>
<td>
-
</td>
<td>
50
</td>
<td>
°C
</td>
</tr>
<tr align="center">
<td rowspan="2">
Độ chính xác
</td>
<td>
Độ ẩm
</td>
<td>
-
</td>
<td>
-
</td>
<td>
±5%
</td>
<td>
RH
</td>
</tr>
<tr align="center">
<td>
Nhiệt độ
</td>
<td>
</td>
<td>
</td>
<td>
±2
</td>
<td>
°C
</td>
</tr>
<tr align="center">
<td rowspan="2">
Độ nhạy
</td>
<td>
Độ ẩm
</td>
<td>
</td>
<td>
-
</td>
<td>
1%
</td>
<td>
RH
</td>
</tr>
<tr align="center">
<td>
Nhiệt độ
</td>
<td>
</td>
<td>
</td>
<td>
1
</td>
<td>
°C
</td>
</tr>
<tr align="center">
<td rowspan="2">
Độ lặp lại
</td>
<td>
Độ ẩm
</td>
<td>
</td>
<td>
</td>
<td>
±1%
</td>
<td>
RH
</td>
</tr>
<tr align="center">
<td>
Nhiệt độ
</td>
<td>
</td>
<td>
</td>
<td>
±1
</td>
<td>
°C
</td>
</tr>
<tr align="center">
<td>
Sự ổn định lâu dài
</td>
<td>
</td>
<td>
</td>
<td>
</td>
<td>
±1%
</td>
<td>
RH/năm
</td>
</tr>
<tr align="center">
<td>
Thời kỳ thu thập tín hiệu
</td>
<td>
</td>
<td>
</td>
<td>
2
</td>
<td>
</td>
<td>
S
</td>
</tr>
</table>



Các nền tảng được hỗ trợ
------------------

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.



Bắt đầu

Khi MCU gửi tín hiệu kích hoạt, cảm biến sẽ thay đổi từ chế độ tiêu thụ điện năng thấp sang chế độ hoạt động. Sau khi cảm biến tín hiệu kích hoạt sẽ gửi tín hiệu phản hồi trở lại MCU, sau đó dữ liệu được thu thập 40 bit được gửi đi và việc thu thập tín hiệu mới được chuyển đi (Lưu ý rằng dữ liệu thu thập 40 bit được gửi từ cảm biến đến MCU đã được thu thập trước khi tín hiệu kích hoạt xuất hiện.) Một tín hiệu kích hoạt nhận dữ liệu phản hồi 40 bit một lần từ cảm biến. Dữ liệu một bus được sử dụng để liên lạc giữa MCU và cảm biến.
Quá trình giao tiếp được hiển thị dưới đây:

![](https://raw.githubusercontent.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/master/img/Twig-Temperature_Humidity.jpg)

Nó tốn 5ms cho giao tiếp một lần. Bit dữ liệu bậc cao gửi ra trước. Dữ liệu tín hiệu là 40 bit, bao gồm dữ liệu độ ẩm 16 bit, dữ liệu nhiệt độ 16 bit và tổng kiểm tra 8 bit. Định dạng dữ liệu là:

    8bits integer part of humidity+8bits decimal part of humidity
    +8bits integer part of temperature+8bits decimal part of temperature
    +8bits checksum.

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


### Đối với Arduino

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Temperature&Humidity Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/list.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Temp%26Humi-Sensor-p-745.html)|


- **Bước 2.** Kết nối cảm biến Grove - Nhiệt độ & Độ ẩm tới cổng **D2** của Grove-Base Shield.

- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/connect_arduino.jpg)


!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove - Temperature and Humidity Sensor Pro tới Seeeduino như dưới đây.


| Seeeduino       | Temperature&Humidity Sensor |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D2            | Vàng                  |


#### Phần mềm

- **Bước 1.** Tải xuống  [ Thư viện Seeed DHT](https://github.com/Seeed-Studio/Grove_Temperature_And_Humidity_Sensor)  từ Github.

- **Bước 2.** Tham khảo [How to install library](http://wiki.seeedstudio.com/How_to_install_Arduino_Library) để cài đặt thư viện cho Arduino.

- **Bước 3.** Khởi động lại Arduino IDE. Mở ví dụ về DHTtester qua đường dẫn: **File --> Examples --> Grove_Humidity_Temperature_Sensor-master --> DHTtester**. Thông qua bản demo này, chúng ta có thể đọc thông tin về nhiệt độ và độ ẩm tương đối của môi trường.

![](https://github.com/SeeedDocument/Grove-Temperature_and_Humidity_Sensor_Pro/raw/master/img/path.png)


!!!Chú ý
    Grove - Temperature&Humidity Sensor và một sản phẩm khác của chúng tôi  [ Grove-Temperature&Humidity Sensor pro](http://wiki.seeedstudio.com/Grove-Temperature_and_Humidity_Sensor_Pro/) đang chia sẻ thư viện này. Cho dù bạn đang sử dụng sản phẩm nào, hãy đảm bảo rằng bạn đã làm cho dòng định nghĩa của cảm biến của bảng của bạn có hiệu lực và nhận xét các dòng định nghĩa của thông số kỹ thuật khác. Ví dụ: cảm biến chúng tôi sử dụng trên Grove - Cảm biến nhiệt độ và độ ẩm là DHT 11. Vì vậy, phần định nghĩa của thông số cảm biến phải là:

```
#define DHTTYPE DHT11   // DHT 11
//#define DHTTYPE DHT22   // DHT 22  (AM2302)
//#define DHTTYPE DHT21   // DHT 21 (AM2301)
```

Cài đặt mặc định của thư viện là `DHT 22`, vì vậy bạn cần thay đổi nó thành `DHT 11` bằng tay.


- **Bước 4.** Tải lên bản demo. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra[ how to upload code](http://wiki.seeedstudio.com/Upload_Code/).



- **Bước 5.** Mở **Serial Monitor** của Arduino IDE bằng cách nhấn **Tool-> Serial Monitor**. Hoặc nhấn phím ++ ctrl + shift + m ++ cùng một lúc. Nếu mọi thứ suôn sẻ, bạn sẽ nhận được nhiệt độ.

Kết quả sẽ như sau:

![](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/result_ar.png)

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Temperature&Humidity Sensor tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/master/img/cc_Temperature_Humidity.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy nhiệt độ và độ ẩm được hiển thị trên Màn hình Nối tiếp.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Temp & Hum Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/list.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Temp%26Humi-Sensor-p-745.html)|


- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối cảm biến nhiệt độ và độ ẩm tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.


![](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/Temp_Hum_Hat.jpg)


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
python grove_temperature_humidity_sensor.py 11 12

```

!!!Chú ý
    1.  Để chạy chương trình này, dòng lệnh phải là +++python grove_temperature_humidity_sensor.py DHT type pin+++. Đối với module này, loại DHT là 11 và chúng tôi đã kết nối cảm biến nhiệt độ và độ ẩm với pin 12 trong trường hợp trên.
    2. Grove - Temperature&Humidity Sensor này và sản phẩm khác của chúng tôi [Grove-Temperature and Humidity Sensor Pro](http://wiki.seeedstudio.com/Grove-Temperature_and_Humidity_Sensor_Pro/) đang chia sẻ cùng mã python có tên 'grove_temperature_humidity_sensor.py'. Sự khác biệt duy nhất là loại DHT là 22 cho Temperature &Humidity Sensor Pro và 11 cho Temperature & Humidity Sensor.

Dưới đây là mã grove_temperature_humidity_sensor.py.

```python

import RPi.GPIO as GPIO
# from grove.helper import *
def set_max_priority(): pass
def set_default_priority(): pass
from time import sleep

GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)

PULSES_CNT = 41

class DHT(object):
    DHT_TYPE = {
        'DHT11': '11',
        'DHT22': '22'
    }

    MAX_CNT = 320

    def __init__(self, dht_type, pin):        
        self.pin = pin
        if dht_type != self.DHT_TYPE['DHT11'] and dht_type != self.DHT_TYPE['DHT22']:
            print('ERROR: Please use 11|22 as dht type.')
            exit(1)
        self._dht_type = '11'
        self.dht_type = dht_type
        GPIO.setup(self.pin, GPIO.OUT)

    @property
    def dht_type(self):
        return self._dht_type

    @dht_type.setter
    def dht_type(self, type):
        self._dht_type = type
        self._last_temp = 0.0
        self._last_humi = 0.0

    def _read(self):
        # Send Falling signal to trigger sensor output data
        # Wait for 20ms to collect 42 bytes data
        GPIO.setup(self.pin, GPIO.OUT)
        set_max_priority()

        GPIO.output(self.pin, 1)
        sleep(.2)

        GPIO.output(self.pin, 0)
        sleep(.018)

        GPIO.setup(self.pin, GPIO.IN)
        # a short delay needed
        for i in range(10):
            pass

        # pullup by host 20-40 us
        count = 0
        while GPIO.input(self.pin):
            count += 1
            if count > self.MAX_CNT:
                # print("pullup by host 20-40us failed")
                set_default_priority()
                return None, "pullup by host 20-40us failed"

        pulse_cnt = [0] * (2 * PULSES_CNT)
        fix_crc = False
        for i in range(0, PULSES_CNT * 2, 2):
            while not GPIO.input(self.pin):
                pulse_cnt[i] += 1
                if pulse_cnt[i] > self.MAX_CNT:
                    # print("pulldown by DHT timeout %d" % i)
                    set_default_priority()
                    return None, "pulldown by DHT timeout %d" % i

            while GPIO.input(self.pin):
                pulse_cnt[i + 1] += 1
                if pulse_cnt[i + 1] > self.MAX_CNT:
                    # print("pullup by DHT timeout %d" % (i + 1))
                    if i == (PULSES_CNT - 1) * 2:
                        # fix_crc = True
                        # break
                        pass
                    set_default_priority()
                    return None, "pullup by DHT timeout %d" % i

        # back to normal priority
        set_default_priority()

        total_cnt = 0
        for i in range(2, 2 * PULSES_CNT, 2):
            total_cnt += pulse_cnt[i]

        # Low level ( 50 us) average counter
        average_cnt = total_cnt / (PULSES_CNT - 1)
        # print("low level average loop = %d" % average_cnt)
       
        data = ''
        for i in range(3, 2 * PULSES_CNT, 2):
            if pulse_cnt[i] > average_cnt:
                data += '1'
            else:
                data += '0'
        
        data0 = int(data[ 0: 8], 2)
        data1 = int(data[ 8:16], 2)
        data2 = int(data[16:24], 2)
        data3 = int(data[24:32], 2)
        data4 = int(data[32:40], 2)

        if fix_crc and data4 != ((data0 + data1 + data2 + data3) & 0xFF):
            data4 = data4 ^ 0x01
            data = data[0: PULSES_CNT - 2] + ('1' if data4 & 0x01 else '0')

        if data4 == ((data0 + data1 + data2 + data3) & 0xFF):
            if self._dht_type == self.DHT_TYPE['DHT11']:
                humi = int(data0)
                temp = int(data2)
            elif self._dht_type == self.DHT_TYPE['DHT22']:
                humi = float(int(data[ 0:16], 2)*0.1)
                temp = float(int(data[17:32], 2)*0.2*(0.5-int(data[16], 2)))
        else:
            # print("checksum error!")
            return None, "checksum error!"

        return humi, temp

    def read(self, retries = 15):
        for i in range(retries):
            humi, temp = self._read()
            if not humi is None:
                break
        if humi is None:
            return self._last_humi, self._last_temp
        self._last_humi,self._last_temp = humi, temp
        return humi, temp

Grove = DHT


def main():
    import sys
    import time

    if len(sys.argv) < 3:
        print('Usage: {} dht_type pin'.format(sys.argv[0]))
        sys.exit(1)

    typ = sys.argv[1]
    sensor = DHT(typ, int(sys.argv[2]))
    
    while True:
        humi, temp = sensor.read()
        if not humi is None:
            print('DHT{0}, humidity {1:.1f}%, temperature {2:.1f}*'.format(sensor.dht_type, humi, temp))
        else:
            print('DHT{0}, humidity & temperature: {1}'.format(sensor.dht_type, temp))
        time.sleep(1)


if __name__ == '__main__':
    main()



```

!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy kết quả sau.
    
```python

pi@raspberrypi:~/grove.py/grove $ python grove_temperature_humidity_sensor.py 11 12
DHT11, humidity 31.0%, temperature 22.0*
DHT11, humidity 30.0%, temperature 23.0*
DHT11, humidity 29.0%, temperature 23.0*
^CTraceback (most recent call last):
  File "grove_temperature_humidity_sensor.py", line 192, in <module>
    main()
  File "grove_temperature_humidity_sensor.py", line 188, in main
    time.sleep(1)
KeyboardInterrupt


```


Bạn có thể thoát chương trình này đơn giản bằng cách nhấn ++ ctrl + c ++.



### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng


- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Temperature&Humidity Sensor|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/list.jpg)|
|[Get One Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get One Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Temperature%26Humidity-Sensor-Pro-p-838.html)|


- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.

- **Bước 3.** Kết nối Grove - Temperature&Humidity Sensor tới cổng **D4** của GrovePi_Plus.

- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/raw/master/img/connect_pi.jpg)


#### Phần mềm
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

-	**Bước 4.** Kiểm tra code.

```python

cd ~/GrovePi/Software/Python
sudo nano grove_dht_pro.py

```

Mã nên như sau:
```python
import grovepi
import math
# Connect the Grove Temperature & Humidity Sensor Pro to digital port D4
# This example uses the blue colored sensor.
# SIG,NC,VCC,GND
sensor = 4  # The Sensor goes on digital port 4.

# temp_humidity_sensor_type
# Grove Base Kit comes with the blue sensor.
blue = 0    # The Blue colored sensor.
white = 1   # The White colored sensor.

while True:
    try:
        # This example uses the blue colored sensor.
        # The first parameter is the port, the second parameter is the type of sensor.
        [temp,humidity] = grovepi.dht(sensor,blue)  
        if math.isnan(temp) == False and math.isnan(humidity) == False:
            print("temp = %.02f C humidity =%.02f%%"%(temp, humidity))

    except IOError:
        print ("Error")

```

Sau đó nhấn ++ ctrl + x ++ để thoát nano.

!!!Chú ý
    Grove - Temperature&Humidity Sensor và Grove - Temperature&Humidity Sensor pro chia sẻ cùng mã python có tên
    `grove_dht_pro.py`.  Sự khác biệt duy nhất là cho câu `[temp,humidity] = grovepi.dht(sensor,blue)`. Chúng tôi sử dụng tham số
    `blue` cho Grove - Temperature&Humidity Sensor trong khi chúng ta sử dụng `white` cho Grove - Temperature&Humidity Sensor pro. Giá trị mặc định là màu xanh, vì vậy đối với cảm biến này, bạn không cần thay đổi mã.

-	**Bước 5.** Thực hiện các lệnh dưới đây để có được giá trị.

```
sudo python grove_dht_pro.py
```

Kết quả sẽ như sau:

```python

pi@raspberrypi:~/GrovePi/Software/Python $ sudo python grove_dht_pro.py
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%
temp = 26.00 C humidity =40.00%

```



## Nguồn


- **[Zip]** [Temperature&Humidity Sensor eagle file](https://raw.githubusercontent.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/master/res/Temperature_Humidity.zip)

- **[Zip]** [Temperature&Humidity Sensor Library](https://github.com/Seeed-Studio/Grove_Temperature_And_Humidity_Sensor)

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-TemperatureAndHumidity_Sensor/master/res/Grove_Temperature_and_Humidity_Sensor_CDC_File.zip)


## Dự án

**Hệ thống quản lý nhà vệ sinh**: Sử dụng hệ thống nhiều người có thể chia sẻ một nhà vệ sinh một cách hiệu quả.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://project.seeedstudio.com/taifur/toilet-management-system-8e2786/embed' width='350'></iframe>


## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi.
<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>