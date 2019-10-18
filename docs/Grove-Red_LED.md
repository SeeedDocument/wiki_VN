---
name: Grove - Red LED
category: Display
bzurl: https://www.seeedstudio.com/Grove-Red-LED-p-1142.html
oldwikiname:  Grove - Red LED
prodimagename: Grove-LED_Photo.jpg
surveyurl: https://www.research.net/r/Grove_Red_LedLED
sku:  104030005
---

![](https://github.com/SeeedDocument/Raspi_wiki/raw/master/img/red_led.jpg)

Grove - Red LED tương tự như module Grove - LED chứa nguồn sáng LED. Ngoài ra, nó cũng có một chiết áp trên tàu để quản lý các yêu cầu năng lượng của đèn LED. PCB của module này có các lỗ lắp có thể được gắn trên bề mặt cần thiết của nguyên mẫu của bạn. Ví dụ, nó có thể được sử dụng như một đèn thử nghiệm để biểu thị sự hiện diện của nguồn hoặc tín hiệu.


<p style=":center"><a href="https://www.seeedstudio.com/Grove-Red-LED-p-1142.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>



## Phiên bản


| Phiên bản sản phẩm              | Thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-LED_v1.3 | Ban đầu                                                                                                                                                                                    | 15/03/2016      |

##  Đặc điểm

*   Cung cấp một đèn LED cho dự án của bạn
*   Hỗ trợ các đèn LED màu khác nhau, đèn LED được cắm vào giá đỡ đèn LED thay vì hàn trên bảng
*   Hỗ trợ kiểm soát độ sáng và dải điện áp đầu vào cao hơn với điều chỉnh chiết áp trên bo mạch

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

##  Getting Started


### Đối với Arduino

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Red LED |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/Red%20LED_s.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get ONE Now](https://www.seeedstudio.com/s/Grove-Red-LED-p-1142.html)|

- Bước 2. Kết nối Grove-Red LED tới cổng D2 của Grove-Base Shield.
- Bước 3. Cắm Grove - Base Shield vào Seeeduino.
- Bước 4. Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/seeedstudio_red_led.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Red_Led tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Red Led |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D2            | Vàng                  |

#### Phần mềm

- **Bước 1**. Sao chép mã vào Arduino IDE và tải lên.
```
void setup() {
  // initialize digital pin2  as an output.
  pinMode(2, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(2, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(2, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

- **Bước 2**. Chúng ta sẽ thấy đèn LED bật và tắt.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Red LED tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield tới Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Red_LED/master/img/cc_LED.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy LED nhấp nháy.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove - Red LED |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/Red%20LED_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/s/Grove-Red-LED-p-1142.html)|

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Red LED tới cổng 12 của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.
![](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/BaseHat_LED.jpg)

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
cd yourpath/grove.py/grove
python grove_led.py 12
```
Nếu bạn kết nối đèn LED đỏ với cổng khác của Base Hat, thay vì loại bỏ **python grove_led.py 12**, bạn nên chạy lệnh sau.
```
python grove_led.py portnumber
```

Dưới đây là mã the grove_led.py.

```python

from grove.gpio import GPIO


class GroveLed(GPIO):
    def __init__(self, pin):
        super(GroveLed, self).__init__(pin, GPIO.OUT)

    def on(self):
        self.write(1)

    def off(self):
        self.write(0)


Grove = GroveLed


def main():
    import sys
    import time

    if len(sys.argv) < 2:
        print('Usage: {} pin'.format(sys.argv[0]))
        sys.exit(1)

    led = GroveLed(int(sys.argv[1]))

    while True:
        led.on()
        time.sleep(1)
        led.off()
        time.sleep(1)


if __name__ == '__main__':
    main()


```
!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ thấy LED bật và tắt.

     
!!!Chú ý
     Đối với hầu hết các module Grove, bạn cần thêm tham số số pin, vì trong ví dụ này `python grove_led.py 12`, **12** là chân GPIO được chọn và đầu ra từ chân 12 sẽ cung cấp cho led. 


### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Red Led |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/Red%20LED_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get ONE Now](https://www.seeedstudio.com/s/Grove-Red-LED-p-1142.html)|

- Bước 2. Cắm GrovePi_Plus vào Raspberry.
- Bước 3. Kết nối Grove-Red Led tới cổng D4 của GrovePi_Plus.
- Bước 4. Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/img/rasp_red_led.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Cài đặt phần mềm](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2**. Git nhân bản kho lưu trữ Github.


```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```
- **Bước 3**. Thực hiện lệnh bên dưới.

```
cd ~/GrovePi/Software/Python
python grove_led_blink.py
```

Đây là code grove_led_blink.py.

```python

import time
from grovepi import *

# Connect the Grove LED to digital port D4
led = 4

pinMode(led,"OUTPUT")
time.sleep(1)

print ("This example will blink a Grove LED connected to the GrovePi+ on the port labeled D4. If you're having trouble seeing the LED blink, be sure to check the LED connection and the port number. You may also try reversing the direction of the LED on the sensor.")
print (" ")
print ("Connect the LED to the port labele D4!" )

while True:
    try:
        #Blink the LED
        digitalWrite(led,1)		# Send HIGH to switch on LED
        print ("LED ON!")
        time.sleep(1)

        digitalWrite(led,0)		# Send LOW to switch off LED
        print ("LED OFF!")
        time.sleep(1)

    except KeyboardInterrupt:	# Turn LED off before stopping
        digitalWrite(led,0)
        break
    except IOError:				# Print "Error" if communication error encountered
        print ("Error")
        
```

- **Bước 4**. Chúng ta sẽ thấy led bật và tắt.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_led_blink.py
This example will blink a Grove LED connected to the GrovePi+ on the port labeled D4.
If you're having trouble seeing the LED blink, be sure to check the LED connection and the port number.
You may also try reversing the direction of the LED on the sensor.

Connect the LED to the port labele D4!
LED ON!
LED OFF!
LED ON!
LED OFF!
```


##  Nguồn

* **[PDF]** [Grove-Red LED Schematic](https://github.com/SeeedDocument/Grove-Red_LED/raw/master/res/Grove-LED_v1.3.pdf)
* **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Red_LED/master/res/Grove_Red_LED_CDC_File.zip)

## Dự án

**Sử dụng Grove Button để điều khiển Grove LED**: Cách kết nối và sử dụng Grove Button để điều khiển Grove LED.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/user50338573/using-grove-button-to-control-grove-led-96d00b/embed' width='350'></iframe>

**Các module nút và LED Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/RCtsxwx4OaA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/78lVn_-oYaY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>