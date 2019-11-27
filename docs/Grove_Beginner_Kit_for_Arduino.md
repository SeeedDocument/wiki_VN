---
name: Grove Beginner Kit for Arduino
category: Others
bzurl:  
oldwikiname:  
prodimagename:
surveyurl: 
sku: 110020171
---


## HỆ THỐNG GROVE 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/pack.jpg)

Grove là một hệ thống modular prototyping (mô-đun mẫu) bao gồm một đơn vị cơ sở và các mô-đun khác nhau với đầu nối tiêu chuẩn. Đơn vị cơ sở nói chung là một bộ vi xử lý cho phép giao tiếp, xử lý và kiểm soát đầu vào hoặc đầu ra từ các mô-đun Grove. Mỗi mô-đun Grove thường xử lý một chức năng duy nhất, từ một nút bấm đơn giản cho đến cảm biến nhịp tim phức tạp hơn. Đầu nối Grove được tiêu chuẩn hóa cho phép người dùng lắp ráp các đơn vị Grove một cách dễ dàng, so với hệ thống sử dụng jump hay việc hàn, việc lắp ráp hoặc tháo rời dễ dàng hơn nhiều, giúp đơn giản hóa hệ thống cho học tập để thử nghiệm, xây dựng và tạo sản phẩm mẫu.
Gove cũng được cung cấp Pin Header Converter hoặc Grove Base HAT có sẵn cho các nền tảng phát triển đa dạng cho những ai muốn sử dụng các mô-đun cảm biến và các mô-đun khác mà không sử dụng Grove System Development Board.

![Grove header](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/grove-wire.jpg)![Grove connector](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connector.png)![Grove-jumper wire](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/jumperwire.png)

Người dùng để có thể sử dụng hệ thống Grove cần có ít nhất một số nền tảng kiến thức điện tử cơ bản, nếu không, bạn cần xem hướng dẫn căn bản này để tìm hiểu một số thao tác cơ bản trên hệ thống Grove, phần đầu tiên của hướng dẫn này bao gồm danh sách thông tin cơ bản về các thành phần có trong bộ starter kit, tiếp theo là thiết lập Arduino IDE cho Seeeduino Lotus. Sau đó, 11 bài hướng dẫn cung cấp nguyên lý hoạt động cơ bản cho từng thành phần riêng lẻ trong bộ started kit và các ứng dụng bằng cách kết hợp nhiều mô-đun lại với nhau, giúp người học hiểu biết và hiểu biết cơ bản việc lập trình với hệ thống Grove.

## Grove Beginner Kit cho Arduino


Grove Beginner Kit cho Arduino chứa một Seeeduino Lotus v1.1 dev board (Tương thích với Arduino) và 8 mô-đun. Các thông tin chi tiết được liệt kê dưới đây.

### Development Board

#### Seeeduino Lotus V1.1

Seeeduino Lotus là một development board với bộ vi điều khiển ATMEGA328, nó là sự kết hợp của Seeeduino và Grove Base Shield. Nó sử dụng bộ vi điều khiển Atmel ATmege328-MU và chip CP2102N, ATmege328-MU là bộ vi điều khiển 8 bit AVR hiệu suất cao, công suất thấp, CP2102N là chip chuyển đổi USB sang serial cho phép bạn giao tiếp với Seeeduino Lotus với máy tính sử dụng Cáp USB. Seeeduino Lotus có 14 đầu vào / ra kỹ thuật số (6 có thể được sử dụng làm đầu ra PWM) và 7 đầu vào / ra Analog, kết nối micro USB, 1 ICSP header, 12 đầu nối Gove connector, nút reset.


**Các tính năng chính**

- Hoàn toàn tương thích với Arduino UNO
- Vi điều khiển ATmega328
- 2 đầu nối Grove connector
- 14 chân I / O kỹ thuật số (6 đầu ra PWM)
- 6 đầu vào tương tự
- ISP Header
- Tương thích Arduino UNO-R3 shield
- Sử dụng cap micro USB để lập trình và cung cấp nguồn
- Điện áp hoạt động 5V
- Hỗ trợ Windows, Mac OS và Linux

**Phần cứng**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/pinout.png)

LED-D13: Một đèn LED được kết nối với chân D13 của bo mạch. Nó có thể được sử dụng như một đèn chỉ báo LED trên board cho programs/sketches.

Đầu vào USB: Cổng USB được sử dụng để kết nối bo mạch với PC để lập trình và cung cấp nguồn. Micro USB là loại cổng USB rất phổ biến, có thể được tìm thấy với hầu hết các điện thoại Android và các thiết bị khác. Bạn có thể tìm thấy rất nhiều các dây cáp như thế xung quanh nhà của bạn.

Reset: Nút bấm này được đặt thuận tiện ở bên sườn của board để cho phép bạn reset board Seeeduino, trong khi các nút bấm trên bo mạch Arduino khác được đặt ở lớp trên cùng khiến nó khó tiếp cận khi có tấm chắn được gắn vào.

Chân nguồn, Chân tương tự & Chân kỹ thuật số: Những headers này được thêm vào để khi bạn muốn kết nối các cảm biến và bộ truyền động không có các connector tương thích, và đặc biệt là các chân nguồn được sử dụng khi bạn muốn cấp nguồn cho nhiều cảm biến / thiết bị hơn.

Grove Connectors: Seeed Studio có nhiều cảm biến / thiết bị có thể sử dụng kết nối Analog, Digital, I2C và UART này. Ngoài ra, chúng tôi bán các Grove connectors độc ​​lập để giúp bạn tạo các kết nối cảm biến của riêng của chúng tôi.

ICSP: Đây là kết nối ICSP cho ATmega328P, nó được đặt ở tiêu chuẩn ICSP / SPI cho phần cứng tương thích Arduino Uno, Due, Mega và Leonardo. Các chân SPI trong cổng này: MISO, SCK và MOSI, cũng được kết nối với các chân kỹ thuật số 12, 13 và 11 tương tự như của Arduino Uno.

USB 2 Uart: Pinout của USB-2-Uart. Những pads này có thể được sử dụng để tương tác với các thiết bị UART khác bằng cách thiết lập ATmega328 on-board ở chế độ reset. Điều này làm cho Seeeduino Lotus được sử dụng làm board tiện ích USB2UART.

**Arduino UNO và Seeeduino Lotus**

|                        | Seeeduino Lotus V1.1 | Arduino Uno R3 |
|:----------------------:|:--------------------:|:--------------:|
|      Ngày phát hành      |        2018/03       |     2016/02    |
|     Vi điều khiển    |      ATMega328P      |   ATMega328P   |
|    Điện áp hoạt động   |          5V          |       5V       |
|          Flash         |         32KB         |      32KB      |
|          SRAM          |          2KB         |       2KB      |
|         EEPROM         |          1KB         |       1KB      |
| Power supply interface |       Micro USB      |  USB, DC Port  |
|    Grove Connectors    |          12          |      None      |

#### Các cảm biến 

**[Grove - Buzzer](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer.jpg)

Mô-đun này sử dụng bộ rung Piezo làm thành phần chính, nó có thể tạo ra âm cao trong khi nó được kết nối với đầu ra kỹ thuật số và mức logic được đặt thành Cao, nếu không, nó có thể tạo ra các âm khác nhau theo tần số được tạo ra từ đầu ra Analog PWM được kết nối với nó . (lưu ý: dải tần mà tai người bình thường có thể phân biệt là từ 20 Hz đến 20kHz.)

**[Grove - Tilt Switch](https://www.seeedstudio.com/Grove-Tilt-Switch-p-771.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/Tilt.jpg)

Grove-Tilt Switch tương đương với một nút bấm và được sử dụng làm đầu vào kỹ thuật số. Bên trong tilt switch là một cặp 2 viên bi tiếp xúc với các chân khi vỏ thẳng đứng. Khi nghiêng các viên bi không tiếp xúc với các chân, do đó không tạo ra kết nối. Nó được nối với dòng SIG, NC không được sử dụng trên mô-đun Grove này.

**[Grove - Chainable RGB LED](https://www.seeedstudio.com/Grove-Chainable-RGB-Led-V2-0-p-2903.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/Grove-Chainable_RGB_LED_V2.0.jpg)


Grove - Chainable RGB LED dựa trên chip P9813 là full-color LED driver. Nó cung cấp 3 constant-current drivers cũng như đầu ra được điều chế 256 màu xám. Nó giao tiếp với MCU bằng cách sử dụng chuẩn giao tiếp 2 dây (Data và Clock). Chuẩn 2 dây này có thể được sử dụng để xếp tầng các mô-đun LED RGB - Chainable RGB. Việc tích hợp clock ở trong hệ thống giúp tăng khoảng cách truyền. Mô-đun Grove này phù hợp cho bất kỳ dự án nào dựa trên đèn LED đầy màu sắc.

**[Grove - Light Sensor](https://www.seeedstudio.com/Grove-Light-Sensor-v1-2-p-2727.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/lightsensor.jpg)

Cảm biến Grove - Light tích hợp một điện trở ảnh (điện trở phụ thuộc ánh sáng) để phát hiện cường độ ánh sáng. Điện trở của quang điện trở giảm khi cường độ ánh sáng tăng. Một chip OpAmp kép LM58 trên bo mạch tạo ra điện áp tương ứng với cường độ ánh sáng (tức là dựa trên giá trị điện trở). Tín hiệu đầu ra là giá trị tương tự, ánh sáng càng mạnh thì giá trị càng lớn.

**[Grove - Line Finder](https://www.seeedstudio.com/Grove-Line-Finder-v1-1-p-2712.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/linefinder.jpg)

Grove-Line finder được thiết kế cho robot dò đường. Nó có một đèn LED phát ra IR và một phototransistor nhạy IR. Nó có thể xuất tín hiệu số đến vi điều khiển để robot có thể đi theo một đường màu đen trên nền trắng hoặc ngược lại.

**[Grove - LCD RGB Backlight](https://www.seeedstudio.com/Grove-LCD-RGB-Backlight-p-1643.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/LCD.jpg)

Grove - LCD RGB Backlight này là màn hình LCD 16 x 2, nó sử dụng giao diện bus I2C để giao tiếp với board phát triển, do đó sẽ giảm số lượng pin headers từ 10 xuống còn 2, rất thuận tiện cho hệ thống Grove. Mô-đun hiển thị LCD này cũng hỗ trợ tùy chỉnh các ký tự, bạn có thể tạo và hiển thị biểu tượng trái tim hoặc hình người trên mô-đun LCD này thông qua cấu hình mã hóa đơn giản.

**[Grove - Temperature & Humidity Sensor(DHT11)](https://www.seeedstudio.com/Grove-Temperature-Humidity-Sensor-DHT1-p-745.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/DHT11.jpg)

Temperature & Humidity sensor này cung cấp đầu ra kỹ thuật số được hiệu chuẩn trước. Một phần tử cảm biến điện dung duy nhất đo độ ẩm tương đối và nhiệt độ được đo bằng nhiệt điện trở hệ số âm (NTC). Nó có độ tin cậy tuyệt vời và ổn định lâu dài. Xin lưu ý rằng cảm biến này sẽ không hoạt động ở nhiệt độ dưới 0 độ.

**[Grove - 3-Axis Digital Accelerometer](https://www.seeedstudio.com/Grove-3-Axis-Digital-Accelerometer-1-5-p-765.html)**
 


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis_cover.jpg)

3-Axis Digital Accelerometer là phần quan trọng trong các dự án như phát hiện định hướng, phát hiện cử chỉ và phát hiện chuyển động. 3-Axis Digital Accelerometer (± 1,5g) này dựa trên mô-đun tiêu thụ năng lượng thấp của Freescale, MMA7660FC. Nó có tính năng sống sót sốc cao tới 10.000g và các mẫu có thể định cấu hình trên mỗi giây. Đối với các ứng dụng hào không yêu cầu phạm vi đo quá lớn, đây là một lựa chọn tuyệt vời vì nó bền, tiết kiệm năng lượng và tiết kiệm chi phí.

## GETTING STARTED 

### Yêu cầu tối thiểu

- Grove starter kit
- Cáp micro USB 
- Máy tính với Arduino IDE

### Hướng dẫn cơ bản 

#### Thiết lập Arduino IDE 

**Bước 1.** Cài đặt driver USB sang serial cho Seeeduino Lotus v1.1

Seeeduino Lotus Phiên bản 1.1 trở lên tương thích với USB CP2102N to serial, nó hỗ trợ các hệ điều hành bao gồm Windows, MacOS và Linux, vui lòng tải xuống và cài đặt các driver có liên quan cho hệ điều hành của bạn.
Link tải xuống: 
Website chính thức: [CP210x USB to UART Bridge VCP Drivers](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers)


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/logo.jpg)

**Cài đặt driver**

Windows:

Giải nén tệp driver đã tải xuống, mở tệp được giải nén và chọn cài đặt trình điều khiển có liên quan theo bit của hệ điều hành của bạn, trong trường hợp này, chúng tôi đã chọn 64bit, người dùng hệ điều hành 32 bit nên chọn tệp _x86, làm theo trình hướng dẫn cài đặt để cài đặt.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/win1.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/win2.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/win3.png)

Mac OS:

Nhấp đúp vào tập tin VCP Driver.pkg của Silicon Silicon Labs và làm theo trình hướng dẫn cài đặt.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/mac1.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/mac2.png)

**Bước 2.** Tải xuống và cài đặt [Arduino IDE](https://www.arduino.cc/en/Main/Software)

Vui lòng tải xuống và cài đặt Arduino IDE theo hệ điều hành của bạn.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard.png)

<b id="step3">Bước 3.</b> Add library for Seeeduino Lotus

- Mở Arduino | Preferences, từ cửa sổ tùy chọn bên dưới trang cài đặt, tìm Additional Boards Manager URLS, copy & paste Library URL vào hộp văn bản, sau đó nhấn ok để có hiệu lực.
Library URL:	https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/package_seeeduino_boards_index.json

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard1.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard2.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard3.png)

- Công Tools | Board: | Boards Manager, tìm kiếm Seeeduino AVR và ấn vào cài đặt để cài đặt thư viện Seeeduino AVR. nếu bạn không thể thấy Seeeduino AVR được liệt kê trong cửa sổ Boards Manager, vui lòng lặp lại bước đầu tiên và đảm bảo URL bạn đã nhập là chính xác.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard4.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard5.png)

- Công cụ Tools | Board: trong danh sách phụ, bạn nên tìm phần Seeeduino AVR Boards như được hiển thị và vui lòng chọn đúng board theo môi trường phát triển của bạn, trong hướng dẫn này, chúng ta nên chọn Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard6.png)
	
**Bước 4.** Kết nối Seeeduino Lotus

Vui lòng kết nối Seeeduino Lotus và máy tính thông qua cáp Micro-USB, đèn LED nguồn màu xanh lá cây trên Seeeduino sẽ sáng lên.


![with micro-USB](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/usb.jpg)

**Bước 5.** Cấu hình IDE cho Seeeduino Lotus

Vui lòng làm theo các bước như được hiển thị trước đó, chọn Lotus Seeeduino Lotus dưới Boards Manager.

Chọn thiết bị nối tiếp của bo mạch Arduino từ Tools | Serial Port. Để tìm ra thiết bị kết nối serial chính xác, bạn có thể ngắt kết nối board Arduino của mình và mở lại menu; mục board Arduino nên bị mất đi. Kết nối lại board và chọn cổng nối tiếp đó. Mục bạn đã chọn nên có “SLAB_USB”.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard07.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard7.png)


Đặt “Tools | Programmer” là “AVR ISP”.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard8.png)


### Blink Demo

Sau khi đã thiết lập Arduino IDE, giờ đây chúng ta có thể thử nghiệm đoạn code demo nhấp nháy LED Seeeduino Lotus development board. Lưu ý: Bạn nên hoàn thành các bước trên để tiếp tục những điều sau.

**Chọn Blink Demo từ Menu**

Chọn File | Examples | 01 Basics | Blink từ thanh menu, blink example code sẽ xuất hiện trong của sổ mới. 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard9.png)


**Upload code**

Vui lòng đảm bảo Board, Port và Programer được chọn chính xác trong menu công cụ.
Bây giờ chúng ta có thể tải mã lên Lotus dev board bằng cách nhấn biểu tượng mũi tên phải ở góc trên cùng bên trái của IDE


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard10.png)

Sau khi mã được tải lên thành công, dòng chữ “avrdude done. Thank you." sẽ xuất hiện trong cửa sổ log của IDE.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard11.png)

Bây giờ bạn sẽ thấy đèn LED tích hợp nhấp nháy trong khoảng thời gian một giây.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/blink.jpg)


**Giải thích về blink code**

void setup() là chức năng thiết lập chỉ chạy một lần khi bạn nhấn reset hoặc cấp nguồn cho bo mạch.

```C

void setup() {
}

```

khởi tạo pin kỹ thuật số LED_BUILTIN làm đầu ra.

```C

pinMode(LED_BUILTIN, OUTPUT);

```

void loop() là hàm vòng lặp chạy đi chạy lại mãi mãi.


```C

void loop() {
}

```

digitalWrite() là hàm đặt chân LED_BUILTIN làm mức điện áp HIGH, có nghĩa là bật đèn LED. Tương tự để tắt đèn LED, chỉ cần đặt mức điện áp thành LOW bằng cách thay đổi mã HIGH thành LOW.

```C

digitalWrite(LED_BUILTIN, HIGH);
digitalWrite(LED_BUILTIN, LOW);

```

delay() có nghĩa là tạm dừng chương trình, số bên trong dấu ngoặc có nghĩa là lượng thời gian (tính bằng mili giây) để tạm dừng (độ trễ).

```C

delay(1000);

```




## 10 bài hướng dẫn với Grove Starter Kit 


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/kit.jpg)

### Mục tiêu
Phần này bao gồm 10 hướng dẫn, các hướng dẫn có thể được chia thành hai phần, 8 phần đầu tiên giới thiệu hoạt động cơ bản của từng mô-đun riêng lẻ từ starter kit và 2 phần cuối sử dụng các ví dụ để hiển thị cách kết hợp các mô-đun và áp dụng trong các ứng dụng thực tế.


### Điều kiện tiên quyết

Kiến thức cơ bản về Seeeduino Lotus với Arduino IDE và kỹ năng lập trình là điều cần thiết cho hướng dẫn này. Do đó, vui lòng đảm bảo bạn đã hoàn thành hướng dẫn thiết lập cơ bản ở trên và cài đặt thành công USB to serial driver trên hệ điều hành cho Seeeduino Lotus, hoàn thành bản demo Blink LED và đảm bảo nó hoạt động hoàn toàn với Seeeduino Lotus board.

### Kết quả học tập

- Có thể sử Arduino IDE để lập trình cho Seeeduino Lotus v1.1 để điều khiển các mô-đun từ Grove Starter Kit.
- Có thể xác định loại mô-đun có trong Bộ công cụ này và các ứng dụng của chúng.
- Có thể trình diễn từng thành phần của Grove Starter Kit và sử dụng mô-đun có liên quan cho các dự án của riêng bạn sau hướng dẫn này

### Phần 1: Grove - Buzzer


![](https://raw.githubusercntent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer.jpg)

**Mục tiêu**	

Sử dụng bộ rung để tạo ra một số tiếng ồn và cũng đặt tần số cụ thể để tạo ra một số âm.

**Kiến thức chính**

- Mô-đun Buzzer là một thiết bị truyền động.
- Sử dụng tín hiệu số để tạo tiếng ồn
- Tạo âm cụ thể bằng cách đặt tần số phù hợp
- Sử dụng chức năng âm (pin, tần số, thời lượng) để tạo tiếng chuông phát nhạc
- Tìm hiểu cách sử dụng vòng lặp "for loop" trong Arduino IDE


**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và đã được cài đặt serial-to-USB driver


Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove - mô-đun Buzzer


**Kết nối phần cứng**

**Bước 1.** Vui lòng sử dụng cáp Grove để kết nối mô-đun Grove - Buzzer với cổng D6 của Seeeduino Lotus

![D6 with seeeduino](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer_ard.jpg)

**Bước 2.** Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB.

**Lập trình phần mềm**	

**Ví dụ 1**:Sử dụng logic kỹ thuật số high / low để tạo tiếng vang "buzz"

Bước 1: Copy & Paste đoạn code sau vào Arduino IDE

```
//assign buzzer as pin 6
#define buzzer 6

void setup()
{
  //set buzzer as output
  pinMode(buzzer, OUTPUT);
}

void loop()
{ //turn on buzzer(set logic level high)
  digitalWrite(buzzer, HIGH);
  //wait 1s
  delay(1000);
  //turn off buzzer(set logic level low)
  digitalWrite(buzzer, LOW);
  //wait 1s
  delay(1000);
}

```
Bước 2: Nạp code lên Seeeduino Lotus

Bước 3: Quan sát kết quả

!!!Thành công
	Khi code đã được hoàn tất tải lên, bạn có thể nghe thấy tiếng "buzz" với khoảng cách 1 giây ở giữa các âm thanh.

**Ví dụ 2**:Sử dụng tần số khác nhau để làm cho tiếng chuông tạo ra âm thanh khác nhau.

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//assign buzzer as pin 6 
#define buzzer 6                

void setup()
{
  /* tone(pin, frequency, duration) */
  //set buzzer pin to play 264Hz for 300ms
  tone(buzzer, 262, 300);
  //wait 1s
  delay(1000);

  //set buzzer pin to play 297Hz for 300ms
  tone(buzzer, 294, 300);
  //wait 1s
  delay(1000);

  //set buzzer pin to play 330Hz for 300ms
  tone(buzzer, 330, 300);
  //wait 1s
  delay(1000);
}

void loop()
{
  // no need to repeat the tone.
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

!!!Thành công
	Khi code được hoàn tất tải lên, bạn sẽ nghe thấy tiếng chuông đang phát ra âm thanh của “Do、 Re、 Mi.

**Ví dụ 3**:Sử dụng chức năng âm (pin, tần số, thời lượng) để tạo nhạc từ bộ rung

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C++

// initalise the frequency of the notes
#define NOTE_A4  440
#define NOTE_AS4 466
#define NOTE_C4  262
#define NOTE_D4  294
#define NOTE_E4  330
#define NOTE_F4  349
#define NOTE_G4  392
#define NOTE_C5  523

//assign buzzer as pin 6
#define buzzer 6

// notes in the melody:
int melody[] = {
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_F4, NOTE_E4,
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_G4, NOTE_F4,
  NOTE_C4, NOTE_C4, NOTE_C5, NOTE_A4, NOTE_F4, NOTE_E4, NOTE_D4,
  NOTE_AS4, NOTE_AS4, NOTE_A4, NOTE_F4, NOTE_G4, NOTE_F4
};

// note durations: 4 = quarter note, 8 = eighth note, etc.:
int noteDurations[] = {
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 4, 4,
  8, 8, 4, 4, 4, 2,
};

void setup() {
  // iterate over the notes of the melody:
  for (int thisNote = 0 ; thisNote < 25 ; thisNote++) {

    // to calculate the note duration, take one second divided by the note type.
    //e.g. quarter note = 1000 / 4, eighth note = 1000/8, etc.
    int noteDuration = 1000 / noteDurations[thisNote];
    tone(buzzer, melody[thisNote], noteDuration);

    // to distinguish the notes, set a minimum time between them.
    int pauseBetweenNotes = noteDuration * 1.30;
    delay(pauseBetweenNotes);
    noTone(buzzer);
  }
}

void loop() {
  // no need to repeat the melody.
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

!!!thành công
	Khi mã kết thúc tải lên, bạn sẽ nghe thấy một giai điệu từ bộ rung.

**Khám phá thêm**

Vui lòng checkout repo Brett Hagman từ GitHub "[Giai điệu] (https://github.com/bhagman/Tone)" để tạo âm và nhạc.

### Phần 2: Grove - Tilt Switch



![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/Tilt.jpg)

**Mục tiêu**	
Sử dụng mô-đun tilt switch để bật / tắt đèn LED tích hợp trên Seeeduino Lotus, đồng thời sử dụng tilt switch để làm cho mô-đun buzzer từ phần trước chuyển sang buzz.

**Kiến thức chính**


- Tilt Switch là một mô-đun đầu vào tín hiệu
- Thao tác trên tilt switch
- Sử dụng chức năng digitalRead (pin) nhận tín hiệu logic đầu vào từ tilt switch là HIGH để bật và LOW khi tắt.
- if (condition) {} other {} hàm và toán tử so sánh như! = (không bằng), <(nhỏ hơn), <= (nhỏ hơn hoặc bằng), == (bằng),> (lớn hơn hơn) và> = (lớn hơn hoặc bằng).

**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit:

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove – Tilt Switch
- Grove – Buzzer
	
**Kết nối phần cứng**

Bước 1: Kết nối Grove - Tilt Switch sang cổng D5 của Seeeduino Lotus.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/tilt_ard.jpg)


Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB


**Lập trình phần mềm**	
**Ví dụ 1**:Quan sát hành vi của tilt switch bằng cách sử dụng Serial Monitor

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//assign name tiltswitchPin to pin 5
#define tiltswitchPin 5
//creates a integer variable called 'val' to store read value
int val;

void setup()
{
  //set pinMode of tiltswitchPin to input
  pinMode(tiltswitchPin, INPUT);
  // opens serial port, sets data rate to 9600 bps
  Serial.begin(9600);
}

void loop()
{ //read the tilt switch input
  val = digitalRead(tiltswitchPin);
  //display the tilt switch status, 1 is on, 0 is off.
  Serial.println(val);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Mở Serial Monitor

để mở serial monitor, vui lòng chọn Tools | Serial Monitor từ thanh menu hoặc chỉ cần nhấp vào biểu tượng kính lúp trên thanh công cụ. Lưu ý: Vui lòng đợi đoạn code được tải lên trước khi mở serial monitor

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard12.png)

Bước 4: Quan sát kết quả

Vui lòng nghiêng tilt switch theo cả hai hướng, bạn sẽ thấy hình 1 1 hoặc hoặc 0 0 được hiển thị trong serial monitor, bây giờ bạn có thể tìm thấy hướng thích hợp cho tilt switch để bật / tắt.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/tilt_off&on.jpg)


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard13.png)

**Ví dụ 2**:Sử dụng tilt switch để bật / tắt đèn LED tích hợp

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//set title of pin 5 as tiltSwitch
#define tiltSwitch 5

void setup()
{ //set pin 5(tilt switch) as input pin
  pinMode(tiltSwitch, INPUT);
  //set pin 13(Builtin LED) as output pin
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{ //read the status of tilt switch
  if (HIGH == digitalRead(tiltSwitch)) {
    /*
       if the logic level of tilt switch
       is high turn on the builtin LED
    */
    digitalWrite(LED_BUILTIN, HIGH);
  } else
  {
    //otherwise turn off the builtin LED
    digitalWrite(LED_BUILTIN, LOW);
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả
!!!Thành công
	Bây giờ bạn sẽ có thể bật / tắt đèn LED tích hợp trên Seeeduino Lotus bằng cách nghiêng tilt switch theo đúng hướng.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/tilt_off&on.jpg)


**Ví dụ 3**: Sử dụng tilt switch để tạm dừng và phát nhạc chuông từ buzzer
Vui lòng kết nối mô-đun Grove - Buzzer với cổng D6 của Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer_tilt.jpg)

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

// initalise the frequency of the notes
#define NOTE_A4  440
#define NOTE_AS4 466
#define NOTE_C4  262
#define NOTE_D4  294
#define NOTE_E4  330
#define NOTE_F4  349
#define NOTE_G4  392
#define NOTE_C5  523

// notes in the melody:
int melody[] = {
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_F4, NOTE_E4,
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_G4, NOTE_F4,
  NOTE_C4, NOTE_C4, NOTE_C5, NOTE_A4, NOTE_F4, NOTE_E4, NOTE_D4,
  NOTE_AS4, NOTE_AS4, NOTE_A4, NOTE_F4, NOTE_G4, NOTE_F4
};

// note durations: 4 = quarter note, 8 = eighth note, etc.:
int noteDurations[] = {
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 4, 4,
  8, 8, 4, 4, 4, 2,
};

//set title of pin 5 as tiltSwitch
#define tiltSwitch 5
//set title of pin 6 as buzzer
#define buzzer 6
// set variable currentNote to store latest note played
int currentNote;

void setup()
{
  //set pin 5(tilt switch) as input pin
  pinMode(tiltSwitch, INPUT);
}

void loop()
{
  /*read the status of tilt switch
if the logic level of tilt switch
is high, start play music */
  if (HIGH == digitalRead(tiltSwitch)) {

for (int thisNote = currentNote ; thisNote < 25 ; thisNote++) {
  // to calculate the note duration, take one second divided by the note type.
  //e.g. quarter note = 1000 / 4, eighth note = 1000/8, etc.
  int noteDuration = 1000 / noteDurations[thisNote];
  tone(buzzer, melody[thisNote], noteDuration);

  // to distinguish the notes, set a minimum time between them.
  int pauseBetweenNotes = noteDuration * 1.30;
  delay(pauseBetweenNotes);

  /*reset the currentNote to the 0
is the music is finished*/
  if (thisNote >= 24) {
currentNote = 0;
  }

  /*druing the music read the status
of tilt switch if the logic level
of tilt switch is LOW, stop play
music and store the previous played
tone and jump to next tone*/
  if (LOW == digitalRead(tiltSwitch)) {

//store the current note(thisNote) to currentNote
currentNote = thisNote;
//set the next note ready to play by increase currentNote by 1 increament
currentNote ++;
/*reset the currentNote to the beginning
  is the music is finished*/
if (currentNote >= 25)
{
  //restart the music from beginning by reset the currentNote to 0,
  currentNote = 0;
}
//if the tilt switch is set to logic level low, stop play music
break;
  }
}
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

!!!Thành công
	Bây giờ bạn có thể tạm dừng nhạc chuông bằng cách nghiêng tilt switch sang vị trí tắt và tiếp tục âm nhạc bằng cách nghiêng tilt switch sang vị trí bật.

**Khám phá thêm**

Sau phần này, bạn có thể gắn mô-đun cảm biến tilt switch vào nắp hộp công cụ, vì vậy khi bạn nhấc nắp, kích hoạt tilt switch để bật, sau đó bạn có thể đặt độ trễ trong một khoảng thời gian ngắn để kích hoạt chuông để tạo một số âm báo. nhắc nhở bạn nắp vẫn mở, vì vậy bạn sẽ không quên đóng nắp sau khi sử dụng xong hộp công cụ.

### Phần 3: Grove – Chainable RGB LED

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/Grove-Chainable_RGB_LED_V2.0.jpg)

**Mục tiêu**	

Sử dụng code để điều khiển đèn chainable RGB LED để hiển thị màu khác nhau và chuyển đổi giữa các màu bằng cách sử dụng tilt switch.

**Kiến thức chính**

- Grove - LED RGB Chainable là một thiết bị truyền động
- Import thư viện cho mô-đun grove
- Sử dụng hàm setColorHSB () để kiểm soát màu sắc, độ bão hòa và độ sáng của mô-đun LED
- Sử dụng hàm setColorRGB () để kiểm soát màu sắc và độ sáng của mô-đun LED
- Sử dụng % (modulo) operation để tìm số dư, ví dụ: 5% 2 = 1, 9% 3 = 0.
- Sử dụng switch (val). function


**Yêu cầu phần cứng**	

Tự chuẩn bị

- cáp micro-USB
- máy tính có Arduino IDE và được cài đặt serial-to-USB driver 

Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove – Chainable RGB LED
- Grove – Tilt Switch
- Grove – Buzzer


**Kết nối phần cứng**

Bước 1: Kết nối Grove – Chainable RGB LED với cổng D7 của Seeeduino Lotus, Lưu ý: vui lòng kết nối cổng G | V | DI | CI từ đèn LED như hình dưới đây.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_ard.jpg)

Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB.


**Lập trình phần mềm**

**Thêm thư viện**

Các bước bên dưới hiển thị cách thêm [thư viện](https://github.com/pjpmarques/ChainableLED/archive/v1.2.zip) cho Grove – Chainable RGB LED.

Bước 1: Mở kho Github repository từ Library URL và tải xuống file zip

Vui lòng tìm “Clone or download | Download ZIP” từ trang Github, bạn phải chọn Download ZIP và vui lòng nhớ đường dẫn tệp mà bạn đã tải xuống và lưu tệp zip.

Bước 2: Chọn “include Library | Add .ZIP Library..

Mở Sketch | Include Library | Add .ZIP Library…, trong cửa sổ bật lên mới, chọn tệp zip bạn đã tải xuống ở bước trước, sau đó nhấp vào choose.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard14.png)


Bước 3: Kiểm tra xem thư viện đã thêm thành công chưa

Chọn và mở File | Examples | ChainableLED-1.2 | CycleTroughColors

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/ard15.png)

Nạp code: Chọn "upload the code"

!!!Thành công
 	nếu mô-đun LED đang chuyển qua các màu khác nhau, tức là bạn đã tải Thư viện thành công.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_flash_8.jpg)

Kết luận: Phương thức thêm thư viện cho phép người dùng dễ dàng thêm driver cảm biến của bên thứ ba và thư viện được tạo bởi người bán mô-đun cảm biến, ví dụ, trong phần hướng dẫn này, chúng tôi đã sử dụng hàm setColorRGB (byte led, byte red, byte green, byte blue) là một trong những thực hiện chức năng bởi Seeed Studio, điều này giúp giảm công sức của người dùng khi họ phát triển mô-đun cảm biến mới. Bạn sẽ cần thêm nhiều thư viện cho các mô-đun Grove khác sau này.

**Ví dụ 1**:Sử dụng hàm setColorHSB để thay đổi màu đèn LED

Buớc 1: copy & paste đoạn code sau vào Arduino IDE

```C++

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

void setup()
{
  //initialise ChainableLED leds
  leds.init();
}
//initialise hue as float point with value of 0.0
float hue = 0.0;
//initialise up as boolean with value of true
boolean up = true;

void loop()
{
  /*for loop is used for loop through
    each LED connected to the chain
    in this case there is only one LED
  */
  for (byte i = 0; i < NUM_LEDS; i++) {

    /*setColorHSB(byte led, float hue, float saturation, float brightness);
       in this case set the first and only chainableLED 0 with changing hue
       and full saturation and half brightness
    */
    leds.setColorHSB(i, hue, 1, 0.5);
    //    delay for 50ms for each color
    delay(50);

    /*if up is true increase
      hue at 0.025 interval
      otherwise decrease hue
      at 0.025 interval
    */
    if (up) {
      hue += 0.025;
    }
    else
    {
      hue -= 0.025;
    }
    /*
      if hue is greater than 1.0
       and up is true set up to false,
       otherwise if hue is less or
       equal to 0.0 and up is not
       ture(! means is not) set up
       to true
    */
    if (hue >= 1.0 && up)
    {
      up = false;
    }
    else if (hue <= 0.0 && !up)
    {
      up = true;
    }
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn sẽ thấy màu sắc của đèn LED thay đổi theo giá trị của hue khi nó tăng thêm 0,025 và khi giá trị hue đạt 1, giá trị hue sẽ giảm 0,025 cho đến khi giá trị trở thành 0 và mỗi màu sẽ sáng 50 mili giây.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_flash_8.jpg)

**Ví dụ 2**:Sử dụng hàm setColorRGB để thay đổi màu sắc và độ sáng của đèn LED

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C++

/*
   Example of using the ChainableRGB library for controlling a Grove RGB.
   This code fades in an out colors in a strip of leds.
*/

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

void setup()
{
  //initialise ChainableLED leds
  leds.init();
}
//initialise power as byte with value of 0
byte power = 0;

void loop()
{
  /*for loop is used for loop through
    each LED connected to the chain
    in this case there is only one LED
  */
  for (byte i = 0; i < NUM_LEDS; i++)
  {
    /*
      % means modulo operation to find remainder
      eg 0 % 2 = 0, 1 % 2 = 1,  2 % 2 = 0...
      setColorRGB(byte led, byte red, byte green, byte blue);
      so in this case the even number of the LED chain
      will fading green color, odd number of the LED
      chain will fading red color, since we count the
      first LED as 0.
    */
    if (i % 2 == 0)
      //brighter red color from 0 to full power
      leds.setColorRGB(i, power, 0, 0);
    else
      //dimmer green color from full power to 0
      leds.setColorRGB(i, 0, 255 - power, 0);
  }
  //set power increment as 10
  power += 10;
  //light 0.5s for each brightness
  delay(500);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

bạn sẽ thấy đèn LED màu đỏ tăng độ sáng trong mỗi 0,5 giây, bởi vì chúng ta chỉ đặt giá trị cho biến màu đỏ trong hàm setColorRGB (byte led, byte red, byte green, byte blue).

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_eg2.jpg)

Nếu chúng ta thay đổi cả hai biến màu đỏ và màu xanh lá cây từ đây:

```C
leds.setColorRGB(i, power, 0, 0);
```

trở thành:

```C
leds.setColorRGB(i, power, 255-power, 0);
```

Vui lòng quan sát sự khác biệt

**Ví dụ 3**:Sử dụng tilt switch để điều khiển LED và Buzzer

Kết nối Grove – Tilt Switch đến cổng D5 của Seeeduino Lotus.

Kết nối mô-đun Grove – Buzzer đến cổng D6 của Seeeduino Lotus.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_buzzer_tilt.jpg)

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

// initalise the frequency of the notes
#define NOTE_A4  440
#define NOTE_AS4 466
#define NOTE_C4  262
#define NOTE_D4  294
#define NOTE_E4  330
#define NOTE_F4  349
#define NOTE_G4  392
#define NOTE_C5  523

// notes in the melody:
int melody[] = {
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_F4, NOTE_E4,
  NOTE_C4, NOTE_C4, NOTE_D4, NOTE_C4, NOTE_G4, NOTE_F4,
  NOTE_C4, NOTE_C4, NOTE_C5, NOTE_A4, NOTE_F4, NOTE_E4, NOTE_D4,
  NOTE_AS4, NOTE_AS4, NOTE_A4, NOTE_F4, NOTE_G4, NOTE_F4
};

// note durations: 4 = quarter note, 8 = eighth note, etc.:
int noteDurations[] = {
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 2,
  8, 8, 4, 4, 4, 4, 4,
  8, 8, 4, 4, 4, 2,
};

//set title of pin 5 as tiltSwitch
#define tiltSwitch 5
//set title of pin 6 as buzzer
#define buzzer 6

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

// set variable currentNote to store latest note played
int currentNote;
//initialise hue as float point with value of 0.0
float hue = 0.0;
//initialise up as boolean with value of true
boolean up = true;
//initialise power as byte with value of 0
byte power = 0;
//initialise color as integer with value of 0
int color = 0;

void setup()
{
  //set pin 5(tilt switch) as input pin
  pinMode(tiltSwitch, INPUT);
  //initialise ChainableLED leds
  leds.init();
}

void loop()
{
  /*read the status of tilt switch
    if the logic level of tilt switch
    is high, start play music */
  if (HIGH == digitalRead(tiltSwitch)) {

    for (int thisNote = currentNote ; thisNote < 25 ; thisNote++) {
      // to calculate the note duration, take one second divided by the note type.
      //e.g. quarter note = 1000 / 4, eighth note = 1000/8, etc.
      int noteDuration = 1000 / noteDurations[thisNote];
      tone(buzzer, melody[thisNote], noteDuration);

      // to distinguish the notes, set a minimum time between them.
      int pauseBetweenNotes = noteDuration * 1.30;
      delay(pauseBetweenNotes);

      /*reset the currentNote to the 0
        is the music is finished*/
      if (thisNote >= 24) {
        currentNote = 0;
      }

      /*set the LED to loop through
        different colors with different hue*/
      leds.setColorHSB(0, hue, 1, 0.5);

      /*if up is true increase
        hue at 0.025 interval
        otherwise decrease hue
        at 0.025 interval
      */
      if (up) {
        hue += 0.025;
      }
      else
      {
        hue -= 0.025;
      }
      /*if hue is greater than 1.0
         and up is true set up to false,
         otherwise if hue is less or
         equal to 0.0 and up is not
         ture(! means is not) set up
         to true
      */
      if (hue >= 1.0 && up)
      {
        up = false;
      }
      else if (hue <= 0.0 && !up)
      {
        up = true;
      }

      /*druing the music read the status
        of tilt switch if the logic level
        of tilt switch is LOW, stop play
        music and store the previous played
        tone and jump to next tone*/
      if (LOW == digitalRead(tiltSwitch)) {
        /* use switch...case to set the LED loop through three colors
           Red when color = 0 enters case 0
           Green when color = 1 enters case 1
           Blue when color = 2 enters case 2
           reset color to 0 if color is greater or equals 3
        */
        if (color >= 3) {
          color = 0;
        }
        switch (color) {
          case 0:
            //set LED to Red
            leds.setColorRGB(0, 255, 0, 0);
            break;
          case 1:
            //set LED to Green
            leds.setColorRGB(0, 0, 255, 0);
            break;
          case 2:
            //set LED to Blue
            leds.setColorRGB(0, 0, 0, 255);
            break;
        }
        //increase color by 1 increment everytime enter this condition
        color ++;

        //store the thisNote to currentNote
        currentNote = thisNote;
        //set the next note ready to play by increase currentNote by 1 increament
        currentNote ++;
        /*reset the currentNote to the beginning
          is the music is finished*/
        if (currentNote >= 25)
        {
          //restart the music from beginning by reset the currentNote to 0,
          currentNote = 0;
        }
        //if the tilt switch is set to logic level low, stop playing music
        break;
      }
    }
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quán sát kêt quả

Bằng cách nghiêng tilt switch, bạn sẽ thấy khi bật tilt switch, đèn LED đổi màu cùng với âm báo thay đổi, khi tắt tilt switch, đèn LED sẽ chuyển qua màu Đỏ, Xanh lục và Xanh lam và chuông dừng.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/rgb_eg3.jpg)



**Khám phá thêm**

Sau phần này, bây giờ bạn có thể kết hợp các mô-đun từ ba phần đầu tiên và biến thành hộp quà sinh nhật, nơi bạn có thể đặt cảm biến tilt switch trên nắp hộp, tại thời điểm hộp được mở, tilt switch được kích hoạt, sau đó còi bắt đầu phát bài hát sinh nhật và đèn LED bắt đầu nhấp nháy đèn nhiều màu sắc.

### Phần 4: Grove - Light Sensor

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/lightsensor.jpg)

**Mục tiêu**	

Sử dụng mô-đun cảm biến ánh sáng để bật / tắt mô-đun chainable RGB LED và kiểm soát độ sáng của đèn LED theo cường độ ánh sáng xung quanh.

**Kiến thức chính**

- Mô-đun cảm biến ánh sáng là mô-đun đầu vào tín hiệu Analog
- Sử dụng hàm map (value, fromLow, fromHigh, toLow, toHigh) để ánh xạ lại số lượng đầu ra Analog từ phạm vi này sang phạm vi khác.
- Sử dụng cảm biến ánh sáng như một công tắc đèn
- Sử dụng cảm biến ánh sáng để điều khiển độ sáng LED bằng cách cảm nhận độ sáng xung quanh

**Yêu cầu phần cứng**	

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit:

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove – Light Sensor
- Grove – Chainable RGB LED


**Kết nối phần cứng**

Bước 1: Kết nối mô-đun Grove – Light Sensor với cổng A0 của Seeeduino Lotus

Bước 2: Kết nối Grove – Chainable RGB LED với cổng D7 của Seeeduino Lotus

Bước 3: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/light_rgb.jpg)

**Lập trình phần mềm**

**Ví dụ 1**: Sử dụng cảm biến ánh sáng để bật / tắt đèn LED bằng độ sáng của ánh sáng xung quanh

Buớc 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED, set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

//naming analog pin A0 as LightSensor
#define LightSensor A0

void setup()
{
  //initialise ChainableLED leds
  leds.init();
}

void loop()
{
  //read the value of Light Sensor and store to value
  int value = analogRead(LightSensor);
  //if Sensor reading is less than 150 turn on LED
  if (value < 150) {
    //turn on LED
    leds.setColorRGB(0, 10, 10, 10);
    //delay for 1s
    delay(1000);
  } else
  {
    //turn off LED
    leds.setColorRGB(0, 0, 0, 0);
    //delay for 1s
    delay(1000);
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Lưu ý nếu có ánh sáng xung quanh, bạn có thể dùng tay để che mô-đun cảm biến ánh sáng, sau đó đèn LED sẽ bật. Khi ánh sáng xung quanh làm cho giá trị đọc của cảm biến ánh sáng cao hơn 150, đèn LED sẽ tắt.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/light_eg1.jpg)

**Ví dụ 2**: Sử dụng cảm biến ánh sáng để kiểm soát độ sáng của đèn LED

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

#define LightSensor A0

void setup()
{
  //initialise ChainableLED leds
  leds.init();
  Serial.begin(9400);
}

//initialise hue as float point with value of 0.0
float hue = 0.0;
//initialise up as boolean with value of true
boolean up = true;

void loop()
{
  //read the value of Light Sensor and store to value
  int value = analogRead(LightSensor);
  /*map(value, fromLow, fromHigh, toLow, toHigh)
    Re-maps a number from one range to another
    In this case maping the analog value of light sensor
    ranging from 0-800 to 100-0, so when the brightness
    of surrounding enviroment is high so the sensor reading
    value is high, therefore the maped value should be opposite,
    so the birghtness LED should be dimmer.
    the brightness of chainable LED only accept float number, so
    we divide the maped value with 100. 
  */
  float value_float = map(value, 0, 800, 50, 0) / 100.0;
  /*setColorHSB(byte led, float hue, float saturation, float brightness);
   * use the maped value(value_float) as brightness
  */
  leds.setColorHSB(0, hue, 1, value_float);
  delay(100);

  /*if up is true increase
    hue at 0.025 interval
    otherwise decrease hue
    at 0.025 interval
  */
  if (up) {
    hue += 0.025;
  }
  else
  {
    hue -= 0.025;
  }
  /*if hue is greater than 1.0
     and up is true set up to false,
     otherwise if hue is less or
     equal to 0.0 and up is not
     ture(! means is not) set up
     to true
  */
  if (hue >= 1.0 && up)
  {
    up = false;
  }
  else if (hue <= 0.0 && !up)
  {
    up = true;
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Độ sáng của đèn LED sẽ giảm khi cường độ sáng của môi trường xung quanh tăng. Khi cường độ sáng xung quanh giảm, độ sáng của đèn LED sẽ tăng. Như được hiển thị, đèn LED mờ khi có ánh sáng chói trên cảm biến ánh sáng, nếu không thì đèn LED sáng.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/light_eg2.jpg)

**Khám phá thêm**

Bây giờ bạn có thể tích hợp mô-đun cảm biến ánh sáng này vào hệ thống chiếu sáng hành lang để kiểm soát độ sáng của ánh sáng, vào ban ngày, cảm biến ánh sáng phát hiện ánh sáng mặt trời sau đó làm giảm độ sáng của ánh sáng hành lang xuống thấp, không chỉ tiết kiệm điện mà còn kéo dài tuổi thọ của các bóng đèn


### Phần 5: Grove - Line Finder

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/linefinder.jpg)

**Mục tiêu**	

Sử dụng line finder để phát hiện đường có màu đen và kiểm soát màu của đèn LED phù hợp khi line finder phát hiện đường có màu đen hay không.

**Kiến thức chính**

- Grove - Line Finder là một mô-đun đầu vào tín hiệu kỹ thuật số
- Xem lại về cách sử dụng  Serial Monitor
- Sử dụng mô-đun đầu vào tín hiệu để điều khiển Grove – Chainable RGB LED

**Yêu cầu phần cứng**	

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit
  
- Grove – Line Finder
- Grove – Chainable RGB LED

**Kết nối phần cứng**

Bước 1: Kết nối mô đun Grove - Line Finder với cổng D3 của Seeeduino Lotus

Bước 2:  Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB 

 ![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/line_ard.jpg)

**Lập trình phần mềm**

**Ví dụ 1**:Sử dụng Serial Monitor để hiển thị và kiểm tra tín hiệu đầu ra từ line finder

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//naming pin3 as singalPin
#define signalPin 3

void setup() {
  // initialize the digital pin as an input:
  pinMode(signalPin, INPUT);
  // opens serial port, sets data rate to 9600 bps
  Serial.begin(9600);
}

void loop() {
  //read the line detector input 
  int val = digitalRead(signalPin);
  
  //display the line detector status, 1 is black, 0 is white.
  Serial.println(val);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Lưu ý, bạn nên giữ khoảng cách ít nhất 5cm cho đối tượng cần phát hiện bằng line finder, để kiểm tra line finder, bạn nên băng một dải băng đen lên giấy trắng hoặc gạch (hoặc sử dụng vật màu đen). Bây giờ, hướng line finder vào đối tượng màu đen, Serial Monitor sẽ hiển thị 0 và nếu bạn di chuyển công cụ tìm dòng khỏi đối tượng màu đen, Serial Monitor sẽ hiển thị 1.

 ![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/line_eg1_1.jpg) 



**Ví dụ 2**:Sử dụng Line detector để bật hoặc tắt mô-đun LED RGB - Chainable.

Kết nối Grove – Chainable RGB LED với cổng D7 của Seeeduino Lotus

 ![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/line_rgb.jpg)

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

//naming pin3 as lineFinder
#define lineFinder 3

void setup() {
  // initialize the digital pin as an input:
  pinMode(lineFinder, INPUT);
  //initialise ChainableLED leds
  leds.init();
}

void loop() {
  /*read the line detector input
   * if detected black(HIGH) turn on LED
  */
  if (HIGH == digitalRead(lineFinder))
  {
    //turn off LED
    leds.setColorRGB(0, 10, 10, 10);
  }
  
  /*read the line detector input
   * if reading Logic low turn off LED
  */
  if (LOW == digitalRead(lineFinder))
  {
    //turn off LED
    leds.setColorRGB(0, 0, 0, 0);
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn sẽ thấy rằng nếu line finder phát hiện dòng màu đen, đèn LED sẽ tắt, nếu không, đèn LED sẽ bật lên nếu line finder không thể phát hiện dòng màu đen.

 ![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/line_eg2.jpg)
 

**Ví dụ 3**:Sử dụng line finder để điều khiển đèn LED phát ra màu Đỏ hoặc Xanh lá cây

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add ChainableLED library to this project
#include <ChainableLED.h>

//set the number of leds linked to the chain
#define NUM_LEDS  1

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

//naming pin3 as lineFinder
#define lineFinder 3

void setup() {
  // initialize the digital pin as an input:
  pinMode(lineFinder, INPUT);
  //initialise ChainableLED leds
  leds.init();
}

void loop() {
  /*read the line detector input
   * if detected black(HIGH) set Green LED
  */
  if (HIGH == digitalRead(lineFinder))
  {
    //Green LED
    leds.setColorRGB(0, 0, 255, 0);
  }
  
  /*read the line detector input
   * if reading Logic low set Red LED
  */
  if (LOW == digitalRead(lineFinder))
  {
    //Red LED
    leds.setColorRGB(0, 255, 0, 0);;
  }
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn nên chú ý khi line finder phát hiện vạch đen, đèn LED sẽ phát ra ánh sáng Đỏ, nếu không, nếu line finder không thể phát hiện ra vạch đen, đèn LED sẽ phát ra ánh sáng Xanh lục.


 ![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/line_eg3.jpg)


**Khám phá thêm**

Bây giờ bạn có thể xây dựng chiếc xe dò đường của riêng mình bằng cách sử dụng mô-đun line finder này và hai động cơ với motor driver(H-bridge), vì vậy khi line finder phát hiện đường màu đen, hãy kích hoạt một bên của động cơ bánh xe, một khi line finder đi khỏi đường màu đen, dừng động cơ đang chạy và kích hoạt phía còn lại, vì vậy xe chạy dọc theo đường màu đen với phần trước của xe liên tục rẽ trái hoặc phải.

### Phần 6: Grove - LCD RGB Backlight

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/LCD.jpg)

**Mục tiêu**	

Sử dụng Grove - LCD RGB Backlight để hiển thị "Hello World" và một số custom character.

**Kiến thức chính**

- Xem lại cách thêm thư viện
- Làm chủ positioning character kvà sử dụng mã nhị phân để tạo custom character.
- Cuộn văn bản hiển thị trên màn hình LCD
- Sử dụng LCD built-in character code để hiển thị các ký tự đặc biệt, ví dụ ký hiệu độ "°"

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/chartable.png)


**Yêu cầu phần cứng**	

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove - LCD RGB Backlight


**Kết nối phần cứng**

Bước 1: Kết nối mô-đun Grove - LCD RGB Backlight với cổng I2C của Seeeduino Lotus 
lưu ý: đó là cổng I2C theo sau là một dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/lcd_ard.jpg)


Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB.


**Lập trình phần mềm**

**Thêm thư viện**

Thêm [Thư viện](https://github.com/Seeed- Studio/Grove_LCD_RGB_Backlight/archive/master.zip) cho Grove - LCD RGB Backlight Screen 

Vui lòng làm theo hướng dẫn trong hướng dẫn 3 về cách <a href="#step3">Thêm thư viện</a>.

**Ví dụ 1**:Hiển thị Hello World

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//include the rgb_lcd library
#include "rgb_lcd.h"

//assign name lcd to rgb_lcd
rgb_lcd lcd;

void setup() 
{
    // set up the LCD's number of columns and rows:
    lcd.begin(16, 2);
    
    // Print Hello, World! to the LCD.
    lcd.print("Hello, World!");
    delay(1000);
}

void loop() 
{
    // set the cursor to column 0, line 1
    // (note: line 1 is the second row, since counting begins with 0):
    lcd.setCursor(0, 1);
    // print the number of seconds since reset:
    lcd.print(millis()/1000);
    delay(100);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn sẽ thấy trong "Hello, World!" được hiển thị ở dòng đầu tiên và đồng hồ đếm ngược ở dòng thứ hai.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/helloworld.jpg)

**Ví dụ 2**: Hiển thị logo Seeed Studio và sử dụng mã ký tự tích hợp để hiển thị văn bản

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add LCD library
#include "rgb_lcd.h"

//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

/*draw customise character
  in this case is the seeed studio logo
*/
byte top_leftleft[8] = {
  B00000,
  B00000,
  B01000,
  B01000,
  B01000,
  B01100,
  B01100,
  B01110
};
byte top_midleft[8] = {
  B00001,
  B00010,
  B00010,
  B00110,
  B00110,
  B00100,
  B01100,
  B01100
};
byte top_midright[8] = {
  B10000,
  B01000,
  B01000,
  B01100,
  B01100,
  B00100,
  B00110,
  B00110
};
byte top_rightright[8] = {
  B00000,
  B00000,
  B00010,
  B00010,
  B00010,
  B00110,
  B00110,
  B01110
};
byte bot_leftleft[8] = {
  B00110,
  B00111,
  B00011,
  B00011,
  B00001,
  B00000,
  B00000,
  B00000
};
byte bot_midleft[8] = {
  B01100,
  B01110,
  B00110,
  B00110,
  B10011,
  B11011,
  B11111,
  B01111
};
byte bot_midright[8] = {
  B00110,
  B01110,
  B01100,
  B01100,
  B11001,
  B11011,
  B11111,
  B11110
};
byte bot_rightright[8] = {
  B01100,
  B11100,
  B11000,
  B11000,
  B10000,
  B00000,
  B00000,
  B00000
};

void setup()
{
  //initialise the lcd screen;
  // set up the lcd's number of columns and rows:
  lcd.begin(16, 2);

  /*create and assign numbers of
    each seeed studio logo elements
  */
  lcd.createChar(0, top_leftleft);
  lcd.createChar(1, top_midleft);
  lcd.createChar(2, top_midright);
  lcd.createChar(3, top_rightright);
  lcd.createChar(4, bot_leftleft);
  lcd.createChar(5, bot_midleft);
  lcd.createChar(6, bot_midright);
  lcd.createChar(7, bot_rightright);


  /* set the cursor to column 4, line 0
    note: line 0 is the first row, since counting begins with 0
    same rule apply to the column as well
  */
  lcd.setCursor(4, 0);
  //Print I and a space to the LCD at column 4, line 0
  lcd.print("I ");
  //set the cursor to column 6, line 0
  lcd.setCursor(6, 0);
  /* Print LOVE by using the LCD character lookup table
     note write() method is mentt to send raw bytes
     print() is mostly intended to format data as ascii.
     this is different way of display text on lcd.
  */
  //character 76 is L on lookup table
  lcd.write(76);
  //the hex number 0x4F(is 79) associates with O on lookup table
  lcd.write(0x4F);
  //character 86 is V on lookup table
  lcd.write(86);
  //character 69 is E on lookup table
  lcd.write(69);
  //set the cursor to column 10, line 0
  lcd.setCursor(10, 0);
  //Print a space and Grove to the LCD
  lcd.write(" Grove");
  //set the cursor to column 4, line 1
  lcd.setCursor(4, 1);
  //Print text Seeed Studio to the LCD
  lcd.print("Seeed Studio");

  //display seeed studio logo
  lcd.setCursor(0, 0);
  lcd.write((unsigned char)0);
  lcd.setCursor(1, 0);
  lcd.write(1);
  lcd.setCursor(2, 0);
  lcd.write(2);
  lcd.setCursor(3, 0);
  lcd.write(3);
  lcd.setCursor(0, 1);
  lcd.write(4);
  lcd.setCursor(1, 1);
  lcd.write(5);
  lcd.setCursor(2, 1);
  lcd.write(6);
  lcd.setCursor(3, 1);
  lcd.write(7);
}

void loop()
{

}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn sẽ thấy Logo của Seeed Studio được hiển thị trong 8 khối đầu tiên, tiếp theo là “I Love Grove” ở dòng đầu tiên, và “Seeed Studio” ở dòng thứ hai.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/lcd_seeed.jpg)

**Ví dụ 3**:Cuộn văn bản trên màn hình LCD

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C


//add LCD library
#include "rgb_lcd.h"

//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

/*draw customise character
  in this case is the seeed studio logo
*/
byte top_leftleft[8] = {
  B00000,
  B00000,
  B01000,
  B01000,
  B01000,
  B01100,
  B01100,
  B01110
};
byte top_midleft[8] = {
  B00001,
  B00010,
  B00010,
  B00110,
  B00110,
  B00100,
  B01100,
  B01100
};
byte top_midright[8] = {
  B10000,
  B01000,
  B01000,
  B01100,
  B01100,
  B00100,
  B00110,
  B00110
};
byte top_rightright[8] = {
  B00000,
  B00000,
  B00010,
  B00010,
  B00010,
  B00110,
  B00110,
  B01110
};
byte bot_leftleft[8] = {
  B00110,
  B00111,
  B00011,
  B00011,
  B00001,
  B00000,
  B00000,
  B00000
};
byte bot_midleft[8] = {
  B01100,
  B01110,
  B00110,
  B00110,
  B10011,
  B11011,
  B11111,
  B01111
};
byte bot_midright[8] = {
  B00110,
  B01110,
  B01100,
  B01100,
  B11001,
  B11011,
  B11111,
  B11110
};
byte bot_rightright[8] = {
  B01100,
  B11100,
  B11000,
  B11000,
  B10000,
  B00000,
  B00000,
  B00000
};

void setup()
{
  //initialise the lcd screen;
  //set up the lcd's number of columns and rows:
  lcd.begin(16, 2);
  //wait for 1s
  delay(1000);
}

void loop()
{

  /*create and assign numbers of
    each seeed studio logo elements
  */
  lcd.createChar(0, top_leftleft);
  lcd.createChar(1, top_midleft);
  lcd.createChar(2, top_midright);
  lcd.createChar(3, top_rightright);
  lcd.createChar(4, bot_leftleft);
  lcd.createChar(5, bot_midleft);
  lcd.createChar(6, bot_midright);
  lcd.createChar(7, bot_rightright);

  /* set the cursor to column 4, line 0
    note: line 0 is the first row, since counting begins with 0
    same rule apply to the column as well
  */
  lcd.setCursor(4, 0);
  //Print I and a space to the LCD at column 4, line 0
  lcd.print("I ");
  //set the cursor to column 6, line 0
  lcd.setCursor(6, 0);
  /* Print LOVE by using the LCD character lookup table
     note write() method is mentt to send raw bytes
     print() is mostly intended to format data as ascii.
     this is different way of display text on lcd.
  */
  //character 76 is L on lookup table
  lcd.write(76);
  //the hex number 0x4F(is 79) associates with O on lookup table
  lcd.write(0x4F);
  //character 86 is V on lookup table
  lcd.write(86);
  //character 69 is E on lookup table
  lcd.write(69);
  //set the cursor to column 10, line 0
  lcd.setCursor(10, 0);
  //Print a space and Grove to the LCD
  lcd.write(" Grove");
  //set the cursor to column 4, line 1
  lcd.setCursor(4, 1);
  //Print text Seeed Studio to the LCD
  lcd.print("Seeed Studio");

  //display seeed studio logo
  lcd.setCursor(0, 0);
  lcd.write((unsigned char)0);
  lcd.setCursor(1, 0);
  lcd.write(1);
  lcd.setCursor(2, 0);
  lcd.write(2);
  lcd.setCursor(3, 0);
  lcd.write(3);
  lcd.setCursor(0, 1);
  lcd.write(4);
  lcd.setCursor(1, 1);
  lcd.write(5);
  lcd.setCursor(2, 1);
  lcd.write(6);
  lcd.setCursor(3, 1);
  lcd.write(7);
  
  // scroll 16 positions (string length) to the left
  // to move it offscreen left:
  for (int positionCounter = 0; positionCounter < 16; positionCounter++) {
    // scroll one position left:
    lcd.scrollDisplayLeft();
    // wait a bit:
    delay(200);
  }

  // scroll 32 positions (string length + display length) to the right
  // to move it offscreen right:
  for (int positionCounter = 0; positionCounter < 32; positionCounter++) {
    // scroll one position right:
    lcd.scrollDisplayRight();
    // wait a bit:
    delay(200);
  }

  // scroll 16 positions (display length + string length) to the left
  // to move it back to center:
  for (int positionCounter = 0; positionCounter < 16; positionCounter++) {
    // scroll one position left:
    lcd.scrollDisplayLeft();
    // wait a bit:
    delay(200);
  }
}

```
Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Bạn sẽ thấy màn hình cuộn đoạn văn bản, trước tiên từ phải sang trái cho đến khi tất cả văn bản biến mất ở cuối bên trái màn hình, sau đó văn bản sẽ cuộn ngược từ trái sang phải.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/lcd_scroll.jpg)

**Khám phá thêm**

[website](https://maxpromer.github.io/LCD-Character-Creator/) này giúp bạn tạo ký tự tùy chỉnh cho màn hình LCD được điều khiển bởi Arduino.

### Phần 7: Grove - Temperature & Humidity Sensor (DHT11)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/DHT11.jpg)

**Mục tiêu**

Sử dụng mô-đun cảm biến DHT11 để phát hiện nhiệt độ và độ ẩm xung quanh và hiển thị dữ liệu đầu ra từ DHT11 sang Màn hình LCD.

**Kiến thức chính**

- DHT11 là mô-đun cảm biến kỹ thuật số
- Xem lại cách vận hành Serial Monitor và Màn hình LCD
- Thêm Thư viện DHT11 và thiết lập ban đầu cho DHT11
- Sử dụng Serial Monitor và Màn hình LCD để hiển thị dữ liệu từ cảm biến DHT11


**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove - Cảm biến nhiệt độ và độ ẩm (DHT11)

**Kết nối phần cứng**

Bước 1: Kết nối mô đun Grove - Cảm biến nhiệt độ và độ ẩm (DHT11) đến cổng D2 của Seeeduino Lotus.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/DHT11_ard.jpg)

Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB


**Lập trình phần mềm**

**Thêm** [Thư viện](https://github.com/Seeed- Studio/Grove_Temperature_And_Humidity_Sensor/archive/master.zip)

**Ví dụ 1**: Sử dụng Serial Monitor để theo dõi nhiệt độ và độ ẩm xung quanh

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add DHT sensor library
#include <DHT.h>

//set digital pin2 as DHTPIN
#define DHTPIN 2
//set the sensor type as DHT 11
#define DHTTYPE DHT11

/*assign dht as the name of DHT sensor
  set the sensor pin as DHTPIN(pin2),
  set the sensor type as DHTTYPE(DHT11)
*/
DHT dht(DHTPIN, DHTTYPE);

void setup() {
  //initialise the dht sensor
  dht.begin();
  // opens serial port, sets data rate to 9600 bps
  Serial.begin(9600);
  //wait for 2s to initialise the board
  delay(2000);
}

void loop() {
  //store the humidity value to h
  int h = dht.readHumidity();
  //store the temperature value to t(in Celsius)
  int t = dht.readTemperature();
  //store the converted temperature value in fahrenheit to f
  int f = dht.convertCtoF(t);
  //display the title Temperature in C:
  Serial.print("Temperature in C: ");
  //display the temperature value t
  Serial.print(t);
  /* note the difference Serial.print()
     and Serial.println(),
     Serial.print() print the data in the same line
     Serial.println() print the data on the new line
     display the temperature unit ºC and change new line
  */
  Serial.println("ºC");
  //display the title Temperature in F:
  Serial.print("Temperature in F: ");
  //display the temperature value f
  Serial.print(f);
  //display the temperature unit ºF and change new line
  Serial.println("ºF");
  //display the title Humidity:
  Serial.print("Humidity: ");
  //display the Humidity value h
  Serial.print(h);
  //display the % sign
  Serial.println("%");
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Mở Serial Monitor

Bước 4: Quan sát kết quả

Bạn sẽ thấy một văn bản tương tự hiển thị dữ liệu nhiệt độ và độ ẩm trong serial monitor như hình dưới đây.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result1.png)

**Ví dụ 2**: Sử dụng màn hình LCD để hiển thị dữ liệu từ cảm biến DHT11

Đầu tiên là kết nối Mô-đun Grove - LCD RGB Backlight với cổng I2C của Seeeduino Lotus 
lưu ý: đó là cổng I2C theo sau là một dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/DHT11_lcd.png)

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add DHT sensor library
#include <DHT.h>
//add LCD library
#include <rgb_lcd.h>

//set digital pin2 as DHTPIN
#define DHTPIN 2
//set the sensor type as DHT 11
#define DHTTYPE DHT11

/*assign dht as the name of DHT sensor
  set the sensor pin as DHTPIN(pin2),
  set the sensor type as DHTTYPE(DHT11)
*/
DHT dht(DHTPIN, DHTTYPE);

//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

void setup() {
  //initialise the dht sensor
  dht.begin();
  //initialise the lcd screen;
  //set up the lcd's number of columns and rows:
  lcd.begin(16, 2);
  //wait for 2s
  delay(2000);
}

void loop() {
  //store the humidity value to h
  int h = dht.readHumidity();
  //store the temperature value to t(in Celsius)
  int t = dht.readTemperature();
  
  //set the LCD cursor to column 0, line 0
  lcd.setCursor(0, 0);
  //Print text temperature: to the LCD
  lcd.print("Temperature:");
  //set the LCD cursor to column 12, line 0
  lcd.setCursor(12, 0);
  //Print temperature value t to the LCD
  lcd.print(t);
  //set the LCD cursor to column 14, line 0
  lcd.setCursor(14, 0);
  //Print temperature º is character 223 on lookup table
  lcd.write(223);
  //Print C to the LCD
  lcd.print("C");
  
  //set the LCD cursor to column 0, line 1
  lcd.setCursor(0, 1);
  //Print text Humidity: to the LCD
  lcd.print("Humidity: ");
  //set the LCD cursor to column 10, line 1
  lcd.setCursor(10, 1);
  //Print humidity value h to the LCD
  lcd.print(h);
  //set the LCD cursor to column 12, line 1
  lcd.setCursor(12, 1);
  //Print sign % to the LCD
  lcd.print("%");
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

bạn có thể thấy màn hình nhiệt độ và độ ẩm phòng hiện tại trên màn hình LCD.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/DHT11_result.jpg)

**Khám phá thêm**

Sau phần này, bạn có thể xây dựng trạm thời tiết của riêng mình bằng cách sử dụng cảm biến DHT11 và màn hình Grove - LCD RGB Backlight.

### Phần 8: Grove - 3-Axis Digital Accelerometer

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis_cover.jpg)

**Mục tiêu**	

Tìm hiểu cách vận hành 3-axis digital accelerometer bằng cách quan sát dữ liệu đầu ra được hiển thị trên màn hình LCD.

**Kiến thức chính**

- Sử dụng serial monitor để hiển thị giá trị offset và gia tốc từ 3-axis accelerometer, khám phá mối quan hệ giữa dữ liệu đầu ra và vị trí của 3-axis accelerometer
- Sử dụng dữ liệu offset từ 3-axis accelerometer để tính giá trị pitch và giá trị roll và quan sát sự thay đổi dữ liệu liên quan đến vị trí của 3-axis accelerometer.
- Tìm hiểu cách sử dụng tilt switch để chuyển đổi giữa các trang của màn hình LCD, do đó, dữ liệu lớn từ 3-axis accelerometer có thể được hiển thị rõ ràng.


**Yêu cầu phần cứng**

Tự chuẩn bị

- Cáp micro-USB
- Một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove
- Grove – 3-Axis Digital Accelerometer
- Grove - LCD RGB Backlight
- Grove – Tilt Switch	


**Kết nối phần cứng**

Bước 1: Kết nối Grove – 3-Axis Digital Accelerometer với cổng I2C của Seeeduino Lotus 
lưu ý: đó là cổng I2C theo sau bởi hai dấu chấm.
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis_ard.jpg)

Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB.

**Lập trình phần phềm**

**Thêm thư viện**

Vui lòng thêm [Thư viện 3-axis accelerometer driver](https://github.com/Seeed- Studio/Accelerometer_MMA7660/archive/master.zip) vào Arduino IDE

**Ví dụ 1**:Sử dụng Serial Monitor để hiển thị dữ liệu đầu ra từ 3-axis accelerometer

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add accelemeter library
#include "MMA7660.h"

//assign accelemeter as the name of MMA7660 accelemeter
MMA7660 accelemeter;

void setup()
{
  //initialise the accelemeter
  accelemeter.init();
  // opens serial port, sets data rate to 9600 bps
  Serial.begin(9600);
}
void loop()
{
  //initialise x, y, z as int8_t
  int8_t x;
  int8_t y;
  int8_t z;
  //initialise ax, ay, az as float
  float ax, ay, az;
  //get x y z offset value from accelemeter
  accelemeter.getXYZ(&x, &y, &z);
  //display title x =
  Serial.print("x = ");
  //display value of x
  Serial.println(x);
  //display title y =
  Serial.print("y = ");
  //display value of y
  Serial.println(y);
  //display title z =
  Serial.print("z = ");
  //display value of z
  Serial.println(z);
  
  //get ax ay az acceleration value from accelemeter
  accelemeter.getAcceleration(&ax, &ay, &az);
  //display title accleration of X/Y/Z: 
  Serial.println("accleration of X/Y/Z: ");
  //display value of ax
  Serial.print(ax);
  //display unit g
  Serial.println(" g");
  //display value of ay
  Serial.print(ay);
  //display unit g
  Serial.println(" g");
  //display value of az
  Serial.print(az);
  //display unit g
  Serial.println(" g");
  //display ************* as divider to make thing prettier
  Serial.println("*************");
  //wait for 0.5s
  delay(500);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Mở Serial Monitor

Bước 4: Quan sát kết quả

Vui lòng lưu ý các thay đổi dữ liệu bằng cách để vị trí 3-axis accelerometer theo hình ảnh bên dưới.


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result2.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result3.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result4.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result5.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result6.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result7.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result8.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result9.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result10.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result11.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result12.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result13.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result14.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result15.png)

**Ví dụ 2**:Sử dụng dữ liệu từ 3-axis accelerometer để tính giá trị của Pitch và Roll

Kiến thức nền tảng:

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/aircraft.png)

như thể hiện trong hình trên:

Pitch (Transverse axis) θ: nó có nguồn gốc ở trung tâm trọng lực và được hướng sang phải, song song với một đường được vẽ từ wingtip đến wingtip. Chuyển động về trục này được gọi là pitch. Một chuyển động pitching tích cực làm tăng mũi máy bay và hạ thấp đuôi. Các thang máy là kiểm soát chính của pitch. (Aircraft principal axes 2018)

Yaw (Vertical axis) ψ: nó có nguồn gốc ở trung tâm trọng lực và được hướng xuống đáy máy bay, vuông góc với cánh và với đường tham chiếu thân máy bay. Chuyển động về trục này được gọi là yaw. Một chuyển động yawing tích cực di chuyển mũi máy bay sang phải. Bánh lái là điều khiển chính của yaw. (Aircraft principal axes 2018)

Roll (Longitudinal axis) Φ: nó có nguồn gốc ở trung tâm trọng lực và được hướng về phía trước, song song với đường tham chiếu thân máy bay. Chuyển động về trục này được gọi là roll. Một sự dịch chuyển góc về trục này được gọi là bank. [3] Một chuyển động rolling tích cực nâng cánh trái và hạ cánh phải. (Aircraft principal axes 2018)

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

#include <Wire.h>
//add accelemeter library
#include "MMA7660.h"

//assign accelemeter as the name of MMA7660 accelemeter
MMA7660 accelemeter;

//set value 0.5 to alpha
const float alpha = 0.5;

//initialise fXg, fYg, fZg as double with value of 0
double fXg = 0;
double fYg = 0;
double fZg = 0;
//initialise pitch and roll as double
double pitch, roll;

void setup()
{
  //initialise the accelemeter
  accelemeter.init();
  // opens serial port, sets data rate to 9600 bps
  Serial.begin(9600);
}
void loop()
{
  //initialise x, y, z as int8_t
  int8_t x;
  int8_t y;
  int8_t z;
  //get x y z offset value from accelemeter
  accelemeter.getXYZ(&x, &y, &z);

  //Low Pass Filter to reduce the noise
  fXg = x * alpha + (fXg * (1.0 - alpha));
  fYg = y * alpha + (fYg * (1.0 - alpha));
  fZg = z * alpha + (fZg * (1.0 - alpha));

  //Roll & Pitch Equations
  roll  = (atan2(-fYg, fZg) * 180.0) / M_PI;
  pitch = (atan2(fXg, sqrt(fYg * fYg + fZg * fZg)) * 180.0) / M_PI;
  //display title roll =
  Serial.print("roll = ");
  //display the roll value
  Serial.println(roll);
  //display title pitch =
  Serial.print("pitch = ");
  //display the pitch value
  Serial.println(pitch);
  delay(500);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Vui lòng đặt 3-axis accelerometer trên một bề mặt được cân bằng như hình bên dưới.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis.jpg)


Quan sát Roll data
Vui lòng lật lên / xuống 3-axis accelerometer theo các mũi tên màu xanh lục trong hình trên, bây giờ giá trị của roll sẽ tăng khi bạn lật xuống, giảm khi lật lên, ngoài ra, giá trị của roll là dương khi lật xuống tại điểm gốc (đặt song song với mực nước), âm khi lật lên.

Quan sát Pitch data
Vui lòng nghiêng trái / phải 3-axis accelerometer theo các mũi tên màu đỏ trong hình trên, bây giờ giá trị của pitch sẽ tăng khi bạn nghiêng phải, giảm khi nghiêng trái, ngoài ra, giá trị của pitch là dương khi nghiêng phải so với gốc (đặt song song với mực nước), âm khi nghiêng trái.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result2.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result16.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result10.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result17.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result8.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result18.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result4.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result19.png)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result6.jpg)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/result20.png)

Bây giờ chúng ta có thể sử dụng gia tốc kế 3 trục để điều khiển hoặc điều chỉnh hướng của máy bay hoặc ô tô, bằng cách chuyển đổi dữ liệu cao độ và cuộn để điều khiển tín hiệu để điều khiển bộ truyền động, công nghệ tương tự được áp dụng cho điều chỉnh màn hình tự động trên điện thoại di động khi bạn nghiêng điện thoại từ dọc sang ngang.



**Ví dụ 3**: Sử dụng màn hình LCD để hiển thị dữ liệu đầu ra từ 3-axis accelerometer

Vui lòng kết nối Grove - Tilt Switch sang cổng D5 của Seeeduino Lotus và kết nối mô đun  Grove - LCD RGB Backlight với cổng I2C của Seeeduino Lotus, 
LƯU Ý: đó là cổng I2C theo sau là một dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis_lcd_tilt.jpg)

Ở đây chúng tôi sử dụng tilt switch để lật trang trên màn hình LCD để hiển thị các bộ dữ liệu khác nhau, khi tilt switch BẬT, màn hình LCD sẽ hiển thị dữ liệu của X, Y, Z Roll và Pitch, khi tilt switch ở vị trí TẮT LCD màn hình sẽ hiển thị dữ liệu tăng tốc của aX, aY, aZ theo từng hướng tương đối.

Bước 1: copy & paste đoạn code sau vào Arduino IDE

```C

//add accelemeter library
#include "MMA7660.h"
//add LCD library
#include <rgb_lcd.h>


//assign name tiltswitchPin to pin 5
#define tiltswitchPin 5

//assign accelemeter as the name of MMA7660 accelemeter
MMA7660 accelemeter;
//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

//set value 0.5 to alpha
const float alpha = 0.5;

//initialise fXg, fYg, fZg as double with value of 0
double fXg = 0;
double fYg = 0;
double fZg = 0;
//initialise pitch and roll as double

void setup()
{
  //initialise the accelemeter
  accelemeter.init();
  //initialise the lcd screen;
  //set up the lcd's number of columns and rows:
  lcd.begin(16, 2);
  //set pinMode of tiltswitchPin to input
  pinMode(tiltswitchPin, INPUT);
  //wait for 2s
  delay(2000);

}
void loop()
{
  /*if tilt switch is on display X, Y, Z, Roll and Pitch data
    if tilt switch is off display X, Y, Z acceleration data
  */
  if (HIGH == digitalRead(tiltswitchPin))
  {
    //initialise x, y, z as int8_t, pitch and roll as double
    int8_t x;
    int8_t y;
    int8_t z;
    double roll;
    double pitch;
    //get x y z offset value from accelemeter
    accelemeter.getXYZ(&x, &y, &z);

    //Low Pass Filter to reduce the noise
    fXg = x * alpha + (fXg * (1.0 - alpha));
    fYg = y * alpha + (fYg * (1.0 - alpha));
    fZg = z * alpha + (fZg * (1.0 - alpha));

    //Roll & Pitch Equations
    roll  = (atan2(-fYg, fZg) * 180.0) / M_PI;
    pitch = (atan2(fXg, sqrt(fYg * fYg + fZg * fZg)) * 180.0) / M_PI;
    //reset the lcd screen
    lcd.clear();
    //set the LCD cursor to column 0, line 0
    lcd.setCursor(0, 0);
    //display text x:
    lcd.print("x:");
    //display value of x
    lcd.print(x);
    //set the LCD cursor to column 5, line 0
    lcd.setCursor(5, 0);
    //display text y:
    lcd.print("y:");
    //display value of y
    lcd.print(y);
    //set the LCD cursor to column 10, line 0
    lcd.setCursor(10, 0);
    //display text z:
    lcd.print("z:");
    //display value of z
    lcd.print(z);

    //set the LCD cursor to column 0, line 1
    lcd.setCursor(0, 1);
    //display text R:
    lcd.print("R:");
    //display value of roll
    lcd.print(roll);
    //set the LCD cursor to column 8, line 1
    lcd.setCursor(8, 1);
    //display text P:
    lcd.print("P:");
    //display value of pitch
    lcd.print(pitch);
  } else
  {
    //initialise ax, ay, az as float
    float ax, ay, az;
    //get ax ay az acceleration value from accelemeter
    accelemeter.getAcceleration(&ax, &ay, &az);
    //reset the lcd screen
    lcd.clear();
    //set the LCD cursor to column 0, line 0
    lcd.setCursor(0, 0);
    //display text ax:
    lcd.print("ax:");
    //display value of ax
    lcd.print(ax);
    //set the LCD cursor to column 8, line 0
    lcd.setCursor(8, 0);
    //display text ay:
    lcd.print("ay:");
    //display value of ay
    lcd.print(ay);
    //set the LCD cursor to column 0, line 1
    lcd.setCursor(0, 1);
    //display text az:
    lcd.print("az:");
    //display value of az
    lcd.print(az);
  }
  //wait 0.5s
  delay(500);
}

```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

Trước tiên, vui lòng kiểm tra xem công tắc nghiêng có làm thay đổi trang của màn hình LCD không. Sau đó, bạn có thể xoay 3-axis accelerometer xung quanh để quan sát sự thay đổi dữ liệu theo các phép quay, làm quen với dữ liệu đầu ra liên kết với các định hướng của  3-axis accelerometer.

Hiển thị vận tốc, pitch và roll khi bật / tắt công tắc nghiêng:

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/3_axis_tilt_on&off.jpg)

**Khám phá thêm**

Sau khi tìm hiểu xung quanh với mô-đun gia tốc kỹ thuật số, bạn có thể hình dung được rằng gia tốc kế là một trong những mô-đun quan trọng nhất có thể được tìm thấy trong hệ thống dẫn đường tên lửa cùng với các mô-đun khác như GPS và con quay hồi chuyển, vv .. gia tốc kế cũng được sử dụng trong điện thoại di động để phát hiện nếu điện thoại ở chế độ dọc hoặc chế độ nằm ngang, do đó màn hình có thể nghiêng và điều chỉnh cho phù hợp.



### Phần 9: Smart Garden


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartgarden.png)

**Mục tiêu**

Để tạo cảm biến và hệ thống nhắc nhở Smart Garden bằng cách kết hợp các mô-đun Grove starter kit

**Kiến thức chính**

- tìm hiểu cách kết hợp nhiều mô-đun vào một ứng dụng
- tìm hiểu cách mã hóa cho nhiều thiết bị trong Arduino IDE
- áp dụng nhiều mô-đun để phát hiện và phân tích môi trường trồng trọt, cải thiện kỹ năng tư duy logic

**Use case analysis**

**Mô-đun Sensor**

Sử dụng mô-đun DHT11 để theo dõi môi trường xung quanh của nhà máy, sử dụng cảm biến ánh sáng để phát hiện cường độ ánh sáng xung quanh.


**Mô-đun Actuator**

Sử dụng bộ rung để tạo các âm báo khác nhau và LCD để thông báo các thông báo các bản tin khác nhau:

- cảnh báo 1: nhiệt độ xung quanh cao hơn 38 ° C
- cảnh báo 2: độ ẩm xung quanh thấp hơn 40%
- cảnh báo 3: Cường độ ánh sáng thấp hơn 50
- cảnh báo 4: nhắc nhở người dùng tưới cây


Sử dụng màn hình LCD:

- trạng thái 1: Hiển thị nhiệt độ
- trạng thái 2: Hiển thị độ ẩm
- trạng thái 3: nhắc nhở người dùng tưới cây

Sử dụng tilt switch để thiết lập lại cảnh báo.

**Flowchart**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/flowchart.png)

**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver
- Khung DIY acrylic


Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove 
- Grove – Buzzer
- Grove – Chainable RGB LED
- Grove – Light Sensor
- Grove - LCD RGB Backlight
- Grove – Temperature &Humidity Sensor(DHT11)
- Grove – Tilt Switch

**Kết nối phần cứng**

Bước 1:
Kết nối Mô-đun Grove – Buzzer với cổng D6 của Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer_ard.jpg)

Kết nối Grove – Chainable RGB LED với cổng D7 của Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect1.jpg)

Kết nối Mô-đun Grove – Light Sensor với cổng A0 của Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect2.jpg)

Kết nối Mô-đun Grove - LCD RGB Backlight với cổng I2C của Seeeduino Lotus 
lưu ý: đó là cổng I2C theo sau là một dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect3.jpg)

Kết nối mô đun Grove – Temperature &Humidity Sensor(DHT11) đến cổng D2 của Seeeduino Lotus.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect4.jpg)

Kết nối Grove – Tilt Switch sang cổng D5 của Seeeduino Lotus.


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect5.jpg)

Cố định tất cả các thành phần với nhau trên khung acrylic DIY

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartgarden1.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartgarden2.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartgarden3.png)

Bước 2: Kết nối Seeeduino Lotus với máy tính bằng cáp micro USB.


**Lập trình phần mềm**

Bước 1: Vui lòng thêm [Thư viện TimeLib](https://github.com/PaulStoffregen/Time/archive/master.zip) vào Arduino IDE
Để biết thêm thông tin, vui lòng truy cập [Arduino TimeLib tutorial](http://playground.arduino.cc/code/time)

Bước 2: copy & paste đoạn code sau vào Arduino IDE

```C

//add DHT sensor library
#include <DHT.h>
//add LCD library
#include <rgb_lcd.h>
//add ChainableLED library to this project
#include <ChainableLED.h>
//add Timelib library
#include <TimeLib.h>

//assign default time as epoch time 1514764800 which is 00:00:00 Jan 1 2018
long DEFAULT_TIME = 1514764800;
long waterTime = DEFAULT_TIME + 86400;

//set the number of leds linked to the chain
#define NUM_LEDS  1

//assign LightSensor as A0
#define LightSensor A0
//set digital pin2 as DHTPIN
#define DHTPIN 2
//set title of pin 5 as tiltSwitch
#define tiltSwitch 5
//assign buzzer as pin 6
#define buzzer 6

//set the sensor type as DHT 11
#define DHTTYPE DHT11

/*assign dht as the name of DHT sensor
  set the sensor pin as DHTPIN(pin2),
  set the sensor type as DHTTYPE(DHT11)
*/
DHT dht(DHTPIN, DHTTYPE);

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

void setup()
{
  //
  setTime(DEFAULT_TIME);
  //initialise the dht sensor
  dht.begin();
  //initialise the lcd screen;
  //set up the lcd's number of columns and rows:
  lcd.begin(16, 2);
  //initialise ChainableLED leds
  leds.init();
  //set pin 5(tilt switch) as input pin
  pinMode(tiltSwitch, INPUT);
  delay(1000);
}
int mode = 0;
void loop()
{
  //-------------DHT---------------------
  //store the humidity value to h
  int h = dht.readHumidity();

  //store the temperature value to t(in Celsius)
  int t = dht.readTemperature();

  int value = analogRead(LightSensor);
  float value_float = map(value, 0, 800, 50, 0) / 100.0;

  leds.setColorHSB(0, 0, 0, value_float);

  //initialise mode to 0, then set to case 0;

  //temperature exceed 38 degrees, then set to case 1;
  if (t > 38) {
    mode = 1;
  }
  //Humidity is less than 40 %, then set to case 2;
  if (h < 40)
  {
    mode = 2;
  }
  //LightSensor reading value is less than 50, then set to case 3;
  if (value < 50)
  {
    mode = 3;
  }
  //current time is greate or equals to waterTime(24 hour ahead), then set to case 4;
  if (now() >= waterTime  ) {
    mode = 4;
  }

  switch (mode) {
    case 0:
      //set the LCD cursor to column 0, line 0
      lcd.clear();
      lcd.setCursor(0, 0);
      //Print text temperature: to the LCD
      lcd.print("Temperature:");
      //set the LCD cursor to column 12, line 0
      lcd.setCursor(12, 0);
      //Print temperature value t to the LCD
      lcd.print(t);
      //set the LCD cursor to column 14, line 0
      lcd.setCursor(14, 0);
      //Print temperature º is character 223 on lookup table
      lcd.write(223);
      //Print C to the LCD
      lcd.print("C");

      //set the LCD cursor to column 0, line 1
      lcd.setCursor(0, 1);
      //Print text Humidity: to the LCD
      lcd.print("Humidity: ");
      //set the LCD cursor to column 10, line 1
      lcd.setCursor(10, 1);
      //Print humidity value h to the LCD
      lcd.print(h);
      //set the LCD cursor to column 12, line 1
      lcd.setCursor(12, 1);
      //Print sign % to the LCD
      lcd.print("%");
      break;
    case 1:
      tone(buzzer, 262, 300);
      leds.setColorRGB(0, 255, 0, 0);
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Temperature too ");
      lcd.setCursor(0, 1);
      lcd.print("High!!");
      if (HIGH == digitalRead(tiltSwitch))
      {
        leds.setColorRGB(0, 0, 0, 0);
        mode = 0;
      }
      break;
    case 2:
      tone(buzzer, 294, 300);
      leds.setColorRGB(0, 255, 0, 0);
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Warning! Too Dry");
      if (HIGH == digitalRead(tiltSwitch))
      {
        leds.setColorRGB(0, 0, 0, 0);
        mode = 0;
      }
      break;
    case 3:
      tone(buzzer, 330, 300);
      leds.setColorRGB(0, 255, 0, 0);
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Not Enough Light");
      lcd.setCursor(0, 1);
      lcd.print("Check the LED..");
      if (HIGH == digitalRead(tiltSwitch))
      {
        leds.setColorRGB(0, 0, 0, 0);
        mode = 0;
      }
      break;
    case 4:
      tone(buzzer, 349, 300);
      leds.setColorRGB(0, 255, 0, 0);
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Time to water");
      lcd.setCursor(0, 1);
      lcd.print("the plants");
      if (HIGH == digitalRead(tiltSwitch))
      {
        waterTime = now() + 86400;
        mode = 0;
      }
      break;

  }
}

```

Bước 3: Nạp code vào Seeeduino Lotus

Bước 4: Quan sát kết quả

Trong điều kiện bình thường, đèn LED chiếu ánh sáng trắng và màn hình LCD hiển thị nhiệt độ và độ ẩm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden.png)

4 trạng thái cảnh báo

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden1.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden2.png)
![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden3.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden4.png)

Cảnh báo đèn LED đỏ

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden5.png)

Đặt lại cảnh báo bằng cách sử dụng tilt switch

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden6.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/garden7.png)



### Phần 10: Smart Cup

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartcup.png)

**Mục tiêu**

Tạo cốc thông minh bằng cách sử dụng còi, đèn LED RGB, 3-Axis Accelerometer và màn hình LCD, nó sẽ nhắc nhở người dùng uống nước trong một khoảng thời gian nhất định, cốc thông minh cũng có thể phát hiện nếu người dùng tiêu thụ một ít nước, màn hình LCD sẽ hiển thị thời gian đếm ngược để nhắc nhở người dùng khi nào sẽ là lần tiếp theo để uống nước.


**Kiến thức chính**

- xem lại Thư viện TimeLib về cài đặt và kiểm soát thời gian với Lotus.
- chỉnh sửa hiển thị và cuộn văn bản trên màn hình LCD
- xem lại if…else…và switch…case…operation với || (hoặc) và toán tử logic && (và).
- kiểm tra thêm các ứng dụng đọc giá trị pitch và roll từ 3-Axis Accelerometer.
- sử dụng phương pháp ví dụ BlinkWithoutDelay để tránh sử dụng hàm Delay, loại bỏ việc  hàm Delay để bỏ lỡ system timer.
- tìm hiểu cách tạo và gọi hàm tùy chỉnh, kết quả trả về có thể là Boolean (trun / false) hoặc giá trị của biến bằng cách sử dụng return X.

**Use case analysis**

**Mô đun sensor**

Bằng cách so sánh dữ liệu pitch và roll từ số đọc 3-axis accelerometer để phát hiện xem cốc có bị nghiêng hay không, do đó, nó nhận ra người dùng có uống nước hay không. Nếu cốc bị nghiêng, bước tiếp theo sẽ phát hiện nếu cốc đã được đặt trở lại trên bàn, một khi cốc đã ở trên bàn, dữ liệu pitch và roll từ 3-axis accelerometer sẽ hiệu chỉnh giá trị tối đa và tối thiểu để so sánh.

**Mô đun actuator**

Sử dụng buzzer để tạo các âm khác nhau để nhắc nhở trạng thái khác nhau:

- trạng thái 1: khi hẹn giờ đếm ngược 30 phút kết thúc, tiếng chuông sẽ kêu để nhắc nhở người dùng uống nước
- trạng thái 2: còi sẽ kêu nếu cốc không nằm yên trên bàn.

Sử dụng màn hình LCD

- trạng thái 1: đếm ngược thời gian
- trạng thái 2: nhắc nhở người dùng uống nước
- trạng thái 3: chúc mừng người dùng đã uống nước
- trạng thái 4: nhắc nhở người đổ nước lại sau khi uống xong


**Flowchart**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/flowchart1.png)

**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- một máy tính có Arduino IDE và được cài đặt serial-to-USB driver

Bao gồm trong kit

- Seeeduino Lotus V1.1 development board
- Cáp Grove 
- Grove – Buzzer
- Grove – LED Chainable RGB LED
- Grove - LCD RGB Backlight
- Grove – 3-Axis Digital Accelerometer

**Kết nối phần cứng**

Bước 1:
Kết nối Mô-đun Grove - Buzzer với cổng D6 của Seeeduino Lotus


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/buzzer_ard.jpg)

Kết nối Grove – Chainable RGB LED với cổng D7 của Seeeduino Lotus

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect1.jpg)


Kết nối Mô-đun Grove - LCD RGB Backlight với cổng I2C của Seeeduino Lotus 
lưu ý: đó là cổng I2C theo sau là một dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect6.jpg)
 

Kết nối Grove – 3-Axis Digital Accelerometer với cổng I2C của Seeeduino Lotus 
Lưu ý: đó là cổng I2C theo sau là hai dấu chấm.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/connect7.jpg)

Cố định tất cả các thành phần với nhau trên một cốc.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/smartcup.png)

**Lập trình phần mềm**

Bước 1: Vui lòng thêm [Thư viện TimeLib]( https://github.com/PaulStoffregen/Time/archive/master.zip) vào Arduino IDE

Copy & paste đoạn code sau vào Arduino IDE

```C

//add LCD library
#include <rgb_lcd.h>
//add accelerometer library
#include "MMA7660.h"
//add Timelib library
#include <TimeLib.h>
//add ChainableLED library to this project
#include <ChainableLED.h>

//assign default time as epoch time 1514764800 which is 00:00:00 Jan 1 2018
long DEFAULT_TIME = 1514764800;
//set drinkTime at 30mins(1800s) after default time
//long drinkTime = DEFAULT_TIME + 1800;
long drinkTime = DEFAULT_TIME + 10;
int lastDrink, seconds;
//will store lastest time in milliseconds
unsigned long previousMillis = 0;

//set the number of leds linked to the chain
#define NUM_LEDS  1

//assign buzzer as pin 6
#define buzzer 6

//assign accelerometer as the name of MMA7660 accelerometer
MMA7660 accelerometer;

//assign lcd as the name of rgb_lcd screen
rgb_lcd lcd;

/*assign leds as the name of
  the ChainableLED set the
  pin of the ChainableLED to
  pin7(clock pin) and pin8(data pin)
  and number of the leds*/
ChainableLED leds(7, 8, NUM_LEDS);

//set motion check tolerance value
int tolerance = 50;
//initalise the calibrated and moveDetedted as false
boolean calibrated = false;
boolean moveDetected = false;

//set int8_t for accelerometer reading value x, y, z
int8_t x;
int8_t y;
int8_t z;

//initialise fXg, fYg, fZg as double with value of 0
double fXg = 0;
double fYg = 0;
double fZg = 0;
//initialise pitch and roll as double
double p, r;

//Accelerometer limits
double rMin; //Minimum roll Value
double rMax; //Maximum roll Value
double rVal; //Current roll Value

double pMin; //Minimum pitch Value
double pMax; //Maximum pitch Value
double pVal; //Current pitch Value

//set value 0.5 to alpha for low pass filter tolerance
const float alpha = 0.5;

//iinitialise mode to set the default switch case to first(count from 0)
int mode = 0;

void setup()
{
  //set the system time to 00:00:00 Jan 1 2018
  setTime(DEFAULT_TIME);
  //initialise the accelerometer
  accelerometer.init();
  //initialise ChainableLED leds
  leds.init();
  //initialise the lcd screen;
  //set up the lcd's number of columns and rows:
  lcd.begin(16, 2);
  //calibrate the accelerometer for at the begining
  calibrateAccel();
  //wait for 2
  delay(2000);
}

//setup accelerometer reading function output mapped value of roll and pitch
void Accel() {
  accelerometer.getXYZ(&x, &y, &z);

  //Low Pass Filter to reduce the noise
  fXg = x * alpha + (fXg * (1.0 - alpha));
  fYg = y * alpha + (fYg * (1.0 - alpha));
  fZg = z * alpha + (fZg * (1.0 - alpha));

  r  = (atan2(-fYg, fZg) * 180.0) / M_PI;
  p = (atan2(fXg, sqrt(fYg * fYg + fZg * fZg)) * 180.0) / M_PI;
  r = map(r, -90, 90, 0, 180);
  p = map(p, -90, 90, 0, 180);
  return r;
  return p;
}

//setup function for calibrate the accelerometer
void calibrateAccel() {
  //reset moveDetected to false
  moveDetected = false;

  //call accelerometer reading funtion
  Accel();

  //assign the reading of roll and pitch
  rVal = r;
  rMin = rVal;
  rMax = rVal;

  pVal = p;
  pMin = pVal;
  pMax = pVal;

  //calibrate the Accelerometer
  for (int i = 0; i < 50; i++) {
    //call accelerometer reading funtion
    Accel();
    /*--calibrate roll---*/
    //assign the reading of roll to rVal
    rVal = r;
    //evaluate if the new reading is greater than stored Maximum value
    if (rVal > rMax) {
      //if new reading value is greater save new value to rMax
      rMax = rVal;
      //evaluate if the new reading is less than stored Minimum value
    } else if (rVal < rMin) {
      //if new reading value is less save new value to rMin
      rMin = rVal;
    }

    /*--calibrate pitch---*/
    //assign the reading of pitch to pVal
    pVal = p;
    //evaluate if the new reading is greater than stored Maximum value
    if (pVal > pMax) {
      //if new reading value is greater save new value to pMax
      pMax = pVal;
      //evaluate if the new reading is less than stored Minimum value
    } else if (pVal < pMin) {
      //if new reading value is less save new value to pMin
      pMin = pVal;
    }
    //Delay 10ms between readings
    delay(10);
  }
  //set the calibrated to true
  calibrated = true;
}

//drinking function check if the bottle is tilting output ture/false
boolean drinking() {
  //initialise tilting as false
  boolean tilting = false;
  //reading from accelerometer
  Accel();

  rVal = r;
  pVal = p;
  /*evaluate if new roll value is greater than the maximum value or
     less than the minimum value saved previously.
     || means or
     if rolling is happening then set tilting to ture
     if pitch is happening then set tilting to ture
  */
  if (rVal > (rMax + tolerance) || rVal < (rMin - tolerance)) {
    tilting = true;
  }

  if (pVal > (pMax + tolerance) || pVal < (pMin - tolerance)) {
    tilting = true;
  }
  //output tilting
  return tilting;
}

//mothin function
void Motion() {
  //don't check for movement until recalibrated again
  calibrated = false;
}

void loop()
{
  /*evaluate if current time is greate or equals
    to drinkTime(30mins ahead), then switch to case 1;
    its time to drink
  */
  if (now() >= drinkTime  ) {
    //switch to case 1
    mode = 1;
  }
  //evaluate if the accelerometer is calibrated
  if (calibrated) {
    //evaluate if the bottle is tilted
    if (drinking()) {
      //switch to case 2
      mode = 2;
      //set moveDetected to true
      moveDetected = true;
    }
  }
  //evaluate if the moveDetected is true
  if (moveDetected) {
    //call motion function
    Motion();
  }
  //save current time in millisecond
  unsigned long currentMillis = millis();
  switch (mode) {
    /*Case 0:
      mode to display countdonw time if nothing happened
    */
    case 0:
      //minutes to drink water
      lastDrink = (drinkTime - now()) / 60;
      //seconds to drink water
      seconds = (drinkTime - now()) % 60;

      leds.setColorHSB(0, 0, 0, 0);

      /*refesh the LCD for 1s without using delay, refer
         to Example "BlinkWithoutDelay", so the system
         won't stop and wait
      */
      if (currentMillis - previousMillis >= 1000) {
        // save the last time you refreshed the LCD
        previousMillis = currentMillis;
        lcd.clear();
        lcd.setCursor(0, 0);
        lcd.print("Countdown to dri");
        lcd.setCursor(0, 1);
        lcd.print("nk water: ");
        lcd.setCursor(10, 1);
        lcd.print(lastDrink);
        lcd.print(":");
        lcd.print(seconds);
      }
      break;
    /*Case 1:
       reached 30mins time to drink some water
       with buzzer alarm and LCD display time
       to drink some water
    */
    case 1:
      tone(buzzer, 262, 300);
      leds.setColorRGB(0, 255, 0, 0);
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Time to drink");
      lcd.setCursor(0, 1);
      lcd.print("Some water");
      break;
    /*Case 2:
       detect if the wate bottle is tilted
       therefore user is drinking some water
       and recalibrate the sensor(accelerometer)
       once the bottle has been put on a flat
       surface if the bottle is still tilted or
       not sitting flat(accelerometer reading
       is not around 90 degrees), enter case 3
       detected the bottle is resting still enter
       to case 0 and reset the drink time to 30mins
       ahead
    */
    case 2:
      //stop buzzer
      noTone(buzzer);
      //update drinkTime
      drinkTime = now() + 1800;
      leds.setColorRGB(0, 0, 255, 0);
      //display message
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Well Done remind");
      lcd.setCursor(0, 1);
      lcd.print("you in 30mins");
      //wait for 5s for user to drink
      delay(5000);
      //reading accelerometer value
      Accel();
      //evaluate if the bottle is resting on flat
      if (r > 80 && r < 100 && p > 80 && p < 100) {
        //evaluate if the accelerometer calibrated
        if (!calibrated) {
          //calibrate accelerometer
          calibrateAccel();
        }
        else
        { //switch to mode 0
          mode = 0;
          //update drinkTime
          drinkTime = now() + 1800;
          leds.setColorRGB(0, 0, 0, 0);
        }
      }
      else
      { //if bottle is not resting on flat switch to mode 3
        mode = 3;
        leds.setColorRGB(0, 0, 0, 0);
      }
      break;
    /*case 3
       if the bottle is not resting on flat surface,
       display message with scrolling "plaase put
       down water bottle when finished!", then check
       if the bottle is resting still, if so, recalibrate
       accelerometer and once recalibrated switch back to
       case 0 and reset drink time to 30mins ahead
    */
    case 3:
      //update drinkTime
      drinkTime = now() + 1800;

      leds.setColorRGB(0, 0, 0, 255);
      //display message with autoscroll
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Please put down water");
      lcd.setCursor(0, 1);
      lcd.print("bottle when finished!");
      for (int positionCounter = 0; positionCounter < 5; positionCounter++) {
        // scroll one position left:
        lcd.scrollDisplayLeft();
        // wait a bit:
        delay(200);
      }
      for (int positionCounter = 0; positionCounter < 5; positionCounter++) {
        // scroll one position right:
        lcd.scrollDisplayRight();
        // wait a bit:
        delay(200);
      }
      for (int positionCounter = 0; positionCounter < 5; positionCounter++) {
        // scroll one position left:
        lcd.scrollDisplayLeft();
        // wait a bit:
        delay(200);
      }

      //reading accelerometer value
      Accel();
      //evaluate if the bottle is resting on flat
      if (r > 80 && r < 100 && p > 80 && p < 100) {
        //evaluate if the accelerometer calibrated
        if (!calibrated) {
          //calibrate accelerometer
          calibrateAccel();
        }
        else
        { //switch to mode 0
          mode = 0;
          //update drinkTime
          drinkTime = now() + 1800;
          leds.setColorRGB(0, 0, 0, 0);
        }
      }
      break;
  }
  delay(1);
}


```

Bước 2: Nạp code vào Seeeduino Lotus

Bước 3: Quan sát kết quả

4 trạng thái của cốc thông minh

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/cup1.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/cup2.png)


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/cup3.png)![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_Arduino/master/img/cup4.png)


## TÀI LIỆU THAM KHẢO

Aircraft principal axes. Accessed November 27, 2018. https://en.wikipedia.org/wiki/Aircraft_principal_axes.

## PHỤ LỤC

Tất cả các đoạn code [coding](https://github.com/peterpanstechland/Grove_starter_kit.git) ở tài liệu này đều có sẵn ở trên Github.

## HỖ TRỢ TTECH 

Xin đừng ngần ngại gửi isssues vào [forum](https://forum.seeedstudio.com/) hoặc địa chỉ email[techsupport@seeed.cc](techsupport@seeed.cc).<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>