# Test cases – FIT4012 Lab 1

Đánh dấu [x] khi đã chạy và kiểm tra kết quả.

## 1. Entropy / Redundancy
- [X] Input: `aaaa` -> entropy thấp, redundancy cao
- [X] Input: `abcd` -> entropy cao hơn `aaaa`
- [X] Input: `hello world` -> entropy và redundancy được tính hợp lệ

## 2. Modulo inverse
- [X] `a=3, m=7` -> nghịch đảo modulo là 5
- [X] `a=10, m=17` -> nghịch đảo modulo là 12
- [X] `a=6, m=9` -> không tồn tại nghịch đảo modulo

## 3. Ghi chú
- [X] Input: aB3$xQz9!mK#2Lp@ → entropy = 4, redundancy = 4 — ký tự đa dạng cho entropy cao nhất
- [X] Input: a=1, m=7 → nghịch đảo là 1 — 1 luôn là nghịch đảo của chính nó
- [X] Input: a=7, m=26 → nghịch đảo là 15 — test case thực tế trong mã Caesar mở rộng (26 ký tự)
- [X] Input: a=4, m=8 → không tồn tại — gcd(4, 8) = 4 ≠ 1
