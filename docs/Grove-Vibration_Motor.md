---
name: Grove - Vibration Motor
category: Actuator
bzurl: https://seeedstudio.com/Grove-Vibration-Motor-p-839.html
oldwikiname: Grove_-_Vibration_Motor
prodimagename: Gvib.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/gvib.jpg
surveyurl: https://www.research.net/r/Grove-Vibration_Motor
sku: 105020003
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_linkit, plat_pi, plat_bbg
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/img/Gvib.jpg)

Đây là một động cơ rung mini thích hợp như một chỉ báo không nghe được. Khi đầu vào ở mức CAO, động cơ sẽ rung giống như điện thoại di động của bạn ở chế độ im lặng.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Vibration-Motor-p-839.html)

## Phiên bản theo dõi

| Sửa đổi | Miêu tả                                                    | Phát hành       |
|----------|----------------------------------------------------------------|---------------|
| v0.9b    | Phát hành công khai ban đầu                                         |  10/05/2011  |
| v1.0     | Sử dụng trực tiếp cổng I / O để điều khiển Rung động             | 05/11/2011   |
| v1.2     | Transitor được thêm vào, sử dụng dòng điện lớn hơn để điều khiển Rung động | 11/07/2013 |

## Đặc điểm

-   Tương thích Grove
-   Không nghe được
-   Điện năng tiêu thụ ít
-   Độ tin cậy cao

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các thông số kỹ thuật

<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Item
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
</tr>
<tr align="center">
<th scope="row">
Điện áp hoạt động
</th>
<td>
3.0V
</td>
<td>
5.0V
</td>
<td>
5.5V
</td>
</tr>
<tr align="center">
<th scope="row">
Chế độ điều khiển
</th>
<td colspan="3" rowspan="1">
Mức logic
(Khi Logic CAO, động cơ BẬT. Khi THẤP, động cơ TẮT.)
</td>
</tr>
<tr align="center">
<th scope="row">
Tốc độ định mức
</th>
<td colspan="3" rowspan="1">
9000 rpm
</td>
</tr>
</table>

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.


## Getting Started

!!!Chú ý
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.

### Đối với Arduino

Để làm cho nó rung cũng dễ như bật đèn LED. Dưới đây là một ví dụ cho thấy cách bật động cơ rung.

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Vibration Motor |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/img/Gvib_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Vibration-Motor-p-839.html)|

- **Bước 2.** Kết nối Grove - Vibration Motor tới cổng D2 của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://github.com/SeeedDocument/Grove-Vibration_Motor/raw/master/img/vibration_motor.png)

!!!NChú ý
	Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove - Vibration Motor tới Seeeduino như dưới đây.

| Seeeduino       | Grove - Vibration Motor |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| Không kết nối | Trắng                   |
| D2            | Vàng                  |

#### Phần mềm

- **Bước 1.** Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải mã lên](http://wiki.seeedstudio.com/Upload_Code/).

```c
int MoPin = 2;    // vibrator Grove connected to digital pin 9

void setup()  {
    pinMode( MoPin, OUTPUT );
}

void loop()  {

    digitalWrite(MoPin, HIGH);
    delay(1000);

    digitalWrite(MoPin, LOW);
    delay(1000);
}

```

- **Bước 2.** Bây giờ, hãy cảm nhận sự rung động của động cơ của bạn!

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Vibration Motor tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Step 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
    Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://github.com/SeeedDocument/Grove-Vibration_Motor/raw/master/img/cc_Vibration_Motor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã kết thúc được tải lên, bạn sẽ cảm thấy rung động cơ rung.

### Đối với Raspberry Pi

#### Phần cứng

- **Bước 1.** Chuẩn bị các thứ như dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Vibration Motor |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/img/Gvib_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Vibration-Motor-p-839.html)|

- **Bước 2.** Cắm GrovePi_Plus vào Raspberry.
- **Bước 3.** Kết nối Grove - Vibration Motor tới cổng **D8** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry tới PC qua cáp USB.

#### Phần mềm

- **Step 1.** Chuyển hướng đến thư mục của các bản demo:

```
cd yourpath/GrovePi/Software/Python/
```

- **Step 2.** Để xem code

```
nano grove_vibration_motor.py   # "Ctrl+x" to exit #
```

```python
import time
import grovepi

# Connect the Grove Vibration Motor to digital port D8
# SIG,NC,VCC,GND
vibration_motor = 8

grovepi.pinMode(vibration_motor,"OUTPUT")

while True:
    try:
        # Start vibrating for 1 second
        grovepi.digitalWrite(vibration_motor,1)
        print 'start'
        time.sleep(1)

        # Stop vibrating for 1 second, then repeat
        grovepi.digitalWrite(vibration_motor,0)
        print 'stop'
        time.sleep(1)

    except KeyboardInterrupt:
        grovepi.digitalWrite(vibration_motor,0)
        break
    except IOError:
        print "Error"
```

- **Step 3.** Chạy demo.

```
sudo python grove_vibration_motor.py
```


## Nguồn

- **[Eagle]** [Grove - Vibration Motor Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/res/Grove-Vibration_Motor_Eagle_Files.zip)

- **[Datasheet]** [S9013 Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/res/S9013.pdf)

- **[Datasheet]** [ANDA-B1020 Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Motor/master/res/ANDA-B1020_datasheet.pdf)

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Vibration_Motor/master/resource/Grove_Vibration_Motor_CDC_File.zip)



<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Vibration_Motor -->

## Dự án 

**Grove - Giới thiệu về Động cơ Rung - chỉ dành cho người lớn**: Người mới bắt đầu-Ví dụ

<iframe frameborder='0' height='327.5' scrolling='no' src='https://www.hackster.io/ingo-lohs/grove-introduction-in-a-vibration-motor-only-for-adults-2acfc2/embed' width='350'></iframe>


**Lấy cảm hứng từ OVERWATCH, chúng tôi đã tạo ra một đồ chơi Súng Laser bằng gỗ rất thú vị cho vui trong ngày này!**

Súng Laser bằng gỗ và Mục tiêu súng đều dựa trên một bảng Arduino có tên là Seeeduino Lotus. Bộ phát laser trên Súng Laser được điều khiển để bắn xung laser để "kích hoạt" Mục tiêu súng. Và có 3 cảm biến ánh sáng trên Gun Target để phát hiện xung laser. Có vẻ rất đơn giản phải không? Nếu bạn quan tâm đến dự án của chúng tôi, hãy làm một cái cho chính bạn hoặc con bạn! Thật đáng để dành một ngày DIY nó như một món quà Xmas.    

[![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Lotus/master/img/gun.jpg)](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>