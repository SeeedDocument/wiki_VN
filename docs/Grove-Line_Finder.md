---
name: Grove - Line Finder
category: Sensor
bzurl: https://www.seeedstudio.com/Grove-Line-Finder-v1.1-p-2712.html
oldwikiname: Grove - Line Finder
prodimagename: Grovelinefinder1.jpg
surveyurl: https://www.research.net/r/grove-line-finder
sku: 101020009
---


![](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/images/Grovelinefinder1.jpg)

Grove-Line finder được thiết kế cho Robot line-following. Nó có một đèn LED phát ra IR và một phototransistor nhạy IR. Nó có thể xuất tín hiệu số đến vi điều khiển để robot có thể đi theo một đường màu đen trên nền trắng hoặc ngược lại.

[![](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/images/300px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-Line-Finder-v1.1-p-2712.html)

## Phiên bản


| Phiên bản sản phẩm              | Thay đổi                                                                                                                                                                                    | Ngày phát hành |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Line Finder V1.0| Ban đầu                                                                                                                                                                                    | 29/1/2010      |
| Grove-Line Finder V1.1 | Thêm điểm kiểm tra                                                                                                                                                                                 | 28/12/2015      |


## Các thông số kỹ thuật

| Tham số              | Giá trị                                                   |
|------------------------|---------------------------------------------------------------|
| Nguồn cấp           | 5                                                             |
| Chế độ đầu ra số    | TTL (Cao khi phát hiện màu đen, Thấp khi phát hiện màu trắng) |
| Kết nối              | Giao diện Buckled Grove 4 pin                                 |
| Kích thước              | 20mm*20mm                                                     |
| ROHS                   | Yes                                                           |
| Diode phản chiếu hình ảnh | RS-06WD                                                       |
| So sánh             | MV358                                                         |

!!!Mẹo
    Thông tin chi tiết về các module Grove vui lòng tham khảo [Hệ thống Grove](http://wiki.seeedstudio.com/Grove_System/)

## Các nền tảng được hỗ trợ

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg) |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.

##  Getting Started

### Đối với Arduino

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Seeeduino V4.2 | Base Shield|  Grove - Button |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/img/line_finder_s.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Line-Finder-v1.1-p-2712.html)|

- Bước 2. Kết nối Grove-line finder tới cổng D3 của Grove-Base Shield.
- Bước 3. Cắm Grove - Base Shield vào Seeeduino.
- Bước 4. Kết nối Seeeduino tới PC qua một cáp USB.


![](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/img/seeeduino_line_finder.jpg)

!!!Chú ý
Nếu chúng tôi không có Grove Base Shield,chúng tôi cũng có thể kết nối trực tiếp Grove-Line finder tới Seeeduino như dưới đây.

| Seeeduino       | Grove-Line finder |
|---------------|-------------------------|
| 5V           | Đỏ                     |
| GND           | Đen                   |
| Not Conencted | Trắng                   |
| D3            | Vàng                  |

#### Phần mềm

- Bước 1. Sao chép code vào Arduino IDE và tải lên.

```c
//------------------------------------------------------------
//Name: Line finder digital mode
//Function: detect black line or white line
//Parameter:   When digital signal is HIGH, black line
//             When digital signal is LOW, white line
//-------------------------------------------------------------
int signalPin =  3;    // connected to digital pin 3
void setup()   {
  pinMode(signalPin, INPUT); // initialize the digital pin as an output:
  Serial.begin(9600);  // initialize serial communications at 9600 bps:
}
// the loop() method runs over and over again,
// as long as the Arduino has power
void loop()
{
  if(HIGH == digitalRead(signalPin))
    Serial.println("black");
  else  Serial.println("white");  // display the color
  delay(1000);                  // wait for a second
}
```

- Bước 2. Mở cổng serial và chúng ta sẽ thấy "black" khi cảm biến trên vạch màu đen và "white" trên vùng màu trắng.

```
white
white
white
black
black
black
black
black
```

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Line Finder tới cổng D3 của Base Shield.

**Bước 2.** Cắm Base Shield vào Seeeduino/Arduino của bạn.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), thêm hỗ trợ Arduino và kéo một lệnh chính vào vùng làm việc.

!!!Chú ý
   Nếu đây là lần đầu tiên bạn sử dụng Codecraft, hãy xem thêm [Hướng dẫn sử dụng Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove_Line_Finder/master/img/cc_Line_Finder.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
   Khi mã được tải lên, bạn sẽ thấy dòng tìm thấy hoặc không trong Serial Monitor.

### Đối với Raspberry Pi

#### Phần cứng

- Bước 1. Chuẩn bị những thứ dưới đây:

| Raspberry pi | GrovePi_Plus | Grove - Line Finder |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/img/line_finder_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Line-Finder-v1.1-p-2712.html)|

- Bước 2. Cắm GrovePi_Plus vào Raspberry.
- Bước 3. Kết nối Grove-Line Finder tới cổng D7 của GrovePi_Plus.
- Bước 4. Kết nối Raspberry Pi tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/img/rasp_line_finder.jpg)

#### Phần mềm

- Bước 1. Theo dõi [Cài đặt phần mềm](http://wiki.seeedstudio.com/Grove_Base_Hat_for_Raspberry_Pi/#installation) để cấu hình môi trường phát triển.
- Bước 2. Git nhân bản kho lưu trữ Github.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```
- Bước 3. Thực hiện lệnh bên dưới.

```
cd ~/GrovePi/Software/Python
python grove_line_finder.py
```

Đây là code grove_line_finder.py.

```python
import time
import grovepi

# Connect the Grove Line Finder to digital port D7
# SIG,NC,VCC,GND
line_finder = 7

grovepi.pinMode(line_finder,"INPUT")

while True:
    try:
        # Return HIGH when black line is detected, and LOW when white line is detected
        if grovepi.digitalRead(line_finder) == 1:
            print ("black line detected")
        else:
            print ("white line detected")

        time.sleep(.5)

    except IOError:
        print ("Error")
```

- Bước 4. Chúng ta sẽ thấy đường màu đen được phát hiện khi cảm biến ở trên đường màu đen.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_line_finder.py 
black line detected
black line detected
white line detected
white line detected

```

## Nguồn

- **[Eagle&PDF]** [Grove-Line Finder Schematic V1.0](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/res/202000970_Grove%20-%20Line%20Finder%EF%BC%88CN%EF%BC%89%20v1.0.zip)
- **[Eagle&PDF]** [Grove-Line Finder Schematic V1.1](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/res/202000932_Grove%20-%20Line%20Finder%20v1.1.zip)
- **[Datasheet]** [LMV358.PDF](https://github.com/SeeedDocument/Grove_Line_Finder/raw/master/res/Lmv358.pdf)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove_Line_Finder/master/res/Grove_Line_Finder_CDC_File.zip)

## Hỗ trợ kỹ thuật
Vui lòng gửi bất kỳ vấn đề kỹ thuật vào [diễn đàn](http://forum.seeedstudio.com/) của chúng tôi. <br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>