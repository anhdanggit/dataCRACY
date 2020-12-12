# Thống kê = "Đếm"

## Phân phối: Distribution

{% tabs %}
{% tab title="Data Yourself" %}
Truy cập: [https://databasic.io/en/wtfcsv](https://databasic.io/en/wtfcsv)

* [ ] Nhấn phân tích "Analyze"
* [ ] Bạn thấy gì từ kết quả?
{% endtab %}
{% endtabs %}

* Biến Categorical, biến Continuous
* Biến Categorical và % - Pivot 
* Đồ thị phân phối \(Cụ thể hơn trong phần: [Science of Counting](../../data-inspires/science-of-counting.md)\)
* Đồ thị phân phối cộng dồn: Biểu diễn rõ ràng hơn concept "Taste nghe nhạc của bạn kỳ lạ hơn 80% người Việt Nam\)

## Phân phối cho ta những thông tin gì?

* Bạn đứng đâu trong đám đông? Tương t: S[potify Music ](../1-what-data-can-do/d-aty-your-spotify-data.md#gout-nhac-cua-ban-di-den-dau)
* Dot-diagram, histogram, box-and-whisker
* Tìm giá  "đại diện": Trung Bình \(Average\), Trung Vị \(Median\), Mode 
* Đo độ trải của data: Standard 

## Data Fall

### Cẩn thận với %

{% tabs %}
{% tab title="Hỏi" %}
**Nghịch lý % - Data Tuyển Sinh ĐH Cambridge 1996**

Tại sao tổng tỷ lệ % được nhận của Nam lại cao hơn Nữ \(24% &gt; 23%\), trong khi từng ngành riêng lẻ, Nữ có tỷ lệ % được nhận cao hơn Nam?
{% endtab %}

{% tab title="Hint" %}
* Vì Tỷ lệ Nữ đăng ký vào các ngành "khó" - Y và Thú `(338 + 416) / 1,184 = 63%` cao hơn hẳn Nam `(140 + 22) / 584 = 27%`
* Cả 2 ngành này có tỷ lệ đậu thấp ở cả Nam lẫn 
{% endtab %}
{% endtabs %}

|  |  |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|  |  | Accept | % |  |  | % |
| Computer  | 26 | 7 | 27% | 228 | 58 | 25% |
| Kinh  | 240 | 63 | 26% | 512 | 112 | 22% |
| Kỹ  | 164 | 52 | 32% | 972 | 252 | 26% |
|  | 416 | 99 | 24% | 578 | 140 | 24% |
| Thú  | 338 | 53 | 16% | 180 | 22 | 12% |
| \*\*\*\* | **1,184** | **274** | **23%** | **2,470** | **584** | **24%** |

### Giá rị trung bình?

{% tabs %}
{% tab title="Hỏi" %}
**Thu nhập cũng trung bình thôi...**

Khi một người nói: "Thu nhập tôi cũng chỉ trung bình thôi"  
Anh ta có khấm khá hơn đa số đám đông? \(Giả sử ước lượng thu nhập của anh ta bằng giá trị trung bình là đúng sự thật\)
{% endtab %}

{% tab title="Hint" %}
* Đa số các yếu tố tự nhiên \(có tính ngẫu nhiên\) sẽ có dạng phân phối tự nhiên \(hình chuông\)
* Thu nhập là dạng data không đi theo phân phối tự nhiên
{% endtab %}
{% endtabs %}



