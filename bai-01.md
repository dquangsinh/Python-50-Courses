### Bài 01: Làm quen với Python
## 1. Giới thiệu về Python
Python là một ngôn ngữ lập trình bậc cao (high-level), thông dịch (interpreted), hướng đối tượng (object-oriented) và đa范式 (multi-paradigm). Nó được tạo ra bởi Guido van Rossum (thường được gọi là "Bố của Python") và phát hành lần đầu tiên vào năm 1991. Tên của ngôn ngữ này không liên quan đến loài rắn trăn (Python), mà lấy từ tên của một nhóm hài kịch truyền hình Anh Quốc mang tên Monty Python's Flying Circus, mà Guido là một người hâm mộ.

Mục tiêu thiết kế của Python tập trung vào tính dễ đọc (readability) và sự ngắn gọn (conciseness). Cú pháp của Python cho phép lập trình viên biểu diễn các ý tưởng chỉ với vài dòng code, trong khi ở các ngôn ngữ khác có thể tốn nhiều dòng hơn.

Slogan của Python
"Simple is better than complex." (Đơn giản luôn tốt hơn phức tạp.)

Bạn có thể xem toàn bộ triết lý thiết kế của Python bằng cách gõ lệnh import this trong môi trường tương tác của Python.

>>> import thisThe Zen of Python, by Tim PetersBeautiful is better than ugly.Explicit is better than implicit.Simple is better than complex.Complex is better than complicated.Flat is better than nested.Sparse is better than dense.Readability counts.Special cases aren't special enough to break the rules.Although practicality beats purity.Errors should never pass silently.Unless explicitly silenced.In the face of ambiguity, refuse the temptation to guess.There should be one-- and preferably only one --obvious way to do it.Although that way may not be obvious at first unless you're Dutch.Now is better than never.Although never is often better than *right* now.If the implementation is hard to explain, it's a bad idea.If the implementation is easy to explain, it may be a good idea.Namespaces are one honking great idea -- let's do more of those!
## 2. Ưu điểm và Nhược điểm của Python
# Ưu điểm
Dễ học và dễ đọc: Cú pháp rõ ràng, trực quan, gần gũi với ngôn ngữ tự nhiên.
Mã nguồn mở: Python là phần mềm mã nguồn mở (FLOSS), bạn có thể tự do sử dụng, chỉnh sửa và phân phối.
Khả năng移植 (Cross-platform): Python có thể chạy trên nhiều nền tảng khác nhau (Windows, Linux/Unix, Mac OS X, v.v.).
Thư viện chuẩn phong phú: Python đi kèm với một kho thư viện khổng lồ, hỗ trợ sẵn cho nhiều tác vụ như xử lý chuỗi, regex, mạng, threading, GUI, v.v.
Cộng đồng lớn: Cộng đồng lập trình viên Python rất đông đảo, cung cấp vô số các thư viện bên thứ 3 (PyPI) và hỗ trợ giải đáp thắc mắc rất nhanh.
# Nhược điểm
Tốc độ thực thi chậm: Do là ngôn ngữ thông dịch và động, tốc độ thực thi của Python chậm hơn so với các ngôn ngữ biên dịch (compiled) như C/C++ hay Java. Tuy nhiên, đối với hầu hết các ứng dụng hiện đại, tốc độ này là chấp nhận được, và các phần quan trọng về hiệu năng có thể được viết bằng C/C++ và tích hợp vào Python.
## 3. Lĩnh vực ứng dụng của Python
Python là một ngôn ngữ "đa năng", được ứng dụng rộng rãi trong nhiều lĩnh vực:

Lập trình Web ở phía Server (Backend): Django, Flask, FastAPI.
Tự động hóa / Scripting: Viết các kịch bản tự động hóa công việc lặp đi lặp lại (DevOps, Mạng, Quản trị hệ thống).
Khoa học Dữ liệu & Phân tích Dữ liệu: NumPy, Pandas, Matplotlib.
Trí tuệ nhân tạo (AI) & Học máy (Machine Learning): TensorFlow, PyTorch, Scikit-learn.
Cào dữ liệu (Web Scraping/Crawling): Requests, BeautifulSoup, Scrapy.
Lập trình GUI: Tkinter, PyQt.
4. Cài đặt môi trường Python
Windows
Truy cập trang chủ: https://www.python.org/downloads/
Tải về phiên bản Python mới nhất cho Windows.
Chạy file cài đặt. LƯU Ý RẤT QUAN TRỌNG: Nhớ đánh dấu chọn vào ô "Add Python 3.x to PATH" trước khi nhấn Install Now. Điều này giúp bạn có thể gọi Python từ bất kỳ đâu trong Command Prompt.
macOS
macOS thường đã được cài sẵn Python 2.7. Tuy nhiên, bạn nên cài đặt Python 3.

Cách dễ nhất là sử dụng Homebrew:
bash

brew install python3
Linux
Hầu hết các bản phân phối Linux đều có sẵn Python. Nếu chưa có, bạn có thể cài qua trình quản lý gói:

Ubuntu/Debian:
bash

sudo apt update
sudo apt install python3
5. Chạy chương trình Python
Có hai cách cơ bản để chạy code Python:

Cách 1: Môi trường tương tác (Interactive Mode)
Mở Terminal (hoặc Command Prompt trên Windows), gõ python (hoặc python3 trên Mac/Linux) và nhấn Enter. Bạn sẽ thấy dấu nhắc >>>.

python

>>> print('hello, world!')
hello, world!
>>> 100 + 200
300
>>> exit()  # Thoát khỏi môi trường tương tác
(Mẹo: Bạn có thể cài đặt IPython bằng lệnh pip install ipython để có một môi trường tương tác mạnh mẽ và thân thiện hơn, hỗ trợ tô sáng cú pháp và tự động hoàn thành).

Cách 2: Chạy file tập lệnh (Script Mode)
Tạo một file có đuôi mở rộng là .py, ví dụ hello.py, và viết code vào đó:

python

# hello.py
print('hello, world!')
print('Chào mừng đến với thế giới Python!')
Mở terminal, di chuyển đến thư mục chứa file hello.py và chạy lệnh:

bash

python hello.py
6. Chương trình Python đầu tiên
Truyền thống của lập trình viên khi học một ngôn ngữ mới là viết một chương trình in ra dòng chữ "hello, world!". Trong Python, việc này chỉ tốn 1 dòng code:

python

print('hello, world!')
Khác với C, C++ hay Java phải có hàm main(), các lớp, và các dấu chấm phẩy ; phức tạp, Python mang lại cảm giác viết code như đang viết tiếng Anh.

7. Chú thích (Comments) trong Python
Chú thích (comment) là những dòng văn bản bị bỏ qua bởi trình thông dịch. Chú thích dùng để giải thích ý nghĩa của code cho người khác (hoặc cho chính mình trong tương lai) đọc.

Chú thích một dòng
Sử dụng dấu thăng #:

python

# Đây là một chú thích một dòng
print('hello, world!')  # Chú thích cũng có thể viết sau dòng code
Chú thích nhiều dòng
Sử dụng 3 dấu nháy kép """ hoặc 3 dấu nháy đơn ''':

python

"""
Đây là một chú thích
dài trên nhiều dòng.
Thường dùng để giải thích hàm hoặc lớp.
"""
print('hello, world!')
Tóm tắt bài học
Trong bài này, chúng ta đã tìm hiểu:

Python là gì, lịch sử ra đời và triết lý thiết kế của nó.
Những ưu/nhược điểm chính của Python.
Các lĩnh vực mà Python đang thống trị.
Cách cài đặt Python và thiết lập biến môi trường PATH.
Hai cách chạy code Python: Tương tác và Chạy file tập lệnh.
Cách viết chương trình đầu tiên9: hello, world!.
Cách sử dụng chú thích (comments) trong code.
Hẹn gặp lại các bạn ở Bài 02!
