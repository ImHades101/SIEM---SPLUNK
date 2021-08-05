# SIEM---SPLUNK
![image](https://user-images.githubusercontent.com/52188500/128276317-636c8e86-5a40-422f-b47d-24a1efa8b9f0.png)

## 1. Giới thiệu về lab
  Sử dụng Splunk để phát hiện tấn công hệ thống website như: XSS, SQL Injection, Code Injection, System Intrusion.
## 2. Các chức năng sử dụng trên Splunk
    Monitor: upload đường dẫn các file logs.</br>
    Search: tìm kiếm, phân tích, phát hiện tấn công.</br>
    Alert: gửi cảnh báo về telegram thông qua con bot telegram.</br>
    Dashboard: hiển thị dưới dạng biểu đồ và các thông số. Dễ dàng theo dõi và phát hiện các rủi ro kịp thời.
## 3. Thực hiện
  ### 3.1. Môi trường
    Sử dụng máy ảo Ubuntu 20.04 để cài đặt Splunk, webservice (trang bị hệ thống ghi logs vào /var/log/webvuln.log), audit log (/var/log/audit/audit.log).
    Sử dụng máy thật để tấn công, bằng cách sử dụng burpsuite để dể dàng bắt gói tin và tiến hành tấn công theo wordlist của các lỗ hổng tương ứng.
  ### 3.2. Luồng hoạt động của lab
    Sau khi kẻ tấn công thưc hiện tấn công vào trang web, hệ thống log của web sẽ ghi lại và splunk phân tích (search query) và gửi cảnh báo về ứng dụng telegram.
    Tiếp theo chung ta có thể vào dashboard trên splunk để dễ dàng theo dõi.
  
