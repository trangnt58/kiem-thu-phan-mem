#Bài toán
Tìm ước chung lớn nhất của 2 số
#Chạy chương trình:
```javascript
npm install mocha 
```
```javascript
mocha 
```

#Phương pháp kiểm thử
Phương pháp kiểm thử tốt nhất: Kiểm thử biên mạnh kết hợp kiểm thử lớp tương đương, vì: 
- vì các biến là vật lý và độc lập với nhau
- cần bắt ngoại lệ cho trường hợp vượt quá giá trị của kiểu Number
- kiểm thử được hết các trường hợp có thể xảy ra với 2 biến đầu vào: lớn hơn, nhỏ hơn, bằng nhau

#Áp dụng kiểm thử
##Kiểm thử biên mạnh
- Test với các giá trị Number.MAX_VALUE + 1, Number.MAX_VALUE, Number.MAX_VALUE - 1
- Test với các giá trị Number.MIN_VALUE + 1, Number.MIN_VALUE, Number.MIN_VALUE - 1

##Kiểm thử tương đương
Xác định các lớp tương đương
- R1: a < b với a, b thuộc Z
- R2: a > b với a, b thuộc Z
- R3: a = b với a, b thuộc Z
- R4: a, b không phải là số nguyên

|      | a  | b  | Kết quả mong đợi
| -----|----|----|-----------------
| TE1  | 12 | 16 | 4
| TE2  | 75 | 20 | 5
| TE3  | 2 | 2 | 2
| TE4  | '3' | 'abc' | false
