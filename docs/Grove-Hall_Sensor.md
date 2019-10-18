---
name: Grove - Hall Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Hall-Sensor-p-965.html
oldwikiname: Grove_-_Hall_Sensor
prodimagename: Grove-Hall_Sensor_New.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/product/hall sensor.jpg
surveyurl: https://www.research.net/r/Grove-Hall_Sensor
sku: 101020046
tags: grove_digital, io_5v, plat_duino, plat_linkit
---

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/img/Grove-Hall_Sensor_New.jpg)

Cảm biến Hall dựa trên Hiệu ứng Hall, là sự tạo ra sự chênh lệch điện áp trên một dây dẫn điện, ngang với một dòng điện trong dây dẫn và từ trường vuông góc với dòng điện. Có một công tắc thời gian liên tục trên Grove này. Đầu ra của các thiết bị này chuyển sang mức thấp (bật) khi từ trường (cực nam) vuông góc với cảm biến Hall vượt quá ngưỡng điểm hoạt động BOP và nó chuyển sang mức cao (tắt) khi từ trường biến mất. Các cành có thể được sử dụng để đo RPM.

[![](https://raw.githubusercontent.com/SeeedDocument/common/master/Get_One_Now_Banner.png)](http://www.seeedstudio.com/depot/grove-hall-sensor-p-965.html)


## Phiên bản theo dõi

| Phiên bản | Mô tả           | Phát hành    |
|----------|------------------------|------------|
| Grove - Hall Sensor v0.9b    | Phát hành công khai ban đầu | 3/10/2011 |


## Đặc tính

-   Giao diện tương thích Grove
-   Giai đoạn chuyển tiếp 400ns cho tăng và giảm.
-   Cảm biến hiệu ứng hội trường thời gian liên tục
-   Bảo vệ pin ngược

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

    
## Các thông số kỹ thuật

| Item                  | Min | Điển hình | Max | Đơn vị |
|-----------------------|-----|---------|-----|------|
| Nguồn cấp        | 3.8 | 5.0     | 24  | V    |
| Dòng cấp      | 4.1 | -       | 24  | mA   |
| Nhiệt độ hoạt động  | -40 | -       | 85  | ºC   |

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

## Ý tưởng ứng dụng

-   Đồng hồ RPM.
-   Động cơ DC đơn giản.

## Getting Started

!!!Chú thích
    Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi chắc chắn khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


### Đối với Arduino

#### Thuyết minh

Cảm biến Hall được sử dụng bằng cách sử dụng các ngắt ngoài có sẵn trên arduino / seeeduino. Trong ví dụ này, chúng tôi đang sử dụng ngắt 0, được tìm thấy trên chân số 2. Đối với các ngắt khác, hãy xem phần [attachInterrupt()](http://www.arduino.cc/en/Reference/AttachInterrupt).

#### Phần cứng

- **Bước 1.** Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield| Grove - Hall Sensor |
|--------------|-------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/img/Grove-Hall_Sensor_New%20_small.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](http://www.seeedstudio.com/depot/grove-hall-sensor-p-965.html)|

- **Bước 2.** Kết nối Grove - Hall Sensor tới cổng **D2** của Grove-Base Shield.
- **Bước 3.** Cắm Grove - Base Shield vào Seeeduino.
- **Bước 4.** Kết nối Seeeduino tới PC qua một cáp USB.

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield, chúng tôi cũng có thể kết nối trực tiếp Grove - Hall Sensor tới Seeeduino như dưới đây.

| Seeeduino       | Grove - Hall Sensor |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D2            | Vàng                  |


#### Phần mềm

- **Bước 1.**  Tải xuống [Hall Sensor Code](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/res/Grove-Hall_Sensor_Demo_Code.zip)

- **Bước 2.**  Mở một trong hai mã. Ví dụ bản Demo **MagnetControlLED**


- **Bước 3.**  Sao chép mã vào Arduino IDE và tải lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [how to upload code](http://wiki.seeedstudio.com/Upload_Code/).


```c
/****************************************************************************/	
//	Function: When a magnet whose south pole is facing up is approaching to 
//			  the onboard sensor, the LED will be turned on.Otherwise, the 
//			  LED will be turned off.
//	Hardware: Grove - Hall Sensor, Grove - LED
//	Arduino IDE: Arduino-1.0
//	Author:	 FrankieChu		
//	Date: 	 Jan 20,2013
//	Version: v1.0
//	by www.seeedstudio.com
//
//  This library is free software; you can redistribute it and/or
//  modify it under the terms of the GNU Lesser General Public
//  License as published by the Free Software Foundation; either
//  version 2.1 of the License, or (at your option) any later version.
//
//  This library is distributed in the hope that it will be useful,
//  but WITHOUT ANY WARRANTY; without even the implied warranty of
//  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
//  Lesser General Public License for more details.
//
//  You should have received a copy of the GNU Lesser General Public
//  License along with this library; if not, write to the Free Software
//  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA
//
/*macro definitions of magnetic pin and LED pin*/
#define HALL_SENSOR 2
#define LED	4//the Grove - LED is connected to D4 of Arduino

void setup()
{
 	pinsInit();
}
 
void loop() 
{
	if(isNearMagnet())//if the hall sensor is near the magnet?
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
	pinMode(HALL_SENSOR, INPUT);
	pinMode(LED,OUTPUT);
}

/*If the hall sensor is near the magnet whose south pole is facing up, */
/*it will return ture, otherwise it will return false.				*/
boolean isNearMagnet()
{
	int sensorValue = digitalRead(HALL_SENSOR);
	if(sensorValue == LOW)//if the sensor value is LOW?
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

- **Bước 4.**  Khi một nam châm có cực nam hướng lên đang tiến đến cảm biến trên bo mạch, đèn LED sẽ được bật. Nếu không, đèn LED sẽ bị tắt.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Hall Sensor tới cổng D2, và kết nối Grove - Red LED tới cổng D4 của Base Shield.

**Step 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Step 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/img/cc_Hall_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, đèn LED sẽ sáng khi Cảm biến Hall phát hiện những thay đổi trong từ trường.

## Nguồn

- **[Eagle]** [Grove-Hall Sensor Schematic](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/res/Twig_Hall_Sensor_v0.9b.zip)

- **[Demo]** [Hall Sensor Demo Code](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/res/Grove-Hall_Sensor_Demo_Code.zip)

- **[Datasheet]** [A1101 datasheet](http://www.allegromicro.com/en/Products/Part_Numbers/1101/1101.pdf)

- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Hall_Sensor/master/res/Grove_Hall_Sensor_CDC_File.zip)


<!-- This Markdown file was created from http://www.seeedstudio.com/wiki/Grove_-_Hall_Sensor -->

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>