---
name: Grove - Buzzer
category: Actuator
bzurl: https://www.seeedstudio.com/Grove-Buzzer-p-768.html
oldwikiname: Grove - Buzzer
prodimagename: Grove%20Buzzer.jpg
surveyurl: https://www.surveymonkey.com/r/grove-buzzer
sku: 107020000
---


![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/Grove%20Buzzer.jpg)

Module Grove - Buzzer có  [piezo buzzer](https://en.wikipedia.org/wiki/Buzzer#Piezoelectric) là thành phần chính. Piezo có thể được kết nối với đầu ra kỹ thuật số và sẽ phát ra âm báo khi đầu ra CAO. Ngoài ra, nó có thể được kết nối với đầu ra điều chế độ rộng xung tương tự để tạo ra các âm và hiệu ứng khác nhau.

[![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/300px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)

## Phiên bản


| Phiên bản sản phẩm              | Các thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Buzzer V1.0| Ban đầu                                                                                                                                                                                    | 25/11/2010      |
| Grove-Buzzer V1.1 | Thêm Transistor S9013                                                                                                                                                                                  |  30/05/2014      |


## Đặc điểm

- Dễ dàng sử dụng còi áp điện
- Sử dụng Cáp Grove 4 chân tiêu chuẩn để kết nối với các mô đun Grove khác như - [Grove Power Modules](/Grove_System/) và Grove - Base Shield

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)
    
## Các thông số kỹ thuật

| Items              | Giá trị |
|--------------------|---------------|
| Điện áp hoạt động  | 3.3V/5V       |
| Đầu ra âm thanh     | ≥85dB         |
| Tần số cộng hưởng| 2300±300Hz    |

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


##  Getting Started

### Đối với Arduino

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Buzzer |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)|

- **Bước 2.** Kết nối Grove-Buzzer tới cổng D6 của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/seeeduino_buzzer.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-buzzer tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Buzzer |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D6            | Vàng                  |

#### Phần mềm

- Bước 1. Sao chép mã vào Arduino IDE và tải lên.

```c
void setup()
{
  pinMode(6, OUTPUT);
}

void loop()
{
  digitalWrite(6, HIGH);
  delay(1000);
  digitalWrite(6, LOW);
  delay(1000);
}
```

- Bước 2. Chúng tôi sẽ nghe thấy tiếng chuông bật và tắt.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Buzzer tới cổng D6 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Buzzer/master/img/cc_Buzzer.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã kết thúc được tải lên, bạn sẽ nghe thấy âm thanh chuông liên tục.

### Đối với Raspberry Pi (Với Grove Base Hat cho Raspberry Pi)

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | Grove Base Hat for RasPi| Grove -  Buzzer|
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/thumbnail.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)|

- **Bước 2**. Cắm Grove Base Hat vào Raspberry.
- **Bước 3**. Kết nối Grove Buzzer tới cổng PWM của Base Hat.
- **Bước 4**. Kết nối Raspberry Pi tới PC qua cáp USB.
![](https://github.com/SeeedDocument/Grove_Base_Hat_for_Raspberry_Pi/raw/master/img/connect1.jpg)


#### Phần mềm

- **Step 1**. Theo dõi [Setting Software](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- **Bước 2**. Tải xuống tệp nguồn bằng cách nhân bản thư viện grove.py.

```
cd ~
git clone https://github.com/Seeed-Studio/grove.py

```

- **Bước 3**. Thực hiện các lệnh dưới đây để chạy mã.

```
cd grove.py/grove
python grove_pwm_buzzer.py
```


Sau đây là mã the grove_led.py.

```python

from __future__ import print_function

import time
from mraa import getGpioLookup
from upm import pyupm_buzzer as upmBuzzer

def main():
    print("Insert Grove-Buzzer to Grove-Base-Hat slot PWM[12 13 VCC GND]")

    # Grove Base Hat for Raspberry Pi
    #   PWM JST SLOT - PWM[12 13 VCC GND]
    pin = 12
    #
    # Create the buzzer object using RaspberryPi GPIO12
    mraa_pin = getGpioLookup("GPIO%d" % pin)
    buzzer = upmBuzzer.Buzzer(mraa_pin)

    chords = [upmBuzzer.BUZZER_DO, upmBuzzer.BUZZER_RE, upmBuzzer.BUZZER_MI,
              upmBuzzer.BUZZER_FA, upmBuzzer.BUZZER_SOL, upmBuzzer.BUZZER_LA,
              upmBuzzer.BUZZER_SI];

    # Print sensor name
    print(buzzer.name())

    # Play sound (DO, RE, MI, etc.), pausing for 0.1 seconds between notes
    for chord_ind in range (0,7):
        # play each note for a half second
        print(buzzer.playSound(chords[chord_ind], 500000))
        time.sleep(0.1)

    print("exiting application")

    # Delete the buzzer object
    del buzzer

if __name__ == '__main__':
    main()



```
!!!Kết quả
    Nếu mọi thứ suôn sẻ, còi sẽ reo vài lần rồi dừng, chương trình sẽ tự động thoát.
     


### Đối với Raspberry Pi (với GrovePi_Plus)

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Buzzer |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)|

- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Step 3.** Kết nối Grove-Buzzer tới cổng D8 của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/rasp_buzzer.jpg)

#### Phần mềm

- **Bước 1.** Theo dõi [Setting Software](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) để cài đặt môi trường phát triển.
- **Bước 2.** Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```
- **Bước 3.** Thực hiện các lệnh dưới đây.

```
cd ~/GrovePi/Software/Python
python grove_buzzer.py
```

Đây là mã the grove_buzzer.py.

```python
import time
import grovepi

# Connect the Grove Buzzer to digital port D8
# SIG,NC,VCC,GND
buzzer = 8

grovepi.pinMode(buzzer,"OUTPUT")

while True:
    try:
        # Buzz for 1 second
        grovepi.digitalWrite(buzzer,1)
        print ('start')
        time.sleep(1)

        # Stop buzzing for 1 second and repeat
        grovepi.digitalWrite(buzzer,0)
        print ('stop')
        time.sleep(1)

    except KeyboardInterrupt:
        grovepi.digitalWrite(buzzer,0)
        break
    except IOError:
        print ("Error")
```

- **Bước 4.** Chúng ta sẽ nghe thấy tiếng chuông bật và tắt.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_buzzer.py
start
stop
start
stop
```


### Với TI LaunchPad

#### Phần cứng

- Ví dụ này cho thấy cách sử dụng module buzzer Grove để chơi các giai điệu. Nó gửi một sóng vuông có tần số thích hợp đến bộ rung, tạo ra âm tương ứng.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/Buzzer.jpg)

#### Phần mềm

```c
/*
  Buzzer
 The example use a buzzer to play melodies. It sends a square wave of the
 appropriate frequency to the buzzer, generating the corresponding tone.

 The circuit:
 * Buzzer attached to pin39 (J14 plug on Grove Base BoosterPack)
 * one side pin (either one) to ground
 * the other side pin to VCC
 * LED anode (long leg) attached to RED_LED
 * LED cathode (short leg) attached to ground

 * Note:
 This example code is in the public domain.

 http://www.seeedstudio.com/wiki/index.php?title=GROVE_-_Starter_Kit_v1.1b#Grove_-_Buzzer

*/

/* Macro Define */
#define BUZZER_PIN               39            /* sig pin of the buzzer */

int length = 15;         /* the number of notes */
char notes[] = "ccggaagffeeddc ";
int beats[] = { 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 2, 4 };
int tempo = 300;

void setup()
{
    /* set buzzer pin as output */
    pinMode(BUZZER_PIN, OUTPUT);
}

void loop()
{
    for(int i = 0; i < length; i++) {
        if(notes[i] == ' ') {
            delay(beats[i] * tempo);
        } else {
            playNote(notes[i], beats[i] * tempo);
        }
        delay(tempo / 2);    /* delay between notes */
    }

}

/* play tone */
void playTone(int tone, int duration) {
    for (long i = 0; i < duration * 1000L; i += tone * 2) {
        digitalWrite(BUZZER_PIN, HIGH);
        delayMicroseconds(tone);
        digitalWrite(BUZZER_PIN, LOW);
        delayMicroseconds(tone);
    }
}

void playNote(char note, int duration) {
    char names[] = { 'c', 'd', 'e', 'f', 'g', 'a', 'b', 'C' };
    int tones[] = { 1915, 1700, 1519, 1432, 1275, 1136, 1014, 956 };

    // play the tone corresponding to the note name
    for (int i = 0; i < 8; i++) {
        if (names[i] == note) {
            playTone(tones[i], duration);
        }
    }
}
```

## Nguồn

- **[Eagle&PDF]** [Grove - Buzzer Schematic Files v1.1](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/Grove-Buzzer_V1.1_eagle.zip)
- **[Eagle&PDF]** [Grove - Buzzer Schematic Files v1.0](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/Grove_-_Buzzer_v1.0_Source_File.zip)
- **[DataSheet]** [S9013datasheet](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/S9013.pdf)
- **[More Reading]** [Wooden Laser Gun](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Buzzer/master/res/Grove_Buzzer_CDC_File.zip)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Button/master/img/gun.jpg)

Lấy cảm hứng từ OVERWATCH, chúng tôi đã tạo ra một đồ chơi Súng Laser bằng gỗ rất thú vị cho vui trong ngày này!

Súng Laser bằng gỗ và Mục tiêu súng đều dựa trên một bảng Arduino có tên là Seeeduino Lotus. Bộ phát laser trên Súng Laser được điều khiển để bắn xung laser để "kích hoạt" Mục tiêu súng. Và có 3 cảm biến ánh sáng trên Gun Target để phát hiện xung laser. Có vẻ rất đơn giản phải không? Nếu bạn quan tâm đến dự án của chúng tôi, hãy làm một cái cho chính bạn hoặc con bạn! Thật đáng để dành một ngày DIY nó như một món quà Xmas.  

## Dự án

**Grove - Giới thiệu về Buzzer**: Bước đầu tiên của tôi với các thành phần 'cắm & chơi' Grove. Đây chủ yếu là một bộ rung.

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ingo-lohs/grove-introduction-in-a-buzzer-981efd/embed' width='350'></iframe>

**Giám sát chất thải nước**: Hàng triệu gallon nước bị lãng phí mỗi năm. Học cách tiết kiệm nước với dự án này!

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/exp0nge/water-waste-monitor-98378e/embed' width='350'></iframe>


**Module Buzzer Grove**:
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/XBqvG6R1ueA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/ug8dJHPmdMA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>