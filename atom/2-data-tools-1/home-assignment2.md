# 2.5 - Home Assignment\#2

{% hint style="info" %}
## Weekend, 08-09/05/2021

* Hoàn thành Week 2 [Lab\#2  Set-up Working Environment](2.4-lab-2-set-up-working-environment.md)
* Chỉnh sửa [Assignment\#1](../1-data-strategy-and-metrics/1.4-home-assignment.md) sau buổi học Week 2
* Mỗi learner reviews &gt;= 2 Assigments trên channel `#atom-assignment1`
{% endhint %}

## Home Assignment\#2 \(Flipped Learning Week 3\)

### Step 1: Github

* Fork: [https://github.com/anhdanggit/atom-assignments](https://github.com/anhdanggit/atom-assignments)
* Dùng Github Desktop, clone repo atom-assignments trên profile của bạn \(sau khi fork\)
* Mở repo trên máy, bằng VS Code \(hoặc cái IDE khác\)
* Repo gồm:
  * `ATOM_Home_Assignment_2.ipynb`: Là file chưa các câu hỏi bài tập \(bạn có thể dùng trên Google Colab hoặc Jupyter Notebook trên local machine\)
  * `env_variable_test.json`: File sẽ sử dụng trong Assignment

### Step 2: Gmail App Password

* Gmail App Password là dạng password để các application \(bot, python program\) có thể thao tác trên gmail. Nhằm automate một số process, ví dụ như gửi mail.
* Copy từ `env_variable_test.json` thành `env_variable.json`

  , update các thông tin

  1. Chọn một địa chỉ email để test cho exercise này =&gt; `SENDER_EMAIL`
  2. Tạo App Passwords [HERE](https://support.google.com/accounts/answer/185833?p=InvalidSecondFactor&visit_id=637562139468610337-3856071038&rd=1) 
  3. Copy the App Password =&gt; `PWD_EMAIL`

     ![](../../.gitbook/assets/image%20%28123%29.png)

### Step 3: API\_KEY

API là một nguồn để lấy data \(giải thích cụ thể hơn trong `ATOM_Home_Assignment_2.ipynb`\). Mỗi API để access cần có quyền truy cập. Assignment 2 dùng API của OpenWeather, bạn tạo API Key như sau:

1. Create the api key: [Weather API - OpenWeatherMap](https://openweathermap.org/api) 
2. Check email =&gt; Verify account 
3. Nếu báo lỗi 401, đợi vài phút để API key được ativated 
4. Tham khảo API Docs: [Current weather data - OpenWeatherMap](https://openweathermap.org/current) 
5. Copy Key =&gt; Update `WEATHER_API_KEY` trong file `env_variable.py` 

![](../../.gitbook/assets/image%20%28120%29.png)

### Step 4: Notebook

* Colab Notebook of [Assignment\#2 ](https://colab.research.google.com/drive/1kH3eqQp9BAH4AL0j3QM90BrjX7uCcKws?usp=sharing)
* Ôn lại kiến thức Python Basics: **Functions, Flow Chart, List, Dictionaries**
* Bạn có thể làm bài tập trên Google Colab hoặc Jupyter Notebook đã cài đặt trên máy quá Lab\#2
  * Colab: Upload file `env_variable.py`  lên Files hoặc Google Drive \(Private\)
  * Local: Lưu ý khi push lên github không push file `env_variable.py` =&gt; Nguy hiểm. Để tên file này trong list `.gitignore` để git ignores file
* Assignment này sẽ hướng dẫn bạn tạo program gửi email theo nội dung, sử dụng các email bạn có để test

  ![](../../.gitbook/assets/image%20%28122%29.png)

![](../../.gitbook/assets/image%20%28127%29.png)

* Cũng trong bài này, sẽ học về HTML. Bạn có thể tìm hiểu cấu trúc của HTML của bất kỳ website bằng Developer Tools 

![](../../.gitbook/assets/image%20%28122%29.png)

![](../../.gitbook/assets/image%20%28125%29.png)

* Đọc thêm phần API, JSON, Email trong **Automate the Boring Stuff with Python**. Al Sweigart\)

{% hint style="success" %}
**Submission**

* Upload Notebook với code cho **TODO \#1 - TODO \#5** trên Github Repo của bạn
* Viết thêm các comments, text bất kỳ vào notebooks
* Copy link vào \#atom-assignment2
{% endhint %}

{% hint style="warning" %}
* Học viên hoàn thành assignments nhiều nhất có thể và submit trên channel chung \(Slack\) trước **5h chiều, Thứ 5 hàng tuần.**
* “Last Chance”: Sau buổi học, học viên có thể hoàn chỉnh thêm assignment theo nội dung review trong lớp học, và submit lại trước **12h trưa Chủ nhật \(sau buổi học\).**
* Khuyến khích mọi người tích cực trao đổi và hỏi các thắc mắc trong quá trình làm bài.
{% endhint %}



