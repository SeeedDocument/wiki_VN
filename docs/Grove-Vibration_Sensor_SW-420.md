---
name: Grove - Vibration Sensor (SW-420)
category: Sensor
bzurl: 
oldwikiname: 
prodimagename:
surveyurl: 
sku: 101020586
tags:
---

![](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/img/main.jpg)

Grove - Vibration Sensor (SW-420) là một cảm biến rung không định hướng độ nhạy cao. Khi module ổn định, mạch được bật và đầu ra ở mức cao. Khi chuyển động hoặc rung động xảy ra, mạch sẽ bị ngắt kết nối trong thời gian ngắn và đầu ra ở mức thấp. Đồng thời, bạn cũng có thể điều chỉnh độ nhạy theo nhu cầu của riêng bạn.

Nói chung, đây là một module hoàn hảo cho cảm biến rung hoặc nghiêng.


<p style=":center"><a href="https://www.seeedstudio.com/Grove-Vibration-Sensor-%28SW-420%29-p-3158.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>

## Phiển bản

| Phiên bản sản phẩm  | Thay đổi                                                                                               | Ngày phát hành |
|------------------|-------------------------------------------------------------------------------------------------------|---------------|
| Grove - Vibration Sensor (SW-420) | Ban đầu                                                                                               | 09/2018      |

## Đặc điểm

- Không định hướng
- Độ nhạy cao
- Đáp ứng độ rung, độ nghiêng
- Không thấm nước
- Kháng nén


## Thông số kỹ thuật

|Item|Giá trị|
|---|---|
|Điện áp hoạt động|3.3V / 5V|
|Giao diện|Số|
|Kích thước |Dài: 40mm Rộng: 20mm Cao: 10mm| 
|Cân nặng|4.3g|
|Kích thước đóng gói|Dài: 140mm Rộng: 85mm Cao: 10mm|
|Tổng trọng lượng|10g|


## Các ứng dụng

- Báo trộm ô tô, xe đạp, xe máy
- Điều khiển trò chơi
- Phát hiện rung động

## Tổng quan về phần cứng

### Sơ đồ chân

![](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/img/pin_map.jpg)


### Sơ đồ

![](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/img/Schematic.jpg)


Đầu tiên, hãy bắt đầu với ** SW1 ** ở góc dưới bên trái. Trên thực tế, ** SW1 ** là module rung ** SW-420 **. Khi module ở trạng thái ổn định, module được bật. ** Pin2 ** của ** U1A ** được kết nối với ** GND ** mặc dù ** SW1 **.

** VR1 ** là chiết áp, ** Pin2 ** của chiết áp được kết nối với ** Pin3 ** của ** U1A **

**U1A** là một [bộ so sánh](https://en.wikipedia.org/wiki/Comparator). Đối với các so sánh, 


$$
V_{out} = 
\begin{cases} 
High,  & \mbox{if }V_+ > V_-  \\
Low,  & \mbox{if }V_+ < V_- 
\end{cases}
$$

**V+** kết nối với **Pin3**, **V-** kết nối với **Pin2**, **V<sub>out</sub>** kết nối với **Pin1**.

Đối với **V+** bạn có thể điều chỉnh nó bằng cách xoay chiết áp, ví dụ, chúng ta có thể làm cho nó $VCC/2$.

Đối với **V-**, nó phụ thuộc vào **SW1(SW-420)**:

- Nếu module này ở trạng thái ổn định, **SW1** được bật, Pin2 của **U1A** được nối xuống **GND** qua **SW1**. Nó sẽ là:


$$
\left. \begin{array}{l}  & V- = 0V \\ & V+ = VCC/2 \end{array} \right\}  V_{out} = High
$$


- Nếu module rung hoặc nghiêng, **SW1** sẽ bị tắt, điện áp của **V-** sẽ được kéo lên bởi **VCC** qua R1. Một khi **V-** cao hơn VCC / 2, sau đó:

$$
\left. \begin{array}{l}  & V- > VCC/2 \\ & V+ = VCC/2 \end{array} \right\}  V_{out} = Low
$$


Bây giờ bạn có thể đặt ** V + ** để điều chỉnh độ nhạy, chỉ cần nhớ: điện áp của ** V + ** càng thấp, độ nhạy càng cao😆




## Các nền tảng hỗ trợ


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo_n.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo_n.jpg)  |

!!!Chú ý
    Các nền tảng được đề cập ở trên được hỗ trợ như chỉ dẫn của phần mềm của module hoặc khả năng tương thích về mặt lý thuyết. Chúng tôi chỉ cung cấp thư viện phần mềm hoặc các ví dụ cho nền tảng Arduino trong hầu hết các trường hợp. Không thể cung cấp thư viện phần mềm / mã demo cho tất cả các nền tảng MCU. Do đó, người dùng phải viết thư viện phần mềm của riêng họ.



## Getting Started


### Đối với Arduino


#### Phần cứng
**Vật liệu thiết yếu**

| Seeeduino V4.2 | Base Shield | Grove - Vibration Sensor|Grove - Buzzer|
|--------------|-------------|-----------------|----|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/img/thumbnail.jpg)|![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|<a href="http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Vibration-Sensor-%28SW-420%29-p-3158.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Grove-Buzzer-p-768.html" target="_blank">Get One Now</a>|


!!!Chú ý
    **1** Vui lòng cắm cáp USB nhẹ nhàng, nếu không bạn có thể làm hỏng cổng. Vui lòng sử dụng cáp USB có 4 dây bên trong, cáp 2 dây không thể truyền dữ liệu. Nếu bạn không chắc chắn về dây bạn có, bạn có thể nhấp vào [đây](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) để mua.
    
    **2** Mỗi module Grove đi kèm với cáp Grove khi bạn mua. Trong trường hợp bạn mất cáp Grove, bạn có thể nhấp vào [tại đây](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) để mua.



- **Bước 1.** Kết nối Grove - Vibration Sensor (SW-420) tới cổng **D2** của Base Shield.

- **Step 2.** Kết nối Grove - Buzzer tới cổng **D3** của Base Shield.

- **Step 3.** Cắm Grove - Base Shield vào Seeeduino.

- **Step 4.** Kết nối Seeeduino tới PC qua cáp USB.

![](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/img/connect.JPG)

!!!Chú ý
        Nếu bạn không có Grove Base Shield, Chúng ta cũng có thể nối trực tiếp module này tới Seeeduino như bên dưới.



| Seeeduino     |  Grove - Vibration Sensor         |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| NC           | Trắng                    |
| D2           | Vàng                   |



| Seeeduino     |  Grove - Buzzer         |
|---------------|-------------------------|
| 5V            | Đỏ                     |
| GND           | Đen                   |
| NC           | Trắng                    |
| D3           | Vàng                   |


#### Phần mềm

!!!Chú ý
        Nếu đây là lần đầu tiên bạn làm việc với Arduino, chúng tôi thực sự khuyên bạn nên xem [Bắt đầu với Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) trước khi bắt đầu.


- **Bước 1.** Mở Arduino IDE, bắt đầu sketch mới.

- **Bước 2.** Sao chép tất cả các mã dưới đây, hoặc bạn chỉ có thể nhấp vào biểu tượng ![](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/copy.jpg) ở góc trên bên phải của khối mã để sao chép mã sau vào sketch mới.

```C++
// constants won't change. They're used here to set pin numbers:
const int buttonPin = 2;     // the number of the pushbutton pin
const int buzzer =  3;      // the number of the buzzer pin

// variables will change:
int buttonState = 0;         // variable for reading the pushbutton status

void setup() {
  // initialize the LED pin as an output:
  pinMode(buzzer, OUTPUT);
  // initialize the pushbutton pin as an input:
  pinMode(buttonPin, INPUT);
}

void loop() {
  // read the state of the pushbutton value:
  buttonState = digitalRead(buttonPin);

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState == HIGH) {
    // turn LED on:
    digitalWrite(buzzer, LOW);
  } else {
    // turn LED off:
    digitalWrite(buzzer, HIGH);
  }
}
```

- **Bước 3.** Tải demo lên. Nếu bạn không biết cách tải lên mã, vui lòng kiểm tra [Cách tải mã lên](http://wiki.seeedstudio.com/Upload_Code/).

!!!Kết quả
    Nếu mọi việc suôn sẻ, mỗi khi bạn di chuyển, lắc hoặc nghiêng cảm biến Grove - Vibration thì chuông Grove sẽ reo.

### Đối với Codecraft

#### Phần cứng

**Bước 1.** Kết nối Grove - Vibration Sensor tới cổng D2, và kết nối Grove - Buzzer tới cổng D3 của Base Shield.

**Bước 2.** Cắm Base Shield tới Seeeduino/Arduino.

**Bước 3.** Kết nối Seeeduino/Arduino tới PC qua cáp USB.

#### Phần mềm

**Bước 1.** Mở [Codecraft](https://ide.chmakered.com/), add Arduino support, và kéo một thủ tục chính vào khu vực làm việc.

!!!Chú ý
    Nếu đây là lần đầu tiên bạn sử dụng Codecraft, xem thêm [Hướng dẫn về Codecraft bằng Arduino](http://wiki.seeedstudio.com/Guide_for_Codecraft_using_Arduino/).

**Bước 2.** Kéo các khối như hình dưới đây hoặc mở tệp cdc có thể được tải xuống ở cuối trang này.

![cc](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/master/img/cc_Vibration_Sensor.png)

Tải chương trình lên Arduino / Seeeduino của bạn.

!!!Kết quả
    Khi mã kết thúc được tải lên, bộ rung sẽ phát ra tiếng bíp khi cảm biến rung phát hiện rung.

## Nguồn

- **[Zip]** [Grove - Vibration Sensor (SW-420) eagle files](https://github.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/raw/master/res/Grove%20-%20Vibration%20Sensor%20(SW-420)%20v1.1.zip)
- **[Codecraft]** [CDC File](https://raw.githubusercontent.com/SeeedDocument/Grove-Vibration_Sensor-SW-420/master/res/Grove_Vibration_Sensor_CDC_File.zip)

## Dự án

Đây là Video giới thiệu về sản phẩm này, các bản demo đơn giản, bạn có thể dùng thử.

<iframe width="560" height="315" src="https://www.youtube.com/embed/oFmvKxoZIuw?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>



## Hỗ trợ kỹ thuật
Xin đừng ngần ngại gửi vấn đề vào [diễn đàn](https://forum.seeedstudio.com/) của chúng tôi.<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>