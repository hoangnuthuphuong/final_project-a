# ỨNG DỤNG THỊ GIÁC MÁY TÍNH VÀ HỌC SÂU VÀO KIỂM TRA CHẤT LƯỢNG LON RỖNG TRONG DÂY CHUYỀN CÔNG NGHIỆP

## 📌 Mô tả đề tài

Đề tài tập trung nghiên cứu, thực nghiệm và so sánh hiệu năng của ba nhóm kiến trúc mạng nơ-ron tích chập (CNN) nhằm tự động hóa quy trình kiểm soát chất lượng lon rỗng trong dây chuyền sản xuất công nghiệp. Nghiên cứu được triển khai trên một bộ dữ liệu cân bằng, với bốn mô hình đại diện cho ba hướng tiếp cận khác nhau:

- **Autoencoder (AE)** – Phát hiện bất thường (Anomaly Detection) bằng học không giám sát.  
- **EfficientNetB0** – Phân loại nhị phân (Binary Classification) bằng học chuyển giao.  
- **YOLOv8-seg & YOLOv11-seg** – Phát hiện và phân đoạn đối tượng (Instance Segmentation).

## 📊 Tóm tắt kết quả

- **Autoencoder** sử dụng chỉ số Youden’s J để thiết lập ngưỡng phát hiện lỗi, nhưng hiệu suất còn hạn chế do không huấn luyện trên dữ liệu lỗi.
- **EfficientNetB0** đạt độ nhạy cao với lớp OK, nhưng gặp vấn đề nghiêm trọng với dương tính giả (False Positive).
- **YOLOv8-seg** cho kết quả vượt trội nhất, đạt độ chính xác 99.8% (OK) và 79.0% (NG).
- **YOLOv11-seg** tích hợp cơ chế chú ý không gian nâng cao (Spatial Attention Mechanisms) nhưng chưa đạt kỳ vọng.

Khóa luận kết luận rằng **YOLOv8-seg** là giải pháp tiềm năng cho việc định vị lỗi, tuy nhiên cần tối ưu thêm để cân bằng giữa Precision và Recall, hoặc kết hợp đa mô hình để xây dựng hệ thống kiểm tra đa tầng.

## 📁 Cấu trúc thư mục

- `CanDetect_Autoencoder.ipynb` – Mô hình phát hiện bất thường bằng Autoencoder.
- `CanDetect_EfficientNet.ipynb` – Mô hình phân loại nhị phân bằng EfficientNetB0.
- `CanDetect_YOLOv8seg.ipynb` – Mô hình phân đoạn đối tượng bằng YOLOv8-seg.
- `CanDetect_YOLOv11seg.ipynb` – Mô hình phân đoạn đối tượng bằng YOLOv11-seg.
- `HoangNuThuPhuong_21E1010003_DATN.pdf` – Báo cáo đồ án chính thức.
- `README.md` – Tài liệu giới thiệu tổng quan dự án.

## 📂 Tài liệu và dữ liệu bổ sung

Toàn bộ dữ liệu, báo cáo, hình ảnh minh họa và tài liệu liên quan có thể được truy cập tại:  
🔗 [Google Drive – Tài liệu đồ án](https://drive.google.com/drive/folders/1FXucC5tWVD3q2fWsqD-H8lGPZJW2VJbF?usp=sharing)

## 👩‍💻 Tác giả

**Hoàng Nữ Thu Phương**  
Mã số sinh viên: 21E1010003  
Ngành: Khoa học dữ liệu và trí tuệ nhân tạo 
Khoa Kỹ thuật và công nghệ - Dại học Huế

---
