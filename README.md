# Bài tập lớn chủ đề 5: Ghép ảnh Panorama 

Dự án này là sản phẩm của nhóm 09 lớp 02 môn XLA - thầy Phạm Hoàng Việt 

---

## 👥 Thành viên 

| Họ và tên          | Mã sinh viên | 
|--------------------|--------------|
| Phạm Hải Dương       | B22DCCN169   | 
| Dương Văn Thuận         | B22DCCN841   | 


## 📝 Giới thiệu

`Best-version.ipynb` là file notebook chính, nơi chứa toàn bộ quy trình xử lý ảnh, phân tích và thực nghiệm. Dự án sử dụng ba thư viện chính:

* **OpenCV (cv2)**: đọc ảnh, xử lý đặc trưng, warp ảnh
* **NumPy**: xử lý ma trận, tính toán
* **Matplotlib**: hiển thị ảnh và đồ thị trong notebook

Thư mục `pictures/` lưu các hình ảnh đầu vào hoặc ảnh minh họa dùng trong notebook.
`slideNoiDung` là file chứa nội dung bài thuyết trình nhóm.
`requirements.txt` là file khai báo thư viện cần cài để chạy dự án.

---

## 📁 Cấu trúc thư mục

```
project/
│
├── Best-version.ipynb       # Notebook chính
├── pictures/                # Thư mục chứa ảnh của dự án
│     ├── img_left.jpg
│     ├── img_middle.png
│     └── ...
├── slideNoiDung             # File bài thuyết trình
├── requirements.txt         # Các thư viện cần thiết
└── README.md                # Tài liệu mô tả dự án
```

---

## 📦 Nội dung của `requirements.txt`

Dự án chỉ dùng ba thư viện sau, vì vậy file sẽ gồm:

```
opencv-python
numpy
matplotlib
```

---

## 🚀 Cách chạy dự án

1. Cài Python (khuyến nghị 3.9+).
2. Cài các thư viện bằng:

```
pip install -r requirements.txt
```

3. Mở notebook:

```
jupyter notebook
```

Sau đó mở `Best-version.ipynb` và chạy từng cell.

---

## 📸 Thư mục ảnh `pictures/`

Thư mục cung cấp ảnh cần dùng trong quá trình xử lý và để test ghép ảnh panorama.
Giữ nguyên cấu trúc thư mục để tránh lỗi đường dẫn trong notebook.

---

## 🎤 File `slideNoiDung`

Đây là tài liệu thuyết trình của nhóm, mô tả nội dung chính, lí thuyết liên quan đến dự án "Tạo ảnh Panorama bằng SIFT". 
File dùng để trình bày, không ảnh hưởng đến quá trình chạy mã nguồn. Ngoài ra còn trình bày các phương pháp sử dụng, giải thích code từng cell rất hữu dụng.

---

## 🧠 Mục tiêu của dự án

Mục tiêu chính của dự án là giúp sinh viên:

* Hiểu và ứng dụng **SIFT** để phát hiện và mô tả điểm đặc trưng.
* Sử dụng **BFMatcher + Lowe Ratio Test** để tìm các cặp điểm tương ứng giữa hai ảnh.
* Ước lượng **Homography** bằng thuật toán **RANSAC**.
* Thực hiện **warpPerspective** để đưa ảnh về cùng hệ tọa độ.
* Ghép ảnh bằng **feather blending** giúp giảm seam và làm ảnh mượt.
* **Tự động crop** để loại bỏ phần đen sau khi ghép.
* Xây dựng pipeline panorama tương tự các hệ thống thực tế như Google Photos, Street View hoặc xử lý ảnh 360°.

Dự án là sự kết hợp giữa lý thuyết và thực hành trong môn **Xử lý ảnh số**, giúp sinh viên hiểu bản chất đồng thời có khả năng tự triển khai một hệ thống ghép ảnh hoàn chỉnh.

