🍎 HỆ THỐNG PHÂN LOẠI QUẢ SỬ DỤNG CAMERA AI NHÚNG
🧠 Giới thiệu đề tài
Đây là một hệ thống nhúng thông minh giúp phân loại trái cây dựa trên AI. Bằng cách sử dụng camera kết hợp với mô hình nhận diện nhẹ, hệ thống có khả năng:

Phân loại trái cây dựa vào màu sắc, hình dạng.

Xác định độ chín, chất lượng sản phẩm.

Hiển thị kết quả ngay trên video trực tiếp.

Truyền dữ liệu lên web, cho phép theo dõi từ xa.

Thống kê, lưu trữ để hỗ trợ đánh giá và chăm sóc cây trồng.

👨‍💻 Nhóm thực hiện
STT	Họ và tên	Mã sinh viên
1	Kiều Bùi Đức Mạnh	B20DCDT129
2	Trần Thành Minh	B21DCDT151
3	Mai Thanh Sơn	B21DCDT192
4	Hoàng Việt Dũng	B21DCDT072
Ngành học: Công nghệ kỹ thuật Điện - Điện tử

🎯 Mục tiêu của hệ thống
Nhận diện trái cây theo từng loại, màu sắc, độ chín.

Tối ưu hóa để chạy tốt trên thiết bị nhúng như Raspberry Pi.

Xử lý và hiển thị hình ảnh thời gian thực.

Truyền và giám sát từ xa qua web.

Ghi lại và thống kê dữ liệu, hỗ trợ người dùng đưa ra quyết định nhanh chóng.

🛠️ Công nghệ và công cụ sử dụng
Thành phần	Công nghệ
Thiết bị nhúng	Raspberry Pi
Nhận diện AI	YOLOv5 / MobileNet
Xử lý hình ảnh	OpenCV, OpenGL
Giao diện người dùng	Flask Web App
Truyền dữ liệu	ThingSpeak, Web Dashboard
Giao tiếp phần cứng	Camera Pi, GPIO
📦 Cấu trúc thư mục dự án

fruit-ai-system/
├── ai_model/              # Mô hình đã huấn luyện
├── camera/                # Code xử lý camera, nhận diện
├── web_server/            # Giao diện web hiển thị kết quả
├── static/                # Hình ảnh và tài nguyên tĩnh
├── templates/             # HTML giao diện web
├── data_logger/           # Ghi log, lưu kết quả nhận diện
├── requirements.txt       # Các thư viện Python cần cài
├── README.md              # Mô tả dự án (file này)

⚙️ Hướng dẫn triển khai
1. Cài đặt môi trường

sudo apt update
sudo apt install python3-pip
pip3 install -r requirements.txt

3. Khởi động hệ thống
Chạy nhận diện camera:

cd camera
python3 main.py
Chạy web server:


cd web_server
python3 app.py

🧪 Kiểm thử hệ thống
✔️ Phân loại chính xác các loại trái cây: táo, chuối, xoài, cam,…

✔️ Phản hồi kết quả < 1 giây với video trực tiếp.

✔️ Hoạt động ổn định nhiều giờ liên tục trên Raspberry Pi.

✔️ Truyền kết quả nhận diện và hình ảnh lên web giám sát.

📚 Tài liệu tham khảo
Redmon et al., You Only Look Once: Unified, Real-Time Object Detection, arXiv:1506.02640

Howard et al., MobileNets: Efficient CNNs for Mobile Vision, arXiv:1704.04861

Kessenich et al., OpenGL Programming Guide, Addison-Wesley, 2016

Akenine-Möller et al., Real-Time Rendering, 4th ed, CRC Press, 2018

Nguyễn Ngọc Minh, Lương Công Duẩn, Ứng dụng học sâu nhận diện vật thể lạ trên đường băng, 2021
