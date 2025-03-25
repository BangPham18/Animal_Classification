# Animal Classification Project

## Giới thiệu
Đây là dự án phân loại động vật sử dụng mô hình học sâu. Dự án bao gồm các bước tiền xử lý dữ liệu, huấn luyện mô hình và triển khai giao diện trực quan để dự đoán hình ảnh động vật.

## Cấu trúc thư mục
- `bien_URL.ipynb`: Chứa danh sách URL hình ảnh và cách tải về dữ liệu.
- `function_And_Class.ipynb`: Chứa các hàm xử lý dữ liệu, mô hình và các lớp hỗ trợ.
- `giao_Dien_Animal.ipynb`: Giao diện kéo thả ảnh để dự đoán nhãn bằng mô hình đã huấn luyện.
- `library.ipynb`: Chứa các thư viện cần thiết cho dự án.
- `model_LSTM_Animal.ipynb`: Huấn luyện mô hình LSTM để hỗ trợ phân loại hình ảnh động vật.
- `model_resnet.pth`: Trọng số mô hình ResNet đã huấn luyện.
- `model_vgg.pth`: Trọng số mô hình VGG đã huấn luyện.

## Xử lý dữ liệu
- Chạy `bien_URL.ipynb` để tải dữ liệu từ URL.
- Sử dụng `function_And_Class.ipynb` để tiền xử lý dữ liệu và tạo tập huấn luyện.

## Huấn luyện mô hình
- Chạy `model_LSTM_Animal.ipynb` để huấn luyện mô hình LSTM.
- Huấn luyện mô hình CNN (ResNet, VGG) trong `function_And_Class.ipynb` và lưu trọng số.
## So sánh hai mô hình
![image](https://github.com/user-attachments/assets/21c88c6a-730c-4285-b163-eacf466212ff)
- Mô hình ResNet50 có thời gian đào tạo thấp hơn nhiều và độ chính xác nhỉnh hơn một chút so với mô hình VGG16

## Giao diện dự đoán
- Mở `giao_Dien_Animal.ipynb` để khởi chạy giao diện.
- Kéo thả ảnh vào để nhận diện loại động vật.
  ![Ảnh chụp màn hình 2025-03-25 175034](https://github.com/user-attachments/assets/1e9668c1-3ac6-4e4c-9ad9-d458eb6fcbb8)
- Sau khi đưa ảnh vào sẽ xuất hiện dự đoán của mô hình
  ![Ảnh chụp màn hình 2025-03-25 175055](https://github.com/user-attachments/assets/93676bc2-2734-44c2-9810-95760bd66044)
  

  


