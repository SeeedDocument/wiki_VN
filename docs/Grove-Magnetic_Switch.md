---
name: Grove - Magnetic Switch
category: Sensor
bzurl: https://seeedstudio.com/Grove-Magnetic-Switch-p-744.html
oldwikiname: Grove_-_Magnetic_Switch
prodimagename: Magnetic_Switch.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020038 1.jpg
surveyurl: https://www.research.net/r/Grove-Magnetic_Switch
sku: 101020038
tags: grove_digital, io_3v3, io_5v, plat_duino, plat_pi, plat_bbg, plat_wio
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/45d.jpg)

Đây là một module chuyển đổi từ tương thích giao diện Grove. Nó dựa trên công tắc sậy khô đóng gói CT10. CT10 là loại tay đòn đơn (SPST), có các tiếp điểm hoá học thường mở. Cảm biến là loại hai đầu và có thể được kích hoạt bằng nam châm điện, nam châm vĩnh cửu hoặc kết hợp cả hai. Công tắc từ là một công cụ tuyệt vời cho các nhà thiết kế muốn bật và tắt mạch dựa trên độ gần.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Magnetic-Switch-p-744.html)

## Đặc điểm

-   Giao diện tương thích Grove
-   Module Grove 2.0cm x 2.0cm 
-   Bộ phận bên ngoài ít
-   Công suất 10W
-   Đóng gói chắc chắn

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Ý tưởng ứng dụng

-   Cảm biến tiệm cận
-   Cảm biến báo động an ninh
-   Cảm biến mức
-   Cảm biến lưu lượng
-   Bộ đếm xung

## Các thông số kỹ thuật

<table border="1">
<tr>
<th scope="col">
Items
</th>
<th scope="col">
Min
</th>
<th scope="col">
Thông thường
</th>
<th scope="col">
Max
</th>
<th scope="col">
Đơn vị
</th>
</tr>
<tr align="center">
<td>
Điện áp làm việc
</td>
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
<td>
Chuyển đổi năng lượng
</td>
<td colspan="3">
10
</td>
<td>
W
</td>
</tr>
<tr align="center">
<td>
Điện áp chuyển mạch giá trị AC,RMS (lớn nhất)
</td>
<td colspan="3">
&lt; 140
</td>
<td>
V
</td>
</tr>
<tr align="center">
<td>
Chuyển đổi dòng DC
</td>
<td colspan="3">
&lt; 500
</td>
<td>
mA
</td>
</tr>
<tr align="center">
<td>
Dòng tải DC
</td>
<td colspan="3">
&lt; 0.5
</td>
<td>
A
</td>
</tr>
<tr align="center">
<td>
Điện trở tiếp xúc
</td>
<td colspan="3">
&lt;200
</td>
<td>
mΩ
</td>
</tr>
<tr align="center">
<td>
Điện trở cách điện
</td>
<td colspan="3">
&gt;10<sup>6</sup>
</td>
<td>
MΩ
</td>
</tr>
<tr align="center">
<td>
Nhiệt độ hoạt động
</td>
<td>
-40
</td>
<td>
-
</td>
<td>
125
</td>
<td>
℃
</td>
</tr>
<tr align="center">
<td>
Dải hoạt động
</td>
<td>
10
</td>
<td>
-
</td>
<td>
40
</td>
<td>
AT
</td>
</tr>
</table>

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


### Đối với Arduino

#### Thuyết minh

Chân SIG của đầu ra module thường là THẤP. Khi một nam châm tiếp cận công tắc, công tắc từ đóng và chân SIG xuất ra mức CAO.

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Grove - Magnetic Switch |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/45d_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Magnetic-Switch-p-744.html)|

- **Step 2.** Kết nối Grove - Magnetic Switch tới cổng **D2** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/with_ardu.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove-Magnetic-Switch tới Seeeduino như dưới đây.

| Seeeduino | Grove-Magnetic_Switch |
|------|----------------------------|
| 5V   | Đỏ                        |
| GND  | Đen                      |
| NC   | Trắng                      |
| D2   | Vàng                     |

#### Phần mềm

- **Bước 1.** Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [cách tải lên mã](http://wiki.seeedstudio.com/Upload_Code/).

```c
/*******************************************************************************/

/*macro definitions of magnetic pin and LED pin*/
#define MAGNECTIC_SWITCH 2
#define LED 13//the on board LED of the Arduino or Seeeduino

void setup()
{
    pinsInit();
}

void loop() 
{
    if(isNearMagnet())//if the magnetic switch is near the magnet?
    {
        turnOnLED();
    }
    else
    {
        turnOffLED();
    }
}
void pinsInit()
{
    pinMode(MAGNECTIC_SWITCH, INPUT);
    pinMode(LED,OUTPUT);
}

/*If the magnetic switch is near the magnet, it will return ture, */
/*otherwise it will return false                                */
boolean isNearMagnet()
{
    int sensorValue = digitalRead(MAGNECTIC_SWITCH);
    if(sensorValue == HIGH)//if the sensor value is HIGH?
    {
        return true;//yes,return ture
    }
    else
    {
        return false;//no,return false
    }
}
void turnOnLED()
{
    digitalWrite(LED,HIGH);
}
void turnOffLED()
{
    digitalWrite(LED,LOW);
}
```

- **Bước 2.**  Sau đó, đèn LED bật khi có từ tính tiếp cận công tắc. Thử!

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Magnetic Switch tới cổng D2 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/cc_Magnetic_Switch.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy nhiệt độ và độ ẩm được hiển thị trên Màn hình Nối tiếp.

### Đối với Raspberry Pi

#### Phần cứng

- **Bước 1**. Các thứ được sử dụng trong dự án:

| Raspberry pi | GrovePi_Plus | Grove - Magnetic Switch |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/45d_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/Grove-Magnetic-Switch-p-744.html)|

- **Bước 2.** Cắm Grove Base Hat vào Raspberry.
- **Bước 3.** Kết nối Grove-Magnetic-Switch ranger tới cổng **D2** của GrovePi_Plus.
- **Bước 4.** Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/with_rpi.jpg)

#### Phần mềm

- **Bước 1**. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.

- **Step 2.** Điều hướng đến thư mục của các bản demo:

```
cd yourpath/GrovePi/Software/Python/
```

- **Bước 3.** Để xem mã (bản demo này có cùng cách sử dụng với công tắc nghiêng)

```
nano grovepi_tilt_switch.py   # "Ctrl+x" to exit #
```

```py
import time
import grovepi

# Connect the Grove Tilt Switch to digital port D2
# SIG,NC,VCC,GND
tilt_switch = 2

grovepi.pinMode(tilt_switch,"INPUT")

while True:
    try:
        print grovepi.digitalRead(tilt_switch)
        time.sleep(.5)

    except IOError:
        print "Error"
```

- **Bước 4.** Chạy demo.

```
sudo python grovepi_tilt_switch.py
```

- **Bước 5.** Kết quả

Đặt một nam châm lên cảm biến, chân SIG sẽ xuất ra ở mức CAO.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/img/Grovepi_tilt_Switch_00.png)

## Nguồn
- **[Eagle]**  [Grove-Magnetic Switch v0.9 Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/res/Magnetic_Switch.zip)

- **[Eagle]**  [Grove-Magnetic Switch v1.3 Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/res/Grove-Magnetic_Switch_v1.3_Eagle_File.zip)

- **[PDF]**  [Grove-Magnetic Switch v1.3 PDF File](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/res/Grove-Magnetic_Switch_v1.3_PDF_File.pdf)

- **[Datasheet]**  [CT10 Datasheet](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/res/CT10.pdf)

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Magnetic_Switch/master/res/Grove_Magnetic_Switch_CDC_File.zip)

<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Magnetic_Switch -->

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>