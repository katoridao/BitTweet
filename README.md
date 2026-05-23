# BitTweet

![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Gradle](https://img.shields.io/badge/Gradle-02303A?logo=gradle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Mục lục

- [Mô tả](#-mô-tả)
- [Tech stack](#-tech-stack)
- [Tính năng](#-tính-năng)
- [Cài đặt](#-cài-đặt)
- [Sử dụng](#-sử-dụng)
- [Cấu trúc thư mục](#-cấu-trúc-thư-mục)
- [Nhóm phát triển](#-nhóm-phát-triển)

## Mô tả

**BitTweet** là ứng dụng Android đặt đồ uống được xây dựng bằng Java và Firebase, cung cấp trải nghiệm mua hàng hiện đại với giao diện trực quan, quản lý đơn hàng và hỗ trợ thanh toán linh hoạt.

Ứng dụng cho phép người dùng đăng ký tài khoản, duyệt sản phẩm, thêm vào giỏ hàng, thanh toán và theo dõi đơn hàng. Ngoài ra, hệ thống còn hỗ trợ nhân viên/quản trị viên quản lý sản phẩm, khách hàng và đơn hàng thông qua Firebase.

Đây là dự án nhóm được phát triển bởi 3 thành viên.

[![Live Demo](https://img.shields.io/badge/Live-Demo-2ea44f?style=for-the-badge)](https://appetize.io/app/b_pastiojddv2nxmfuob2rfjyfum)

## Tech stack

- Java
- Android SDK
- Material Design
- Firebase Authentication
- Firebase Firestore
- Firebase Storage
- Glide
- Picasso
- ZXing
- Gradle

## Tính năng

- Đăng nhập, đăng ký và khôi phục mật khẩu
- Hiển thị danh sách đồ uống và chi tiết sản phẩm
- Thêm sản phẩm vào giỏ hàng và quản lý số lượng
- Thanh toán bằng tiền mặt hoặc thẻ
- Tạo và lưu mã QR cho giao dịch
- Xem lịch sử đơn hàng
- Quản lý sản phẩm, khách hàng và đơn hàng cho nhân viên/quản trị viên
- Tải và hiển thị ảnh sản phẩm từ Firebase Storage
- Đồng bộ dữ liệu người dùng và đơn hàng bằng Firebase Firestore

## Cài đặt

### 1. Clone repository

```bash
git clone https://github.com/katoridao/BitTweet.git
cd BitTweet
```

### 2. Cấu hình Firebase

1. Tạo project mới trên Firebase Console
2. Bật:
   - Authentication
   - Firestore Database
   - Firebase Storage
3. Tải file `google-services.json`
4. Đặt file vào thư mục:

```text
app/google-services.json
```

### 3. Chạy project

1. Mở project bằng Android Studio
2. Sync Gradle
3. Chạy ứng dụng trên emulator hoặc thiết bị thật

### 4. Build APK

```bash
./gradlew assembleDebug
```

Trên Windows:

```bash
gradlew.bat assembleDebug
```

## Sử dụng

1. Mở ứng dụng và đăng nhập hoặc đăng ký tài khoản
2. Duyệt danh sách đồ uống và xem thông tin chi tiết
3. Thêm sản phẩm vào giỏ hàng
4. Chọn phương thức thanh toán phù hợp
5. Theo dõi lịch sử đơn hàng
6. Nhân viên/quản trị viên có thể quản lý sản phẩm và đơn hàng trong hệ thống

## Cấu trúc thư mục

```text
BitTweet/
├── app/
│   ├── build.gradle.kts
│   ├── google-services.json
│   ├── src/
│   │   ├── main/
│   │   │   ├── AndroidManifest.xml
│   │   │   ├── java/
│   │   │   │   └── fpt/anhdhph/bittweet/
│   │   │   │       ├── DAO/
│   │   │   │       ├── fragment/
│   │   │   │       ├── model/
│   │   │   │       ├── screen/
│   │   │   │       └── util/
│   │   │   └── res/
│   │   │       ├── layout/
│   │   │       ├── drawable/
│   │   │       ├── values/
│   │   │       └── mipmap/
│   └── proguard-rules.pro
├── build.gradle.kts
├── gradle.properties
├── gradlew
├── gradlew.bat
├── settings.gradle.kts
└── README.md
```

## Nhóm phát triển

### Đào Hoàng Anh

- Team Leader
- Backend Development
- Testing & Debugging

GitHub: @katoridao

### Kiều Khánh Duy

- Android Development
- Authentication Flow
- Firebase Integration

GitHub: @codertiger24

### Cao Minh Hiếu

- UI/UX Design
- User Experience
- Interface Implementation

GitHub: @hieuKao
