# Exci
Exci là viết tắt của Excellent với mong muốn là một ứng dụng học tập tuyệt vời. Trong phiên bản đầu tiên này là một nguyên bản đầu tiên phục vụ cho việc học từ vựng tiếng anh là chủ yếu. Sử dụng Llama3.2 để làm công cụ đắc lực trong việc trao đổi học tiếng anh.
# Key Features
- Admin
    - Vocabulary/ Collection management
    - Users management
    - AI assistance
    - analyzing User/ Vocabulary/ Collection.
- Search/ Save vocabulary from dictionary api (https://dictionaryapi.dev/).
- Spaced repetition
- AI assistance by Ollama 3.2

# Structure
- exci-fe-flutter: User interface
- WinForm_Exci
    - APIForClient: chương trình chạy API dựng bằng ASP .NET
    - data:
        - EXCI_DEV.bacpac: các mẫu dữ liệu đơn giản
    - Exci: chương trình quản lý dựng bằng WinForm .NET

# Platforms
- [x] Web
- [ ] Android (Waiting)

# Requirement
- Flutter
- SQL Server
- ASP .NET
- Ollama

# Installing
```
git clone https://github.com/Khoa15/exci.git
cd exci
```
Tạo model trong ollama. Trong tệp đã có sẵn mẫu các prompt đơn giản để tạo model phục vụ cho người dùng và người quản lý.
```
cd ollama
python main.py
```
Cài đặt dữ liệu mẫu "EXCI_DEV.bacpac" vào SQL Server với tên database là "EXCI_DEV". Sau đó chạy chương trình trong thư mục APIForClient.
<br>
Chạy câu lệnh sau để cài đặt các gói cần thiết sau đó chạy trên nền tảng web. Hiện chỉ hỗ trợ web.
```
cd exci-fe-flutter
flutter pub get
flutter run
```
Trong trường hợp sử dụng Ollama, hãy bảo đảm ollama đã được bật và kiểm tra lại port.

# Architecture
Updating later...

# Contributors
- Thank Thao for admin management.
- Thank dictionaryapi.dev for open api dictionary.

# Contact
If there have any problems. Please contact me: nguyentrongdangkhoa15@gmail.com or khoa15503.work@gmail.com