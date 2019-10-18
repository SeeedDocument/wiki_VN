---
name: Grove - Button
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Button-p-766.html
oldwikiname: Grove - Button
prodimagename: Button.jpg
surveyurl: https://www.surveymonkey.com/r/grove-button
sku: 101020003
---

![](https://github.com/SeeedDocument/Grove_Button/raw/master/img/Button.jpg)

Grove - Button là một nút ấn tạm thời. Nó chứa một nút "bật / tắt" độc lập. Ngay lập tức có nghĩa là nút bật lại sau khi nó được nhả. Nút này phát ra tín hiệu CAO khi nhấn và THẤP khi nhả. Sig được đánh dấu trên lớp lụa tượng trưng cho tín hiệu trong khi NC không phải là không sử dụng. Có hai phiên bản của nút này có sẵn như trong hình. Sự khác biệt duy nhất là hướng của ổ cắm Grove.

[![](https://github.com/SeeedDocument/Grove_Button/raw/master/image/300px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-Button-p-766.html)

## Phiên bản


| Phiên bản sản phẩm              | Các thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Button | Ban đầu                                                                                                                                                                                    |  25/11/2010      |

## Đặc tính

- Dễ dàng sử dụng nút BẬT / TẮT tạm thời
- Sử dụng Cáp Grove 4 chân tiêu chuẩn

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật

| Tham sô             | Giá trị    |
|-----------------------|----------------|
| Điện áp hoạt động     | 3.3/5V         |
| Vòng đời điện        | 200,000 cycles |
| Lực hoạt động      | 100 ± 50gf     |
| Nhiệt độ hoạt động| -25℃ to +70℃   |
| Kích thước                  | 20mmX20mm      |

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

| Seeeduino V4.2 | Base Shield|  Grove - Button |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Button/raw/master/img/button_s.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Button-p-766.html)|

- Bước 2. Kết nối Grove-Button tới cổng D2 của Grove-Base Shield.
- Bước 3. Cắm Grove - Base Shield vào Seeeduino.
- Bước 4. Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Button/raw/master/img/seeeduino_button.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Button tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Button |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D2            | Vàng                  |

#### Phần mềm

- Bước 1. Sao chép mã vào Arduino IDE và tải lên.

```c
const int buttonPin = 2;     // the number of the pushbutton pin
const int ledPin =  13;      // the number of the LED pin

// variables will change:
int buttonState = 0;         // variable for reading the pushbutton status

void setup() {
    // initialize the LED pin as an output:
    pinMode(ledPin, OUTPUT);
    // initialize the pushbutton pin as an input:
    pinMode(buttonPin, INPUT);
}

void loop(){
    // read the state of the pushbutton value:
    buttonState = digitalRead(buttonPin);

    // check if the pushbutton is pressed.
    // if it is, the buttonState is HIGH:
    if (buttonState == HIGH) {
        // turn LED on:
        digitalWrite(ledPin, HIGH);
    }
    else {
        // turn LED off:
        digitalWrite(ledPin, LOW);
    }
}
```

- Step 2. Chúng ta sẽ thấy đèn LED Pin13 trên và tắt.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Button tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Button/master/img/cc_Button.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã kết thúc được tải lên, đèn LED trên bo mạch Arduino / Seeeduino sẽ sáng khi nhấn nút.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi | Grove - Button |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Button/raw/master/img/button_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Button-p-766.html)

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Step 3**. Kết nối Grove - Button tới cổng PWM (cổng 12) của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.
![](https://github.com/SeeedDocument/Grove_Button/raw/master/img/with_hat.jpg)


#### Phần mềm

- **Bước 1**. Theo dõi [Setting Software](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py.

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_button.py 12
```
Nếu bạn kết nối đèn LED đỏ với cổng khác của Base Hat, thay vì loại bỏ **python grove_led.py 12**, bạn nên chạy lệnh sau.
```
python grove_button.py portnumber
```


Sau đây là mã grove_button.py.

```python

import time
from grove.button import Button
from grove.factory import Factory


class GroveButton(object):
    def __init__(self, pin):
        # High = pressed
        self.__btn = Factory.getButton("GPIO-HIGH", pin)
        self.__last_time = time.time()
        self.__on_press = None
        self.__on_release = None
        self.__btn.on_event(self, GroveButton.__handle_event)

    @property
    def on_press(self):
        return self.__on_press

    @on_press.setter
    def on_press(self, callback):
        if not callable(callback):
            return
        self.__on_press = callback

    @property
    def on_release(self):
        return self.__on_release

    @on_release.setter
    def on_release(self, callback):
        if not callable(callback):
            return
        self.__on_release = callback

    def __handle_event(self, evt):
        dt, self.__last_time = evt["time"] - self.__last_time, evt["time"]
        # print("event index:{} event:{} pressed:{}".format(evt["index"], evt["code"], evt["pressed"]))
        if evt["code"] == Button.EV_LEVEL_CHANGED:
            if evt["pressed"]:
                if callable(self.__on_press):
                    self.__on_press(dt)
            else:
                if callable(self.__on_release):
                    self.__on_release(dt)


Grove = GroveButton

def main():
    from grove.helper import SlotHelper
    sh = SlotHelper(SlotHelper.GPIO)
    pin = sh.argv2pin()

    button = GroveButton(pin)

    def on_press(t):
        print('Button is pressed')
    def on_release(t):
        print("Button is released, pressed for {0} seconds".format(round(t,6)))

    button.on_press = on_press
    button.on_release = on_release

    while True:
        time.sleep(1)


if __name__ == '__main__':
    main()


```


!!!Kết quả
    Nếu mọi thứ suôn sẻ, bạn sẽ có thể thấy kết quả sau:
```python

pi@raspberrypi:~/grove.py/grove $ python grove_button.py 12
Hat Name = 'Grove Base Hat RPi'
Button is pressed
Button is pressed
Button is pressed
Button is pressed
Button is pressed
Button is pressed
Button is released, pressed for 0.002685 seconds
Button is pressed
Button is released, pressed for 0.219019 seconds
Button is pressed
Button is released, pressed for 0.001372 seconds
Button is pressed
Button is pressed
Button is released, pressed for 0.043143 seconds
Button is pressed
Button is released, pressed for 1.083292 seconds
^CTraceback (most recent call last):
  File "grove_button.py", line 103, in <module>
    main()
  File "grove_button.py", line 99, in main
    time.sleep(1)
KeyboardInterrupt


```

Bạn có thể nhấn ++ ctrl + c ++ để thoát khỏi chương trình này.



### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Button |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Button/raw/master/img/button_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Button-p-766.html)|

- Bước 2. Cắm GrovePi_Plus vào Raspberry.
- Bước 3. Kết nối Grove-Button tới cổng D3 của GrovePi_Plus.
- Bước 4. Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Button/raw/master/img/rasp_button.jpg)

#### Phần mềm

- Bước 1. Theo dõi [Setting Software](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- Bước 2. Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```
- Bước 3. Thực hiện các lệnh dưới đây.

```
cd ~/GrovePi/Software/Python
python grove_button.py
```
Đây là mã grove_button.py.

```python
import time
import grovepi

# Connect the Grove Button to digital port D3
# SIG,NC,VCC,GND
button = 3

grovepi.pinMode(button,"INPUT")

while True:
    try:
        print(grovepi.digitalRead(button))
        time.sleep(.5)

    except IOError:
        print ("Error")
```

- Bước 4. Chúng ta sẽ thấy nút bật và tắt.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_button.py
0
1
1
1
1
0
0
```

## Nguồn

- **[Eagle&PDF]** [Grove-Button Eagle Files](https://github.com/SeeedDocument/Grove_Button/raw/master/resources/Grove_-_Button_v1.0_Source_File.zip)

- **[More Reading]** [Wooden Laser Gun](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Button/master/res/Grove_Button_CDC_File.zip)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Button/master/img/gun.jpg)

Lấy cảm hứng từ OVERWATCH, chúng tôi đã tạo ra một đồ chơi Súng Laser bằng gỗ rất thú vị cho vui trong ngày này!

Súng Laser bằng gỗ và Mục tiêu súng đều dựa trên một bảng Arduino có tên là Seeeduino Lotus. Bộ phát laser trên Súng Laser được điều khiển để bắn xung laser để "kích hoạt" Mục tiêu súng. Và có 3 cảm biến ánh sáng trên Gun Target để phát hiện xung laser. Có vẻ rất đơn giản phải không? Nếu bạn quan tâm đến dự án của chúng tôi, hãy làm một cái cho chính bạn hoặc con bạn! Thật đáng để dành một ngày DIY nó như một món quà Xmas. 


## Dự án

**Grove - Giới thiệu về Nút & Đèn LED Chuỗi**: Sơ cấp-Ví dụ - Tôi cá là Người mới bắt đầu sẽ mỉm cười sau dự án - đã gửi cho tôi một bức ảnh tự sướng!

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ingo-lohs/grove-introduction-in-a-button-led-string-light-f7e4d6/embed' width='350'></iframe>


**Sử dụng nút Grove để điều khiển đèn LED Grove**: Cách kết nối và sử dụng Nút Grove để điều khiển bộ ổ cắm Grove LED.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/user50338573/using-grove-button-to-control-grove-led-96d00b/embed' width='350'></iframe>

**Các module nút và LED Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/RCtsxwx4OaA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/78lVn_-oYaY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật

Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>