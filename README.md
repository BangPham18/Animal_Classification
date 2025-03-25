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
- Dữ liệu có tổng cộng 120 lớp bao gồm các nhóm động vật trên cạn, trên trời, dưới nước. Một số hình ảnh tiêu biểu như:
![7ae826e4ac](https://github.com/user-attachments/assets/94d515c1-eb07-4a2b-ad69-0c5f340cb536)
![4f11bf2ff1](https://github.com/user-attachments/assets/f394b41f-53aa-46a7-94ff-310a0095411d)
- Phải đưa ảnh về dạng mà mô hình nhận vào được (size: 224x224, channel: RGB)
  
## Huấn luyện mô hình
- Chạy `model_LSTM_Animal.ipynb` để huấn luyện mô hình LSTM.
- Sử dụng phương pháp transfer learning để đào tạo lớp cuối cùng của mô hình ResNet50 và VGG16
  ![image](https://github.com/user-attachments/assets/15970fe8-034c-4b2c-b5d8-3a6c75720c0c)
  ![image](https://github.com/user-attachments/assets/1656c82f-1c7d-4cce-93bf-3c02707dde73)

- Huấn luyện mô hình CNN (ResNet, VGG) trong `function_And_Class.ipynb` và lưu trọng số.

## So sánh hai mô hình
![image](https://github.com/user-attachments/assets/a66ea0b1-3dfc-4042-a81b-b901eb5411cb)
- Mô hình ResNet50 có thời gian đào tạo thấp hơn nhiều và độ chính xác nhỉnh hơn một chút so với mô hình VGG16
-> Sử dụng mô hình ResNet50 để đưa ra dự đoán

## Giao diện dự đoán
- Mở `giao_Dien_Animal.ipynb` để khởi chạy giao diện.
- Kéo thả ảnh vào để nhận diện loại động vật.
  ![Ảnh chụp màn hình 2025-03-25 175034](https://github.com/user-attachments/assets/1e9668c1-3ac6-4e4c-9ad9-d458eb6fcbb8)
- Sau khi đưa ảnh vào sẽ xuất hiện dự đoán của mô hình
  ![Ảnh chụp màn hình 2025-03-25 175055](https://github.com/user-attachments/assets/93676bc2-2734-44c2-9810-95760bd66044)
  

  


