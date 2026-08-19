# 🎓 HCMUT Report Template

Template LaTeX chuẩn dành cho viết báo cáo Bài tập lớn, Đồ án môn học, Thực tập ngoài trường và Đồ án Tốt nghiệp tại Trường Đại học Bách khoa - ĐHQG TP.HCM (HCMUT). Template này được tinh chỉnh đặc biệt phù hợp với các bạn sinh viên nhóm ngành Kỹ thuật.

## ✨ Tính năng nổi bật

*   **Chuẩn quy định Đồ án Bách Khoa:** Căn lề chuẩn (Trái 40mm, Phải 25mm, Trên 40mm, Dưới 25mm), dùng font Times New Roman 13pt, giãn dòng 1.3.
*   **Cấu trúc tự động:** Tự động tạo và liên kết (hyperlink) Mục lục, Danh sách hình minh họa, Danh sách bảng số liệu.
*   **Highlight Code chuẩn IDE:** Tích hợp sẵn bộ style màu chuẩn của VSCode và MATLAB IDE cho các ngôn ngữ thường dùng: `C/C++`, `Python`, `MATLAB`, `Verilog`.
*   **Trích dẫn IEEE:** Tự động hóa quản lý tài liệu tham khảo theo chuẩn IEEE bằng `biblatex` và Biber.
*   **Mạch điện:** Tích hợp sẵn `circuitikz` để vẽ sơ đồ mạch nguyên lý trực tiếp, và `siunitx` để gõ chuẩn đơn vị vật lý.

## 📂 Cấu trúc thư mục

*   `main.tex`: File báo cáo chính (chứa toàn bộ nội dung, các chương, phụ lục).
*   `styles.tex`: File cấu hình màu sắc và style cho code C++, Python, MATLAB.
*   `verilogstyle.tex`: File cấu hình chuyên biệt cho code Verilog/VHDL.
*   `references.bib`: File chứa data tài liệu tham khảo (sách, báo, link web).
*   `figures/`: Thư mục chứa hình ảnh (ảnh bìa, logo HCMUT, đồ thị, sơ đồ khối).

---

## 🚀 Hướng dẫn sử dụng

Tại giao diện GitHub, bấm *Code > Download ZIP* để tải toàn bộ source code về máy. Bạn có thể compile template này bằng 3 cách:

### Cách 1: Sử dụng Overleaf (Khuyên dùng cho làm việc nhóm)
Overleaf là trình soạn thảo LaTeX trực tuyến tiện lợi nhất, không cần cài đặt phần mềm nặng máy.
1. Truy cập [Overleaf](https://www.overleaf.com/) và đăng nhập.
2. Chọn **New Project** -> **Upload Project**.
3. Nén toàn bộ các file trong template này thành một file `.zip` và tải lên.
4. Mở file `main.tex`. Ở Menu bên trái, đảm bảo **Compiler** được thiết lập là `pdfLaTeX`.
5. Bấm **Recompile** (hoặc `Ctrl + S`) để xem kết quả PDF ở khung bên phải.

### Cách 2: Sử dụng Prism AI Workspace
Prism là không gian soạn thảo tích hợp AI, hỗ trợ đắc lực trong việc debug lỗi cú pháp LaTeX hoặc nhờ AI viết công thức toán học nhanh.
1. Tạo một workspace mới trên Prism AI.
2. Tải toàn bộ các file `.tex`, `.bib` và thư mục `figures/` lên hệ thống file của Prism.
3. Mở file `main.tex`.
4. Bấm nút **Compile** trên giao diện để kết xuất ra PDF. Nếu trình biên dịch báo lỗi thiếu package, bạn có thể chat trực tiếp với AI để nhờ fix ngay tại chỗ.

### Cách 3: Biên dịch Local trên máy tính (VSCode + MiKTeX trên Windows)
Dành cho những bạn thích code offline, quản lý file trực tiếp trên máy cá nhân và tận dụng tốc độ của máy tính.

1. **Cài đặt trình biên dịch MiKTeX:**
   * Truy cập trang chủ [MiKTeX](https://miktex.org/download) và tải file cài đặt (Installer) dành cho Windows.
   * Chạy file `.exe` vừa tải, cứ nhấn *Next* để cài đặt theo các thông số mặc định (có thể chọn *Install MiKTeX only for me*).
2. **Cài đặt Visual Studio Code (VSCode):**
   * Tải và cài đặt [VSCode](https://code.visualstudio.com/) nếu máy bạn chưa có.
3. **Cài đặt Extension LaTeX Workshop:**
   * Mở VSCode, click vào biểu tượng **Extensions** ở thanh menu bên trái (hoặc nhấn `Ctrl + Shift + X`).
   * Gõ tìm kiếm `LaTeX Workshop` (của tác giả James Yu) và nhấn nút **Install**.
4. **Mở Project và Biên dịch (Compile):**
   * Kéo thả thư mục chứa template báo cáo của bạn vào VSCode (hoặc chọn *File > Open Folder*).
   * Click mở file `main.tex`.
   * Ở góc trên cùng bên phải màn hình, nhấn vào nút **Build LaTeX project** (biểu tượng hình nút Play ▷) hoặc dùng phím tắt `Ctrl + Alt + B`.
   * **Lưu ý quan trọng:** Trong lần Build đầu tiên, do template sử dụng nhiều thư viện (như `vietnam.sty`, `biblatex`...), trình biên dịch MiKTeX sẽ bật lên các hộp thoại yêu cầu tải package (Package Installation). Bạn chỉ cần bỏ dấu tick ở ô *"Always show this dialog"* và nhấn **Install** để nó tự động tải ngầm về máy.
5. **Xem file PDF trực tiếp trên VSCode:**
   * Sau khi thanh trạng thái báo Build thành công (*Recipe succeeded*), bạn nhấn vào biểu tượng **View LaTeX PDF** (hình tờ giấy có kính lúp) nằm ngay cạnh nút Build ở góc trên bên phải.
   * File PDF sẽ xuất hiện dưới dạng chia đôi màn hình (Split View). Từ bây giờ, mỗi khi bạn gõ text và lưu lại (`Ctrl + S`), file PDF bên cạnh sẽ tự động cập nhật ngay lập tức.

📺 **Tham khảo Video hướng dẫn chi tiết từng bước tại đây:** 
[Install LaTeX Workshop and compile PDF in VSCode LaTeX (Windows)](https://www.youtube.com/watch?v=4lyHIQl4VM8)

---

## 💡 Mẹo nhỏ khi viết báo cáo

*   **Chèn code:** Để chèn code, hãy dùng lệnh `\begin{lstlisting}[style=tên_style, caption={Tên đoạn code}]`. Các style hiện có hỗ trợ: `prettyc`, `prettypython`, `prettymatlab`, `prettyverilog`.
*   **Trích dẫn:** Chỉ cần thả link/thông tin sách vào file `references.bib`. Ở file `main.tex`, lệnh `\nocite{*}` sẽ tự động kéo tất cả ra trang Tài liệu tham khảo theo format IEEE.
*   **Thêm ảnh:** Hãy thả tất cả ảnh vào thư mục `figures/`. Trong code, chỉ cần gọi tên file ảnh (VD: `HCMUT.png`).

---

**Trường:** Đại học Bách Khoa - ĐHQG TP.HCM (HCMUT)

*Nếu thấy template này hữu ích, hãy tặng kho lưu trữ một ⭐ nhé! Chúc các bạn làm đồ án điểm cao!*
