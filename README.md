
# Projectile motion with drag

Tính toán khoảng cách mà viên đạn đi được trong môi trường có lực cản không khí.

Calculate the distance traveled by the bullet in the presence of air resistance.

# Tham Khảo

https://scipython.com/book2/chapter-8-scipy/examples/a-projectile-with-air-resistance/
https://web.physics.wustl.edu/~wimd/topic01.pdf?fbclid=IwAR3Zwo0cU_KoCJrgqzq66fBkkv5kP0vNlm6ADLTz-NKLtSbAsE3c_LC6qLY

sách : Learning Scientific Programming with Python

#
# Mô tả

Ở phiên bản đầu tiên, tôi cố gắng tạo ta một thứ gì đó có thể tính toán được khoảng cách di chuyển của viên đạn, với các thông số đầu vào như : khối lượng, vận tốc, hệ số cản, diện tích bề mặt....
ver 1 của chương trình hoạt động theo sơ đồ sau : 


![image](https://user-images.githubusercontent.com/54757285/182513132-8ea59a84-1e8a-42d7-ac62-213770739565.png)


# Ver 02
Ở phiên bản số 2 này, tôi muốn nó tự động tính toán góc bắn với thông số đầu vào là khối lượng, vận tốc, hệ số cản, diện tích bề mặt.... VÀ MỘT THÔNG SỐ MỚI : KHOẢNG CÁCH MÀ TÔI MUỐN NÓ ĐI ĐƯỢC
theo sơ đồ sau : 


![image](https://user-images.githubusercontent.com/54757285/183102240-63050f8e-ec9e-4c9c-b8ea-f7d182af2d72.png)


# Cách sử dụng 
Để sử dụng được chương trình bạn phải thêm các thông số đầu vào : 

![image](https://user-images.githubusercontent.com/54757285/183226206-de0fd12f-657a-4e2c-890f-a456cc5d5bfc.png)

#
#NẾU BẠN CHẠY TRÊN GOOGLE COLAB ĐỪNG QUÊN CHẠY LẠI CELL THÔNG SỐ ĐẦU VÀO TRƯỚC MỖI LẦN CHẠY, KHÔNG THỰC HIỆN VIỆC NÀY SẼ DẪN ĐẾN SAI LỆCH KẾT QUẢ
#

Sau đó, nếu chạy trên máy tính cá nhân với ide hãy gõ trong cmd "python tên file mà bạn lưu.py" và file python sẽ được chạy, trường hợp sử dụng notbook hoặc colab : chỉnh sửa thông số và chạy lần lượt từng cell


Đối với phiên bản số 2 : 

ĐỪNG QUÊN : đặt giá trị ang ở mục đầu thành 0 

![image](https://user-images.githubusercontent.com/54757285/183229682-d309eeca-0a50-4cfe-9eb2-71a23cbe0779.png)


tính toán đã được chỉnh sửa thành một hàm có tên là tinhtoan, nó nhận vào tham số phi0 vả trả về giá trị khoảng cách đi được aka X

![image](https://user-images.githubusercontent.com/54757285/183229513-be223cc6-1000-4d14-93a1-8c4111c88d53.png)

để sử dụng nó hãy tạo ra một vòng lặp => vòng lặp này xét giá trị trả về của hàm tinhtoan(), lặp lại cho đến khi giá trị đó bằng với giá trị khoảng cách mà bạn mong muốn, trong hình ảnh dưới đây tôi ví dụ mình muốn nó đi được 100 mét. 

![image](https://user-images.githubusercontent.com/54757285/183229571-b594baf3-d379-4f69-a3bf-49bb68a9391f.png)

khi mà giá trị trả về vẫn nhỏ hơn khoảng cách mong muốn => tăng góc bắn lên thêm 1 khoảng ở đây ví dụ là 0.1 độ bạn có thể đặt nó là gì tùy thích => nếu đạt khoảng cách nó sẽ dừng vòng lặp và trả về giá trị khoảng cách cũng như góc bắn.


## Dự định

- Tính được khoảng cách di chuyển

- Tính được góc bắn cần thiết để di chuyển 

- Đã hoàn thành nhưng tôi muốn nó có độ chính xác cao hơn, dự án sẽ còn được cập nhật tiếp.




