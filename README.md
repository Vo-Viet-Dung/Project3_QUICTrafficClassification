# Đề tài: Phân biệt lưu lượng QUIC bằng mạng CNN

## Hướng dẫn cài đặt
1. Clone Repo:
* git clone: [QUIC Traffic Classification](https://github.com/Vo-Viet-Dung/Project3_QUICTrafficClassification)
* Tải và cài đặt Python: [Python](https://www.python.org/downloads/)
* Tải và cài đặt các thư viện liên quan bao gồm: scapy, pandas, numpy, sklearn, keras.
2. Tạo dataset:
* Dữ liệu lưu lượng mẫu mà bài toán sử dụng được cắt ra từ tập dữ liệu khá lớn nên đồ án này chỉ sử dụng lại một phần tại: [QUIC Traffic](https://drive.google.com/drive/folders/1V7rfXIu2tE3Dh8Dg15AMfN2ryW_mVhQX?usp=sharing)
* Chương trình tạo dữ liệu huấn luyện được để trong 2 file:
  * Tiền xử lý cho mô hình RandomForest tại file: project3PreprocessingRandomForest.ipynb
  * Tiền xử lý cho mô hình RandomForest tại file: project3PreprocessingCNN.ipynb
* Do project được chạy và thực thi trên Google Colab và dữ liệu được import từ Google Drive nên nếu dùng nguyên đoạn code hiện tại thì sẽ cần đưa các folder trong thư mục Netfow_QUIC1 lên thư mục có tên là "project3" trên Google Drive.
* Hoặc có thể chạy đoạn code ở jupyternotebook phía local tuy nhiên cần sửa lại đường dẫn của cấu trúc thư mục (Nên sử dụng Colab do file dữ liệu có rất nhiều gói tin nên việc đọc ở máy tính cá nhân sẽ rất lâu so với sử dụng Colab được tích hợp cơ chế phân tán).
3. Sử dụng dataset đã được tạo sẵn:
* Ngoài ra thì trong repo đã được tạo sẵn 2 file dữ liệu huấn luyện cho 2 mô hình thuật toán RandomForest và CNN
* File dataset.csv chứa dữ liệu huấn luyện cho mô hình thuật toán Randomforest.
* File datasetCNN.csv chưa dữ liệu huấn luyện cho mô hình mạng CNN.
4. Chạy mô hình RandomForest:
* Chương trình thuật toán RandomForest được chứa trong file "project3RandomForest.ipynb"
* Do các đoạn mã chương trình được xây dựng và thực thi trên Colab cho nên nếu muốn sử dụng nguyên lại đoạn chương trình hiện tại thì các file .csv chứa dataset cần phải được đẩy lên Google Drive với cấu trúc thư mục tương ứng.
* Nếu muốn chạy chương trình ở phía máy tính cá nhân thì cần thay đổi đường dẫn tới các file .csv ở trong code.
5. Chạy mô hình mạng CNN:
* Chương trình thuật toán RandomForest được chứa trong file "project3RandomForest.ipynb"
* Cách chạy chương trình cũng tương tự như với mô hình RandomForest tuy nhiên với mạng CNN thì nên ưu tiên sử dụng Google Colab để sử dụng GPU tối ưu hóa thời gian chạy mô hình.
