# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Bài lab giúp sinh viên hiểu và cài đặt hai khái niệm nền tảng trong mật mã học: entropy Shannon (đo lượng thông tin của một chuỗi ký tự) và modulo inverse (nghịch đảo theo modulo, dùng trong mã hóa như RSA, Caesar mở rộng). Qua đó, sinh viên luyện tập đọc hiểu code C++ có sẵn và bổ sung phần còn thiếu.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Toàn ký tự giống nhau -> không có thông tin, dư thừa tối đa |
| abcd | 2.0 | 6.0 | 4 ký tự phân bố đều → entropy trung bình, còn nhiều dư thừa |
| hello world | 2.845 | 5.155 | Ngôn ngữ tự nhiên → có ký tự lặp (l, o), dư thừa ~64% |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab này, em hiểu được cách tính entropy
Em cũng nắm được độ dư thừa là phần thông tin "lãng phí" so với trường hợp lý tưởng
Qua việc chạy thử với các chuỗi khác nhau, em thấy rõ chuỗi càng đa dạng ký tự thì entropy càng cao và độ dư thừa càng thấp. Điều này giúp em hiểu vì sao trong mật mã học, dữ liệu cần có entropy cao để khó bị tấn công phân tích tần suất.
