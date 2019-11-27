---
name: Grove Base Kit for Raspberry Pi
category: Others
bzurl:  
oldwikiname:  
prodimagename:
surveyurl: 
sku: 110020169
---


## GROVE SYSTEM

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/groveSystem.png)

Grove là một hệ thống module mẫu bao gồm một đơn vị cơ sở và các module khác nhau  với những kết nối được chuẩn hóa. Đơn vị cơ sở nói chung là một bộ vi xử lý cho phép giao tiếp, xử lý, và kiểm soát đầu vào hoặc đầu ra từ các module Grove . Mỗi module thường xử lý một chức năng duy nhất, từ một nút đơn giản đến cảm biến nhịp tim phức tạp hơn. Các kết nối Grove đã được chuẩn hóa cho phép người dùng kết nối các đơn vị Grove với các khối được xây dựng từ trước, so với hệ thống dây nhảy hoặc mối hàn dựa trên việc tháo và lắp dễ dàng hơn, đơn giản hóa hệ thống học tập để thử nghiệm, xây dựng và tạo mẫu.
Chúng tôi cũng cung cấp bộ chuyển đổi từ Grove sang Pin Header hoặc Grove Base HAT có sẵn cho các nền tảng phát triển đa dạng, cho những ai muốn sử dụng các module cảm biến Grove và bộ truyền động mà không có Grove System Development Board.

Người dùng Grove system cần có ít nhất một số nền tảng kiến thức cơ bản về điện tử, nếu không bạn cần xem hướng dẫn cơ bản này để tìm hiểu một số thao tác cơ bản trên Grove system, phần đầu tiên của hướng dẫn này bao gồm danh sách các thông tin cơ bản về các thành phần có trong starter kit, tiếp theo là thiết lập cơ bản Arduino IDE cho Seeeduino Lotus. Sau đó, 11 bài hướng dẫn sẽ cung cấp các hoạt động cơ bản cho từng thành phần riêng lẻ trong starter kit và các ứng dụng bằng cách kết hợp nhiều module với nhau, giúp người học có cái nhìn và hiểu biết cơ bản về kết nối và lập trình với Grove system.

## GROVE BASE KIT FOR RASPBERRY PI

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/kit.jpg)


Grove start kit chứa một Grove Base Hat (cho Raspberry Pi) và 10 module Grove. Các thông tin chi tiết được liệt kê dưới đây.

### Chi tiết sản phẩm

#### Grove Base Hat

**[Grove Base Hat cho Raspberry Pi](https://www.seeedstudio.com/Grove-Base-Hat-for-Raspberry-Pi-p-3186.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/BaseHat.jpg)


Ngày nay, hàng loạt các cảm biến, thiết bị truyền động, và màn hình đã phát triển thành một hệ sinh thái rộng lớn. Ngày càng có nhiều module sẽ được đưa vào hệ sinh thái Grove trong tương lai. Chúng tôi thấy Grove giúp các nhà sản xuất, kỹ sư, giáo viên, sinh viên và thậm chí là các nghệ sĩ,... Chúng tôi luôn cảm thấy có trách nhiệm làm cho module Grove tương thích với nhiều nền tảng hơn. Bây giờ chúng tôi mang đến cho bạn Grove Base Hat  cho Raspberry Pi và Grove Base Hat cho Raspberry Pi Zero, nói cách khác, chúng tôi mang đến Raspberry Pi the Grove System.


Grove Base Hat cho Raspberry Pi cung cấp cổng Digital/Analog/I2C/PWM/UART để đáp ứng mọi nhu cầu của bạn. Với sự trợ giúp của MCU được tích hợp sẵn, ADC 8 kênh 12 bit cũng có sẵn cho Raspberry Pi.


**Đặc trưng**

- Hỗ trợ Raspberry 2/3B/3B+/Zero
- MCU được tích hợp sẵn
- ADC 12 bit 
- Đa dạng về cổng Grove


**Tổng quan phần cứng**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/pi_pinout.jpg)

GPIO：Các chân ra giống raspberry pi.

PWM：Cổng PWM Grove kết nối tới GPIO/BCM pin12(PWM0) và GPIO/BCM pin13(PWM1), là hardware PWM pin của Raspberry Pi, ngoài ra, bạn có thể sử dụng tất cả các chân GPIO như soft PWM pin.

!!!Chú ý
	- Tất cả số chân của lớp silkscreen ngoài cổng Grove là số pin BCM. Sự khách biệt giữa BCM pins và physical pins vui lòng tham khảo [tại đây](https://www.raspberrypi.org/forums/viewtopic.php?p=726435)
	
	- So với PWM hardware, software PWM không chính xác và sẽ gặp sự cố ở tần số cao.

	- GPIO/BCM pin18 được đánh dấu là PWM0, thực tế GPIO/BCM 12 và GPIO/BCM 18 chia sẻ cùng một kênh PWM, vì vậy chúng không thể được đặt ở tốc độ khác nhau.

	- Đầu ra giắc âm thanh cũng sử dụng PWM 0 và PWM 1, vì vậy bạn không thể có đầu ra âm thanh trên cổng đó và sử dụng các PWM cùng một lúc.

UART: Cổng Grove UART kết nối với GPIO14(UART0 TX) và GPIO15(UART0 RX). UART thường được sử dụng trên Pi như một cách thuận tiện để điều khiển nó trên GIPO, hoặc truy cập các thông điệp khởi động hạt nhân từ bản điều khiển nối tiếp (được bật theo mặc định). Nó có thể được sử dụng giống như cách để giao tiếp với Arduino, bootloaded ATmega, ESP8266, vv với Pi của bạn.

Digital：Có 6 digital Grove sockets trên mạch này, thông thường dây màu vàng (kết nối với chân trên của ổ Grove socket 4 chân) của cáp Grove là dây tín hiệu, vì vậy chúng tôi đặt tên cho các cổng digital Grove D5/D16/D18/D22/D24/D26.

Analog：Như chúng ta biết, Raspberry Pi không có ADC, vì vậy nó không thể hoạt động trực tiếp với cảm biến analog. Giờ đây với sự giúp đỡ của MCU STM32 được tích hợp sẵn, Grove base hat có thể hoạt động như một bộ ADC 12 bit bên ngoài, có nghĩa là bạn có thể sử dụng cảm biến analog với Raspberry Pi. Điều thú vị hơn nữa là không chỉ có một mà là bốn analog Grove sockets. Cảm biến analog đặt điện áp analog vào ADC 12 bit. Sau khi ADC chuyển đổi dữ liệu analog thành dữ liệu digital, nó sẽ gửi dữ liệu digital vào Raspberry Pi thông qua giao diện I2C.

I2C：Có 3 cổng I2C trên mạch, tất cả được kết nối trực tiếp với chân I2C của raspberry. Bạn có thể coi phần này như trung tâm I2C. Hầu hết các module grove mới của seeed có giao diện I2C, bạn có thể thấy 3 cổng này rất hữu ích.

SWD： Chúng tôi sử dụng cổng SWD để ghi firmware cho hat. Ngoài ra, bạn có thể thấy 3 chân GPIO trong phần này, tức là, chân 9/ chân 10/ chân 11. Ba chân đó không thể sử dụng bởi bất kỳ cổng Grove nào, bạn có thể tự do sử dụng chúng mà không phải lo lắng về xung đột chân.

#### Các module Grove


**[Grove - Buzzer](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/buzzer.jpg)

Module này sử dụng piezo buzzer làm thành phần chính, nó có thể tạo ra âm cao trong khi nó kết nối với đầu ra digital và mức logic cao, nếu không nó có thể tạo ra các âm khác nhau theo tần số được tạo ra từ đầu ra Analog PWM được kết nối với nó. (lưu ý: Dải tần mà tai người bình thường có thể phân biệt là từ 20Hz đến 20kHz.)

**[Grove - Red LED Button](https://www.seeedstudio.com/Grove-Red-LED-Button-p-3096.html)**



![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/LEDButton.jpg)

Grove - LED Button gồm Grove - Yellow Button, Grove - Blue LED Button và Grove - Red LED Button. Nút này ổn định và đáng tin cậy với vòng đời 100000 lần. Với đèn LED tích hợp, bạn có thể áp dụng nó cho nhiều dự án thú vị, thực sự hữu ích khi sử dụng LED để hiển thị trạng thái của nút.

**[Grove - Light Sensor](https://www.seeedstudio.com/Grove-Light-Sensor-v1-2-p-2727.html)**


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lightsensor.jpg)

Grove - Light sensor tích hợp một quang điện trở (điện trở phụ thuộc ánh sáng) để phát hiện cường độ ánh sáng. Điện trở của quang điện trở giảm khi cường độ ánh sáng tăng. Một chip OpAmp kép LM58 trên mạch tạo ra điện áp tương ứng với cường độ ánh sáng (tức là dựa trên giá trị điện trở). Tín hiệu đầu ra là giá trị tương tự, ánh sáng càng sáng thì giá trị càng lớn.


**[Grove - Moisture Sensor](https://www.seeedstudio.com/Grove-Moisture-Sensor-p-955.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/Moisture_sensor.jpg)

Moisture Senor có thể được sử dụng để phát hiện độ ẩm của đất hoặc phán đoán nếu có nước xung quanh cảm biến, hãy để cây trong vườn của bạn có thể tìm sự giúp đỡ của con người khi chúng thiếu nước. Cảm biến này rất dễ sử dụng, bạn chỉ cần cắm vào đất và đọc dữ liệu. Với cảm biến này, bạn có thể tạo một dự án nhỏ và để cây gửi tin nhắn cho bạn như "Tôi đang thiếu nước, xin hãy tưới nước cho tôi".

**[Grove - mini PIR motion sensor](https://www.seeedstudio.com/Grove-mini-PIR-motion-sensor-p-2930.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/miniPIR.jpg)

Grove - mini PIR motion sensor cho phép bạn cảm nhận chuyển động, thường là chuyển động của con người trong phạm vi của nó. Chỉ cần kết nối nó với Grove - Base Shield  và lập trình cho nó, khi bất kỳ ai di chuyển trong phạm vi phát hiện của nó, đầu ra của cảm biến sẽ ở mức cao trên chân SIG.


**[Grove - Servo](https://www.seeedstudio.com/Grove-Servo-p-1241.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/Servo.jpg)

Grove - Servo là động cơ DC với hệ thống bánh răng và phản hồi. Nó sử dụng trong cơ chế lái của robot. Module là một sản phẩm thưởng cho những người yêu thích Grove. Chúng tôi đã điều chỉnh servo ba dây thành một đầu nối tiêu chuẩn Grove. Bạn có thể cắm và sử dụng nó như một module Grove điển hình, mà không có các dây nhảy phức tạp.

**[Grove - Temperature & Humidity Sensor （DHT11）](https://www.seeedstudio.com/Grove-Temperature-Humidity-Sensor-DHT1-p-745.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/DHT11.jpg)

Temperature & humidity sensor cung cấp một đầu ra digital được hiệu chuẩn trước. Một phần tử cảm biến điện dung duy nhất đo độ ẩm tương đối và nhiệt độ được đo bằng nhiệt điện trở hệ số âm (NTC). Nó có độ tin cậy cao và ổn định lâu dài. Xin lưu ý rằng cảm biến này sẽ không hoạt động ở nhiệt độ dưới 0 độ. 

**[Grove - Relay](https://www.seeedstudio.com/Grove-Relay-p-769.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/Relay.jpg)

Module Grove-Relay là một công tắc digital thường mở. Thông qua nó, bạn có thể điều khiển  mạch điện áp cao với điện áp thấp, giả sử 5V trên bộ điều khiển. Có một đèn LED báo trên mạch, đèn sẽ sáng lên khi các thiết bị đầu cuối được điều khiển đóng lại. 

**[Grove - Ultrasonic Ranger](https://www.seeedstudio.com/Grove-Ultrasonic-Ranger-p-960.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/Ultrasonic.jpg)

Grove - Ultrasonic ranger là module đo khoảng cách không tiếp xúc, hoạt động ở tần số 40KHz. Khi chúng ta cung cấp tín hiệu kích hoạt xung với hơn 10uS qua chân đơn, Grove - Ultrasonic ranger sẽ phát ra 8 chu kì với tần số 40kHz và phát hiện tiếng vang. Độ rộng xung của tính hiệu dội lại tỷ lệ với khoảng cách đo được với công thức: Khoảng cách = echo signal high time * Sound speed (340M/S)/2. Grove_Ultrasonic_Ranger's trig và echo singal chia sẻ 1 chân SIG.


**[Grove - 16 x 2 LCD (White on Blue)](https://www.seeedstudio.com/Grove-16-x-2-LCD-White-on-Blu-p-3196.html)**

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lcd.jpg)

Module Grove – 16x2 LCD  là màn hình LCD 16 ký tự 2 dòng, nó sử dụng giao diện bus I2C để giao tiếp với development board, do đó những điều này giảm pin header từ 10 xuống 2, thuận tiện cho Grove system. LCD cũng hỗ trợ tùy chỉnh các ký tự, bạn có thể tạo và hiển thị biểu tượng trái tin hoặc hình người trên module này thông qua cấu hình code đơn giản.

## GETTING STARTED 

### Minimum Requirement 

- Cáp micro USB
- Raspberry Pi
- SD card
- Grove Base Kit for Raspberry Pi

### Hướng dẫn cơ bản

#### Thiết lập cơ bản Arduino IDE

#### Làm thế nào để ghi một hình ảnh Raspbian 

**1. Raspbian Stretch download**

Download [Raspbian Stretch](https://www.raspberrypi.org/downloads/raspbian/) từ trang web chính thức của Raspberry Pi và chọn nhóm với desktop và phần mềm được đề xuất.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss0.png)

**2. Win32 Disk Imager**

- Download [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/) từ trang Sourceforge Project dưới dạng tệp cài đặt và chạy nó để cài đặt phần mềm. 

- Lắp thẻ SD vào đầu đọc thẻ SD và kết nối với PC của bạn.

- Chạy Win32DiskImager từ desktop hoặc menu.

- Trong device box, chọn ký tự ổ đĩa tương ứng của thẻ SD. Hãy cẩn thận để chọn đúng ổ đĩa: nếu bạn chọn sai ổ đĩa bạn có thể bị mất dữ liệu trên đĩa cứng của máy tính! Nếu bạn đang sử dụng khe cắm thẻ SD trong máy tính của mình và không thể thấy Win32DiskImager, hãy thử sử dụng bộ chuyển đổi SD bên ngoài.

- Click 'Write' và chờ nó viết xong.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss1.png)

- Hoàn thành.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss2.png)

- Thoát khỏi màn hình và eject SD card.

#### Cấu hình cơ bản

**Kết nối không dây và SSH**

**1.** Tạo một tệp có tên "wpa_supplicant.conf" vào thư mục /boot và copy code sau đây.


```txt
country=CN
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
 
network={
ssid="WiFi-name"
psk="WiFi-password"
key_mgmt=WPA-PSK
priority=1
}
```

!!!Chú ý

	Tên và mật khẩu Wifi phải giống Wi-Fi cục bộ mà PC của bạn kết nối với (đảm bảo PC và Raspberry Pi của bạn nằm trong cùng một mạng LAN).


**2.** Tạo file trống với tên "ssh" vào thư mục /boot.

**3.** Thêm SD Card với Raspbian vào Raspberry Pi

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/sd_card.jpg)

**4.** Kết nối Raspberry Pi tới nguồn và bật nó lên.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/power.jpg)

**5.** Mở putty để kết nối PC với Raspberry Pi. 

Download putty： [https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss3.png)


**Raspberry Pi**
Default username : pi
Default password : raspberry

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss4.jpg)

**VNC Configuration**

**1.** Mở raspi-config bằng cách gõ lệnh sau trong terminal.

```bash
sudo raspi-config
```

Ấn mũi tên xuống 5 interfacing Options và ấn "enter" để lựa chọn.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss5.png)

Ấn mũi tên xuống đến P3 VNC và ấn "enter" để lựa chọn.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss6.png)

Chọn "Yes" để kích hoạt nó.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss7.png)

Chọn "Ok".

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss8.png)

**2. ** Cài đặt VNC Viewer

Downloadr [VNC Viewe](https://www.realvnc.com/en/connect/download/viewer/)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss9.png)

Mở VNC Viewer và ấn địa chỉ  IP của Raspberry Pi. Bạn có thể tìm thấy địa chỉ IP bằng cách gõ lệnh ++ifconfig++ trong terminal của Raspberry Pi (hoặc bạn có thể nhập raspberrypi.local). 

!!!Chú ý

		Nếu bạn sử dụng raspberrypi.local để đăng nhập Pi của mình, bạn nên đảm bảo chỉ có một Raspberry Pi được sử dụng trong LAN.

Nhập default user name và password, và bạn có thể nhập Raspberry Pi's remote desktop!


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss10.png)

Thành công!

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss11.PNG)

**Cấu hình Base Hat**

**1.** Shutdown the Raspberry Pi

```bash
sudo shutdown -h now
```


Cắm Grove Base Hat cho Raspberry Pi vào Raspberry Pi.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/pi&hat.jpg)

**2.** Cấp nguồn Raspberry Pi với micro-usb cable để kích hoạt I2C

Mở raspi-config bằng cách đánh lệnh dưới vào terminal.

```bash
sudo raspi-config
```

Di chuyển xuống 5 interfacing Options và ấn "enter" để lựa chọn.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss5.png)

Di chuyển xuống P5 I2C và ấn "enter" để lựa chọn.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss13.png)

Chọn "Yes" để kích hoạt.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss14.png)

Chọn "Ok".

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss15.png)

Chọn "Finish" để lưu các thay đổi.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss16.png)

**3.** Cài đặt bằng một cú nhấp chuột, quick start, bất cứ khi nào bạn gọi, với lệnh duy nhất bên dưới. 

```bash
curl -sL https://github.com/Seeed-Studio/grove.py/raw/master/install.sh | sudo bash -s -
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ss12.PNG)

Nếu mọi thứ ổn, bạn sẽ thấy thông báo sau.

```bash
Successfully installed grove.py-0.6
#######################################################
Lastest Grove.py from github install complete   !!!!!
#######################################################
```

**4.** Bên cạnh cài đặt bằng one-click, bạn cũng có thể [cài đặt tất cả phụ thuộc](https://github.com/Seeed-Studio/grove.py#installation)).

                            
**5.** Sao chép thư viện python.py mới nhất.

```bash
git clone https://github.com/Seeed-Studio/grove.py
```


### Grove – LED button demo

Sau khi thiết lập cơ bản Raspberry Pi, giờ đây chúng ta có thể chạy mã demo LED. Lưu ý: Bạn nên hoàn thành các bước trên để tiếp tục bước sau.

**Kết nối Hardware**

Bước 1: Kết nối Grove - Red LED Button với cổng D5 Base Hat

Bước 2: Thêm Base Hat vào Raspberry Pi

Bước 3: Kết nối Raspberry Pi đến nguồn điện bằng cáp micro USB. 

![](![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/LEDbutton.png)
	
**Upload Code**

Bước 1: Chạy lệnh sau để tạo file python


```bash
cd grove.py
nano example.py
```

Bước 2: Sao chép code dưới vào file python

!!!Cảnh báo
	
	Vui lòng đảm bảo text editor ở dạng unix.


```python
#!/usr/bin/env python

import time
from grove.grove_ryb_led_button import GroveLedButton

def main():
    ledbtn = GroveLedButton(5)
    
    while True:
        ledbtn.led.light(True)
        time.sleep(1)
        
        ledbtn.led.light(False)
        time.sleep(1)

if __name__ == '__main__':
    main()
```

Bước 3：Chạy chương trình

```bash
sudo chmod +x  example.py
sudo ./example.py
```

Khi bạn click một nào vào LED button, LED sẽ chuyển sang chế độ "BẬT","TẮT" nếu bạn nhấn và giữ lâu. Nếu bạn click hai lần vào LED button, đèn LED sẽ nhấp nháy.

```bash
pi@raspberrypi:~/grove.py $ sudo ./example.py
turn on  LED
turn on  LED
turn off LED
turn on  LED
blink    LED
^CTraceback (most recent call last):
  File "./example.py", line 17, in <module>
    main()
  File "./example.py", line 14, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $ 
```

**Explanation of the blink code**

Trong python, khi các module được tham chiếu với nhau, các module khác có thể định nghĩa "__main__" khác nhau, và chỉ có thể có một chương trình trong mỗi lần. Việc lựa chọn chương trình nhập tùy thuộc vào giá trị của __name__. "if__name__=='__main__'" bằng nhau, có nghĩa đó là mục nhập của mô phỏng python.


```python
if __name__ == '__main__':
    main()
```

## Grove Base Kit for Raspberry Pi

 Bây giờ, bạn đã sẵn sàng để khám phá Grove system? Chúng tôi đã thiết kế 8 hướng dẫn để bạn bắt đầu với một số module Grove cơ bản. Phần này giới thiệu cho bạn các module có thể được kết hợp và áp dụng cho các ứng dụng thực tế.


###  Prerequisite

Để bắt đầu với hướng dẫn Grove, bạn cần có kiến thức cơ bản về ngôn ngữ lập trình Raspberry Pi và Python. Vui lòng đảm bảo rằng bạn đã hoàn thành hướng dẫn thiết lập cơ bản ở trên thành công và hoàn thành bản demo LED Blink và đảm bảo nó hoạt động hoàn toàn với Raspberry Pi và  Grove Base Hat.
 

###  Learning outcome 

- Có thể sử dụng Grove Base Hat để xây dựng các ứng dụng với các module Grove.
- Có thể làm rõ từng thành phần của Grove Starter Kit và sử dụng module có liên quan các dự án của riêng bạn sau hướng dẫn này
- Có thể xác định loại module có trong Kit và ứng dụng của chúng.
- Hiểu sự khác biệt giữa tín hiệu analog và tín hiệu digital.


### Lesson 1: Buzzer

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/buzzer.jpg)

**Objective**	

Sử dụng buzzer để tạo ra một số âm thanh và cũng đặt tần số cụ thể để tạo ra một số âm điệu.


**Yêu cầu phần cứng**

Tự chuẩn bị 

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer


Bao gồm trong kit

- Grove Base Hat
- Cáp Grove
- Grove – Buzzer 


**Kết nối Hardware**

**Bước 1.** Sử dụng cáp Grove để kết nối Grove - Buzzer với cổng PWM của Base Hat và chèn Hat vào Raspberry Pi.

**Bước 2.** Kết nối Raspberry Pi tới nguồn điện bằng cáp micro USB. 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/buzzer&pi.jpg)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo rằng bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy các lệnh sau để tạo file python

```bash
cd grove.py
nano lesson_1.py
```

Bước 2: Copy code dưới đây

```python
#!/usr/bin/env python
import time
from mraa import getGpioLookup
from upm import pyupm_buzzer as upmBuzzer

def main():
    # Grove - Buzzer connected to PWM port
    buzzer = upmBuzzer.Buzzer(getGpioLookup('GPIO12'))
    
    CHORDS = [upmBuzzer.BUZZER_DO, upmBuzzer.BUZZER_RE, upmBuzzer.BUZZER_MI, 
        upmBuzzer.BUZZER_FA, upmBuzzer.BUZZER_SOL, upmBuzzer.BUZZER_LA, 
        upmBuzzer.BUZZER_SI]
    for i in range(0, len(CHORDS)):
        buzzer.playSound(CHORDS[i], 500000)
        time.sleep(0.1)
    
    del buzzer
    print('application exiting...')

if __name__ == '__main__':
    main()
```


Step 3：Chạy chương trình

```bash
sudo chmod +x lesson_1.py
sudo ./lesson_1.py
```

Nếu mọi thứ ổn, bạn nên chú ý buzzer đang tạp ra âm thanh “Do Re Mi Fa So La Si”.

	

### Lesson 2: Red LED Button

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/LEDButton.jpg)


**Objective**	

Sử dụng Grove - Red LED Button để điều khiển nhấp nháy của LED và để Grove - Buzzer tạo các hiệu ứng âm thanh khác nhau.

**Yêu cầu phần cứng**

Tự chuẩn bị

- cáp micro-USB
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - Red LED Button
- Grove – Buzzer


**Kết nối phần cứng**

**Bước 1.** Sử dụng cáp Grove  để kết nối Grove - Buzzer tới cổng PWM và Grove - Red LED Button với D5 của Base Hat và chèn Hat vào Raspberry Pi.


**Bước 2.** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable. 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/Buzzer&Button.png)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh dưới để tạo file python

```bash
cd grove.py
nano lesson_2.py
```

Bước 2: Copy code dưới


```python	
#!/usr/bin/env python

import time
from mraa import getGpioLookup
from upm import pyupm_buzzer as upmBuzzer

from grove.button import Button
from grove.grove_ryb_led_button import GroveLedButton

def main():
    # Grove - LED Button connected to port D5
    button = GroveLedButton(5)
    
    # Grove - Buzzer connected to PWM port
    buzzer = upmBuzzer.Buzzer(getGpioLookup('GPIO12'))
    
    def on_event(index, event, tm):
        if event & Button.EV_SINGLE_CLICK:
            print('single click')
            button.led.light(True)
            buzzer.playSound(upmBuzzer.BUZZER_DO, 500000)
            
        elif event & Button.EV_LONG_PRESS:
            print('long press')
            button.led.light(False)
            buzzer.playSound(upmBuzzer.BUZZER_DO, 1000000)
            
    button.on_event = on_event
    
    while True:
        time.sleep(1)

if __name__ == '__main__':
    main()
```

Bước 3：Chạy chương trình

```bash	
sudo chmod +x lesson_2.py
sudo ./lesson_2.py
```

!!!Success
		Nếu mọi thứ ổn, bạn sẽ thấy rằng khi bạn giữ LED button, đèn LED sẽ tắt và buzzer sẽ phát ra âm thanh "Do" dài. Tuy nhiên khi bạn ấn một lần, đèn LED sẽ sáng và còi sẽ phát ra âm thanh "Do" ngắn. 


```bash
pi@raspberrypi:~/grove.py $ sudo ./lesson_2.py
single click
single click
single click
long press
single click
long press
long press
Traceback (most recent call last):
  File "./lesson2.py", line 34, in <module>
    main()
  File "./lesson2.py", line 31, in main
    time.sleep(1)
KeyboardInterrupt
^Cpi@raspberrypi:~/grove.py $ 
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/LED&Buz_demo.jpg)


### Lesson 3: Light Sensor

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lightsensor.jpg)


**Objective**	

Trong bài này, chúng tôi sẽ chỉ cho bạn cách sử dụng Grove - Light Sensor để điều khiển Grove - Servo. Trong trường hợp này, góc quay servo thay đổi theo cường độ ánh sáng. 

**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - Light Sensor
- Grove - Servo

**Kết nối phần cứng**

**Bước 1** Kết nối Grove - Light Sensor tới cổng A0，Grove - Servo tới cổng PWM.

**Bước 2** Thêm Base Hat vào Raspberry Pi.

**Bước 3** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable. 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/servo&light.png)


**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh dưới để tạo file python


```bash
cd grove.py
nano lesson_3.py
```

Bước 2: Copy code dưới

```python	
#!/usr/bin/env python

import time

from grove.grove_servo import GroveServo
from grove.grove_light_sensor_v1_2 import GroveLightSensor

def main():
    # Grove - Servo connected to PWM port
    servo = GroveServo(12)

    # Grove - Light Sensor connected to port A0
    sensor = GroveLightSensor(0)

    while True:
        angle = sensor.light * 180 / 1000
        print('light value {}, turn to {} degree.'.format(sensor.light, angle))
        servo.setAngle(angle)

        time.sleep(1)

if __name__ == '__main__':
    main()
```



Step 3：Chạy chương trình


```bash
sudo chmod +x lesson_3.py
sudo ./lesson_3.py
```

Nếu mọi thứ thuận lợi, sự thay đổi cường độ ánh sáng sẽ dẫn đến góc quay khác nhau của servo.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/light_on&off.jpg)



```bash
pi@raspberrypi:~/grove.py $ sudo ./lesson_3.py
light value 300, turn to 113 degree.
light value 80, turn to 80 degree.
light value 166, turn to 165 degree.
light value 498, turn to 132 degree.
light value 601, turn to 60 degree.
light value 200, turn to 21 degree.
light value 459, turn to 99 degree.
light value 172, turn to 173 degree.
light value 319, turn to 138 degree.
^CTraceback (most recent call last):
  File "./lesson3.py", line 23, in <module>
    main()
  File "./lesson3.py", line 20, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $ 
```

### Lesson 4: Motion Sensor & Relay

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/pir+relay.jpg)


**Objective**	

Sử dụng Grove - mini PIR motion sensor để phát hiện chuyển động, đèn bật nếu có người đến.

**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable 
- Grove - mini PIR motion sensor
- Grove - Relay

**Kết nối phần cứng**

**Bước 1** Kết nối Grove - mini PIR motion sensor tới cổng D5, Grove - Relay tới cổng D16 của Base Hat.

**Bước 2** Thêm Base Hat vào Raspberry Pi


**Bước 3** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable.


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/pir&relay.png)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh sau để tạo file python

```bash
cd grove.py
nano lesson_4.py
```


Bước 2: Copy code dưới

```python	
#!/usr/bin/env python

import time

from grove.grove_mini_pir_motion_sensor import GroveMiniPIRMotionSensor
from grove.grove_relay import GroveRelay

def main():
    # Grove - mini PIR motion sensor connected to port D5
    sensor = GroveMiniPIRMotionSensor(5)
    
    # Grove - Relay connected to port D16
    relay = GroveRelay(16)
    
    def on_detect():
        print('motion detected')
        
        relay.on()
        print('relay on')
        
        time.sleep(1)
        
        relay.off()
        print('relay off')
    
    sensor.on_detect = on_detect
    
    while True:
        time.sleep(1)

if __name__ == '__main__':
    main()
```

Step 3：Chạy chương trình

```bash	
sudo chmod +x lesson_4.py
sudo ./lesson_4.py
```

Nếu mọi thử thuận lợi, bạn If everything goes well, bạn sẽ thấy bật / tắt relay một khi nó phát hiện ra một chuyển động.

```bash	
pi@raspberrypi:~/grove.py $ sudo ./lesson_4.py
motion detected
relay on
relay off
motion detected
relay on
relay off
^CTraceback (most recent call last):
  File "./lesson_4.py", line 33, in <module>
    main()
  File "./lesson_4.py", line 30, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $ 
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/pir_light.jpg)

### Lesson 5: Ultrasonic Sensor & Relay


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ultra+relay.jpg)


**Objective**	

Trong bài học này, chúng ta sử dụng Grove - Ultrasonic Ranger để phát hiện khoảng cách, khi ai đó đến gần, ánh sáng trên Grove - Relay sẽ được "BẬT". 


**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - Ultrasonic Ranger
- Grove - Relay

**Kết nối phần cứng**

**Bước 1** Kết nối Grove - Ultrasonic Ranger tới cổng D5, Grove - Relay tới cổng D16 của Base Hat.

**Bước 2** Thêm Base Hat vào Raspberry Pi


**Bước 3** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ultra&relay.png)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh dưới để tạo file python 

```bash
cd grove.py
nano lesson_5.py
```

Bước 2: Copy code dưới

```python	
#!/usr/bin/env python

import time

from grove.grove_relay import GroveRelay
from grove.grove_ultrasonic_ranger import GroveUltrasonicRanger

def main():
    # Grove - Ultrasonic Ranger connected to port D5
    sensor = GroveUltrasonicRanger(5)
    
    # Grove - Relay connected to port D16
    relay = GroveRelay(16)
    
    while True:
        distance = sensor.get_distance()
        print('{} cm'.format(distance))
        
        if distance < 20:
            relay.on()
            print('relay on')
            
            time.sleep(1)
            
            relay.off()
            print('relay off')
            
            continue
        
        time.sleep(1)

if __name__ == '__main__':
    main()
```


Bước 3：Chạy chương trình

```bash
sudo chmod +x lesson_5.py
sudo ./lesson_5.py
```

Nếu mọi thứ thuận lợi, sự thay đổi cường độ ánh sáng sẽ dẫn đến góc quay khác nhau của servo.


```bash	
pi@raspberrypi:~/grove.py $ sudo ./lesson_5.py
253.722585481 cm
253.739028141 cm
252.896341784 cm
1.20442489098 cm
relay on
relay off
4.51762100746 cm
relay on
relay off
253.985668051 cm
^CTraceback (most recent call last):
  File "./lesson_5.py", line 34, in <module>
    main()
  File "./lesson_5.py", line 31, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $ 
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/ultra_light.jpg)

Bây giờ, so sánh kết quả từ bài 4 và bài 5, bạn có thể liệt kê những ưu và nhược điểm của Grove - mini PIR motion sensor và Grove Ultrasonic Ranger?


### Lesson 6:  LCD

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lcd.jpg)


**Objective**	

Sử dụng Grove - 16*2 LCD screen để hiển thị “Hello World”. 

**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - 16*2 LCD


**Kết nối phần cứng**

**Bước 1** Kết nối Grove - 16*2 LCD tới cổng I2C của Base Hat.

**Bước 2** Thêm Base Hat vào Raspberry Pi.

**Bước 3** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable. 

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/LCD.png)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh dưới để tạo file python


```bash	
cd grove.py
nano lesson_6.py
```

Bước 2: Copy code dưới


```python	
#!/usr/bin/env python

import time

from grove.display.jhd1802 import JHD1802

def main():
    # Grove - 16x2 LCD(White on Blue) connected to I2C port
    lcd = JHD1802()

    lcd.setCursor(0, 0)
    lcd.write('hello, world!!!')

    print('application exiting...')

if __name__ == '__main__':
    main()
```


Step 3：Chạy chương trình


```bash
sudo chmod +x lesson_6.py
sudo ./lesson_6.py
```

Bạn sẽ thấy “hello, world!!!” được hiển thị trên LCD screen.


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/helloworld.jpg)


Nếu bạn muốn sử dụng Grove - 16*2 LCD screen để hiển thị ký tự khác, bạn có thể thay đổi ++ lcd.write('hello, world!!!')++ trong code. 


### Lesson 7: LCD & Temperature and Humidity Sensor


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lcd+dht11.jpg)


**Objective**	

Sử dụng Grove - 16*2 LCD screen để hiển thị dữ liệu (nhiệt độ và độ ẩm) từ Grove - Temperature and Humidity Sensor

**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - 16*2 LCD
- Grove - Temperature and Humidity Sensor

**Kết nối phần cứng**

**Bước 1** Kết nối Grove - 16*2 LCD tới cổng I2C，Grove - Temperature and Humidity Sensor tới cổng D5.

**Bước 2** Thêm Base Hat vào Raspberry Pi.

**Bước 3** Kết nối Raspberry Pi tới nguồn điện bằng micro USB cable. 


![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/DHT11&LCD.png)

**Lập trình phần mềm**	

!!!Chú ý

	Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh sau để tạo file python

```bash	
cd grove.py
nano lesson_7.py
```

Bước 2: Copy code dưới

```python	
#!/usr/bin/env python

import time

from grove.grove_temperature_humidity_sensor import DHT
from grove.display.jhd1802 import JHD1802

def main():
    # Grove - 16x2 LCD(White on Blue) connected to I2C port
    lcd = JHD1802()

    # Grove - Temperature&Humidity Sensor connected to port D5
    sensor = DHT('11', 5)

    while True:
        humi, temp = sensor.read()
        print('temperature {}C, humidity {}%'.format(temp, humi))

        lcd.setCursor(0, 0)
        lcd.write('temperature: {0:2}C'.format(temp))

        lcd.setCursor(1, 0)
        lcd.write('humidity: {0:5}%'.format(humi))

        time.sleep(1)

if __name__ == '__main__':
    main()
```

Step 3：Chạy chương trình

```bash
sudo chmod +x lesson_7.py
sudo ./lesson_7.py
```

Nếu mọi thứ thuận lợi, bạn sẽ thấy nhiệt độ và độ ẩm hiện tại hiển thị trên LCD screen 


```bash
pi@raspberrypi:~/grove.py $ sudo ./lesson_7.py
temperature 23C, humidity 16%
temperature 22C, humidity 17%
temperature 22C, humidity 17%
^CTraceback (most recent call last):
  File "./lesson_7.py", line 28, in <module>
    main()
  File "./lesson_7.py", line 25, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/temp&humi_LCD.jpg)


### Lesson 8: LCD & Moisture Sensor & Buzzer

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lcd+moisture+buzzer.jpg)

**Objective**	

Sử dụng Grove - 16 * 2 LCD để hiển thị mức độ ẩm hiện tại. Khi trạng thái độ ẩm là "wet",  Grove - Buzzer sẽ cảnh báo bạn. 

**Yêu cầu phần cứng**

Tự chuẩn bị

- micro-USB cable
- Raspberry Pi 3 Model B
- Computer

Bao gồm các kit

- Grove Base Hat
- Grove cable
- Grove - 16*2 LCD
- Grove - Moisture Sensor
- Grove - Buzzer

**Kết nối phần cứng**

**Bước 1** Kết nối Grove - 16*2 LCD tới cổng I2C, Grove - Moisture Sensor tới cổng A0 và Grove - Buzzer tới cổng PWM của Grove Base Hat. 

**Bước 2** Thêm Base Hat tới Raspberry Pi. 


**Bước 3**  Sử dụng micro USB để kết nối Raspberry Pi với PC.

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lesson8.png)

**Lập trình phần mềm**	

!!!Chú ý

		Vui lòng đảm bảo bạn đã sao chép thư viện lưu trữ python.py vào Raspberry Pi.

Bước 1: Chạy lệnh dưới để tạo file python

```bash
cd grove.py
nano lesson_8.py
```

Bước 2： Copy code dưới

```python	
#!/usr/bin/env python

import time
from mraa import getGpioLookup
from upm import pyupm_buzzer as upmBuzzer

from grove.grove_moisture_sensor import GroveMoistureSensor
from grove.lcd.sh1107g import JHD1802

def main():
    # Grove - 16x2 LCD(White on Blue) connected to I2C port
    lcd = JHD1802()
    
    # Grove - Moisture Sensor connected to port A0
    sensor = GroveMoistureSensor(0)
    
    # Grove - Buzzer connected to port PWM
    buzzer = upmBuzzer.Buzzer(getGpioLookup('GPIO12'))
    
    while True:
        mois = sensor.moisture
        if 0 <= mois and mois < 300:
            level = 'dry'
        elif 300 <= mois and mois < 600:
            level = 'moist'
        else:
            level = 'wet'
            buzzer.playSound(upmBuzzer.BUZZER_DO, 200000)
        
        print('moisture: {}, {}'.format(mois, level))
        
        lcd.setCursor(0, 0)
        lcd.write('moisture: {0:>6}'.format(mois))
        
        lcd.setCursor(1, 0)
        lcd.write('{0:>16}'.format(level))
        
        time.sleep(1)

if __name__ == '__main__':
    main()
```


Bước 3：Chạy chương trình

```bash
sudo chmod +x lesson_8.py
sudo ./lesson_8.py
```

Nếu mọi thứ thuận lợi, bạn sẽ có thể thấy mức độ ẩm trên LCD screen. Buzzer được sử dụng để cảnh báo mọi người khi mức độ ẩm đạt đến "wet". 


```bash	
pi@raspberrypi:~/grove.py $ sudo ./lesson_8.py
moisture: 0, dry
moisture: 0, dry
moisture: 396, moist
moisture: 398, moist
moisture: 407, wet
moisture: 418, wet
^CTraceback (most recent call last):
  File "./lesson_8.py", line 41, in <module>
    main()
  File "./lesson_8.py", line 38, in main
    time.sleep(1)
KeyboardInterrupt
pi@raspberrypi:~/grove.py $
```

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Beginner_Kit_for_RaspberryPi/master/img/lesson8.png)

## TECH SUPPORT

Xin đừng ngần ngại gửi vấn đề vào [diễn đàn](https://forum.seeedstudio.com/) của chúng tôi hoặc gửi thư đến [techsupport@seeed.cc](techsupport@seeed.cc).<br /><p style="text-align:center"><a href="https://www.seeedstudio.com/act-4.html?utm_source=wiki&utm_medium=wikibanner&utm_campaign=newproducts" target="_blank"><img src="https://github.com/SeeedDocument/Wiki_Banner/raw/master/new_product.jpg" /></a></p>