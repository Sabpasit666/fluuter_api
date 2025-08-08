# Flutter API Recipe App 🍳

> **ใบงานที่ 8**: แอปพลิเคชัน Flutter สำหรับดึงตำรับอาหารจาก API

## 📖 คำอธิบายโปรเจกต์

แอปพลิเคชันนี้เป็น Flutter app ที่ออกแบบมาเพื่อดึงข้อมูลตำรับอาหารจาก API และแสดงผลในรูปแบบที่สวยงามและใช้งานง่าย ผู้ใช้สามารถเรียกดูสูตรอาหารต่างๆ พร้อมด้วยรายละเอียดและคำแนะนำในการทำอาหาร

## ✨ คุณสมบัติหลัก

- 🔍 ดึงข้อมูลตำรับอาหารจาก API
- 📱 UI ที่ตอบสนองและใช้งานง่าย
- 🍽️ แสดงรายการตำรับอาหารพร้อมรูปภาพ
- 📝 รายละเอียดสูตรอาหารและวิธีทำ
- ⚡ การโหลดข้อมูลแบบ asynchronous

## 🛠️ เทคโนโลยีที่ใช้

- **Flutter** - Framework สำหรับพัฒนาแอป mobile
- **Dart** - ภาษาโปรแกรมมิ่ง
- **HTTP Package** - สำหรับเรียก API
- **JSON Parsing** - สำหรับจัดการข้อมูล

## 📋 ความต้องการของระบบ

- Flutter SDK (เวอร์ชัน 3.0 หรือใหม่กว่า)
- Dart SDK (เวอร์ชัน 2.17 หรือใหม่กว่า)
- Android Studio หรือ VS Code
- Android SDK หรือ iOS SDK

## 🚀 การติดตั้งและรัน

### 1. Clone โปรเจกต์
```bash
git clone https://github.com/Sabpasit666/fluuter_api.git
cd fluuter_api
```

### 2. ติดตั้ง dependencies
```bash
flutter pub get
```

### 3. รันแอปพลิเคชัน
```bash
flutter run
```

### 4. สร้างไฟล์ APK (สำหรับ Android)
```bash
flutter build apk
```

## 📁 โครงสร้างโปรเจกต์

```
fluuter_api/
├── lib/
│   ├── main.dart              # ไฟล์หลักของแอป
│   ├── models/                # โมเดลสำหรับข้อมูล
│   ├── screens/               # หน้าจอต่างๆ
│   ├── services/              # บริการสำหรับเรียก API
│   └── widgets/               # Component ที่ใช้ซ้ำ
├── assets/                    # รูปภาพและไฟล์ทรัพยากร
├── test/                      # ไฟล์ทดสอบ
├── pubspec.yaml              # การตั้งค่า dependencies
└── README.md                 # ไฟล์คำอธิบายนี้
```

## 🔧 Dependencies ที่สำคัญ

```yaml
dependencies:
  flutter:
    sdk: flutter
  http: ^0.13.0
  cupertino_icons: ^1.0.2
  
dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^2.0.0
```

## 📱 ภาพหน้าจอ

*รูปภาพหน้าจอของแอปจะแสดงที่นี่*

## 🎯 การใช้งาน

1. **เปิดแอป**: เมื่อเปิดแอปจะแสดงหน้าหลักพร้อมรายการตำรับอาหาร
2. **เลือกตำรับ**: แตะที่ตำรับอาหารที่สนใจเพื่อดูรายละเอียด
3. **อ่านสูตร**: ดูส่วนผสมและวิธีทำอาหารแบบละเอียด

## 🔗 API ที่ใช้

โปรเจกต์นี้ใช้ Recipe API สำหรับดึงข้อมูลตำรับอาหาร:
- **Endpoint**: [ระบุ URL ของ API ที่ใช้]
- **Method**: GET
- **Response Format**: JSON

## ⚠️ ปัญหาที่พบบ่อย

### ปัญหา Network Permission
หากพบปัญหาการเชื่อมต่อ internet ใน Android ให้เพิ่มใน `android/app/src/main/AndroidManifest.xml`:
```xml
<uses-permission android:name="android.permission.INTERNET" />
```

### ปัญหา HTTPS Certificate
หากใช้ API ที่เป็น HTTP แทน HTTPS ให้ตั้งค่า network security config

## 🤝 การมีส่วนร่วม

1. Fork โปรเจกต์
2. สร้าง feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit การเปลี่ยนแปลง (`git commit -m 'Add some AmazingFeature'`)
4. Push ไปยัง branch (`git push origin feature/AmazingFeature`)
5. เปิด Pull Request

## 📞 ติดต่อ

- **ผู้พัฒนา**: Sabpasit666
- **GitHub**: [https://github.com/Sabpasit666](https://github.com/Sabpasit666)
- **โปรเจกต์**: [https://github.com/Sabpasit666/fluuter_api](https://github.com/Sabpasit666/fluuter_api)

## 📄 License

โปรเจกต์นี้อยู่ภายใต้ MIT License - ดูรายละเอียดใน [LICENSE](LICENSE) file

## 🙏 ขอบคุณ

- Flutter Team สำหรับ framework ที่ยอดเยี่ยม
- Recipe API provider สำหรับข้อมูลตำรับอาหาร
- ชุมชน Flutter Thailand สำหรับการสนับสนุน

---
⭐ หากโปรเจกต์นี้มีประโยชน์ อย่าลืมกด Star ให้ด้วยนะครับ!
