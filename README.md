# DetectingInappropriateVideosTargetingYoungChildren

## Hướng dẫn cài đặt và sử dụng

### Hướng dẫn cài đặt

Các gói cần cài đặt trước khi chạy:

Node.js và npm: Sử dụng lệnh sau để kiểm tra version đã cài đặt:

```bash
node -v
npm -v
```

Nếu kết quả trả về version của Node.js và npm, có nghĩa là bạn đã cài đặt thành công. Nếu không, vui lòng tiến hành cài đặt lại.

**Bước 1:** Clone Repository

```bash
git clone https://github.com/emilynh/DetectingInappropriateVideoTargetingYoungChildren.git
```

**Bước 2:** Cài đặt requirements cho mô hình:

```bash
pip install tensorflow
pip install google-api-python-client
pip install scikit-learn
pip install isodate
pip install emoji
```

**Bước 3:** Cài Đặt Dependencies:

- Mở folder vừa clone về trong VSCode.
- Mở terminal trong VSCode, di chuyển tới thư mục backend:

```bash
cd backend
pip install flask
python3 app.py  # hoặc python app.py
```

Sau khi chạy thành công lệnh `python3 app.py` hoặc `python app.py`, terminal sẽ hiển thị:

```vbnet
 * Serving Flask app 'app'
 * Debug mode: on
INFO:werkzeug:WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:5000
INFO:werkzeug:Press CTRL+C to quit
INFO:werkzeug: * Restarting with stat
```

Tiếp theo, mở một terminal mới và di chuyển vào lại thư mục react_app:

```bash
cd react_app
npm install react-scripts --save
npm install react-router-dom
npm start
```

Sau khi chạy thành công câu lệnh `npm start`, màn hình giao diện sẽ được hiển thị tại: [http://localhost:3000/](http://localhost:3000/)

### Hướng dẫn sử dụng

#### Giao diện phần Ứng dụng (APPLICATION):

1. Truy cập vào Home page của dự án.
2. Trên Nav bar, bạn có thể click vào "APPLICATION" hoặc trên hero page click vào nút "Get Started" để di chuyển tới phần ứng dụng.

**Bước 1:** Copy URL của một video Youtube bất kỳ và dán vào ô textfield trên giao diện.

**Bước 2:** Sau khi hoàn tất bước 1, click vào nút "Check" ngay bên cạnh để chạy mô hình. Đợi khoảng 4-5 giây để màn hình hiển thị kết quả.

**Bước 3:** Kết quả trả về là nhãn dự đoán của video.
