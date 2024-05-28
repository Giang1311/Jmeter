# JMeter
## Kiểm tra hiệu năng trang web
### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://wheelofnames.com.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://wheelofnames.com.
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:
![jmeter](https://github.com/Giang1311/Jmeter/assets/96896545/4a024182-1b6d-40ec-b048-45a2fcfc6dc9)

### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 998/1000 = 99,8%
- Số lượng yêu cầu thất bại: 2/1000 = 0,2%
- Thời gian phản hồi trung bình: 40 ms
- Thời gian phản hồi trung vị: 38 ms
- Thời gian phản hồi percentil 90: 70 ms
- Chuyển tải: 16 yêu cầu/giây
### Kết luận:

Trang web https://wheelofnames.com/ có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (99,8%), số lượng yêu cầu thất bại rất thấp (0,2%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web cũng khá cao (16 yêu cầu/giây).
### Hình ảnh tổng quát
![wheelofnames](https://github.com/Giang1311/Jmeter/assets/96896545/39d6439d-0363-4a47-8b60-a62d3ad87782)

## Kiểm tra hiệu năng API

### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://openweathermap.org/current
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:
![api](https://github.com/Giang1311/Jmeter/assets/96896545/9e0b6884-feec-4353-b3de-6527b8393cbe)


### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 996/1000 = 99,6%
- Số lượng yêu cầu thất bại: 4/1000 = 0,4%
- Thời gian phản hồi trung bình: 10
