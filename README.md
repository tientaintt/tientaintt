# CloudComputing

## Đề tài: Tìm hiểu Amazon Translate và viết ứng dụng minh họa

        Nguyễn Tiến Tài - 20110563
        Võ Hoàn Hảo - 20110472
        Nguyễn Sỹ Hoàng Lâm - 20110514

## Các dịch vụ sử dụng

- AWS Translate
- AWS Polly
- AWS Textract
- AWS EC2

## Cài đặt và deloy lên AWS với docker-compose

### Chuẩn bị

- Tài khoản AWS có đăng ký dịch vụ IAM User
- Tạo user mới bằng IAM và ghi nhớ aws_access_key_id, aws_secret_access_key để cấu hình cho website

### Cài đặt

- Bước 1: Tạo máy ảo Ubuntu với EC2.

- Bước 2: Kết nối tới máy ảo EC2, cài đặt docker và docker-compose.

- Bước 3: Clone dự án về máy ảo EC2: https://github.com/BaoNguyen1001/aws-translate-app.git

- Bước 4: Cấu hình aws_access_key_id và aws_secret_access_key

  - Configuration index.html

    cd aws-translate-app/translate-app/templates/index.html

    ![](aws-translate-app/translate-app/assets/config_index.png)

  - Configuration app.py

    cd aws-translate-app/translate-app/app.py

    ![](aws-translate-app/translate-app/assets/config_app.png)

- Bước 5: Build và run file docker-compose

  - cd aws-translate-app
  - docker-compose build
  - docker-compose up

- Bước 6: Test web bằng địa chỉ máy ảo EC2 port 8000

#
#   T r a n s l a t e W e b  
 #   t i e n t a i n t t  
 #   t r a n s l a t e  
 