# Xác suất & Giả-thuyết-không

> Đời là một giảng đường của xác suất. — Walter Bagehot.

## Chọn Mẫu và Xác Suất

{% hint style="success" %}
**Hoạt Động\#1 — Seeing Theory**

1. Truy cập: [Seeing Theory - Probability Distribution](https://seeing-theory.brown.edu/probability-distributions/index.html#section1)
2. Giả sử vùng các ô lục giác bên màn hình tay phải tượng trưng cho phần **Dân Số ta quan tâm** \(Người Việt Nam &gt;18 tuổi\)
3. Bạn có thể bôi màu cho các ô lục giác để quy định tỷ lệ của các câu trả lời khác nhau trên dân số
4. Bấm nút **"Sample Distribution"** bên dưỡi
{% endhint %}

![](../../.gitbook/assets/image%20%2867%29.png)

Ta đang mô phỏng lại quá trình chọn mẫu, để minh hoạ cho việc vì sao kết quả trên một mẫu \(sample\) được chọn ngẫu nhiên lại có ý nghĩa phóng chiếu cho một quần thể \(population\).

Bản chất của mô phỏng \(simulation\) ở đây là: Ta giả bộ ta biết phân phối giá trị trong quần thể thật:

* 1/7 \(14%\) dân số có 0 có mối tình nào \(tô trắng\)
* 1/7 \(14%\) dân số có 1 mối tình \(tô đỏ\)
* 1/7 \(14%\) dân số có 2 mối tình \(tô xanh\)
* 1/7 \(14%\) dân số có 3 mối tình \(tô cam\)
* 3/7 \(44%\) dân số có 4+ mối tình \(tô vàng\)

{% hint style="warning" %}
**Lưu ý:** Tổng xác suất của các trường hợp = 1/7 + 1/7 + 1/7 + 1/7 + 3/7 = 1 = 100%
{% endhint %}

### Ngẫu nhiên + Số lượng = Tính Đại Diện

Nhưng lại vờ như không biết, ta bắt đầu lấy mẫu ngẫu nhiên. Quá trình đó được minh hoạ bằng những điểm đen được "chấm" bất kỳ trên "không gian" quần thể. Bên dưới, ta có một biểu đồ cột phân phối.

{% hint style="info" %}
**Phân phối tần suất:** Thể hiện tần suất xuất hiện của các giá trị khác nhau.
{% endhint %}

Ta thấy trong mẫu ngẫu nhiên, tỷ lệ phân phối \(số lượng người của từng giá trị \(mối tình vắt vai\) trên tổng số người trong mẫu\) gần giống với toàn quần thể thực mà ta biết. Tính ngẫu nhiên đảm bảo việc ta có thể "tái tạo" lại phân phối tần suất gốc trên phân phối của một mẫu nhỏ, và vì phân phối tần suất gần giống nhau nên các giá trị thống kê \(trung bình, giá trị kỳ vọng, độ dàn trải của dữ liệu\) sẽ giống với quần thể gốc.

Ta cũng để ý là: Ở một số ít các các quan sát đầu tiên "bốc" ngẫu nhiên được, ta chưa thể tạo ra phân phối tần suất với quần thể gốc. Nhưng khi số quan sát trong mẫu càng tăng lên, tỷ lệ phân phối dần trở nên càng giống hơn với phân phối gốc.

{% hint style="info" %}
Như vậy, **số lượng của mẫu** cũng ảnh hưởng đến tính "đại diện" của mẫu \(so với quần thể gốc\).
{% endhint %}

![](../../.gitbook/assets/image%20%2869%29.png)

### Phân phối của Data

{% hint style="success" %}
**Hoạt Động\#2** - Vị trí của bạn trên Phân Phối về Gout Âm nhạc Hãy trở lại DataYourself của [**Datatalk\#1**](../1-hello-world/d-aty-spotify-data.md) [www.obscurifymusic.com](http://www.obscurifymusic.com). Bạn hiểu biểu đồ này như thế nào?

1. Biểu đồ này nói gì? Tiêu đề, trục ngang, trục dọc?
2. Mỗi cột trên biểu đồ này có độ cao tượng trưng cho điều gì?
3. Biểu dồ được tạo ra từ data gì? Các bước tính toán?
4. Con số 80% có ý nghĩa gì?
{% endhint %}

Nếu được phép nói về Thống Kê - một cách cho "dẫn dã", thì đó chỉ là liệt kê và đếm. Như trong ví dụ bên trên:

* Liệt kê giá trị một cá thể trong mẫu có thể nhận được \(Điểm Obscure trên trục ngang\). Giá trị có thể rời rạc \(như trong ví dụ về số mối tình\) hay liên tục \(như bên dưới\). Về mặt bản chất, giá trị liên tục có thể chuyển về rời rạc, bằng cách chia thành các đoạn \(bin\) ⇒ mỗi đoạn giá trị ứng với chiều ngang của 1 cột trên biểu đồ
* Đếm số người tham gia \(Use Count\) có giá trị ứng với mỗi "bin" ⇒ Ứng với chiều cao của mỗi cột
* Ta cũng có một biểu đồ thể hiện **Phân Phối Tần Suất** của các giá trị khác nhau
* Giá trị có cột cao là giá trị có tần suất cao, thường xuyên xảy ra
* Giá trị có cột thấp là giá trị có tần suất thấp, hiếm khi xảy ra

{% hint style="info" %}
**Phân phối tần suất** cho ta biết mức độ thường xuyên hay hiếm xảy ra của một giá trị bất kỳ.
{% endhint %}

![](../../.gitbook/assets/image%20%2873%29.png)

Phân phối tần suất đó, có một số điểm tương đồng với Lý Thuyết Xác Suất:

* Tổng chiều cao các cột cộng lại = tổng số lượng mẫu \(Tổng tần suất của mọi giá trị = 100%\)
* Ở biểu đồ trên, đường màu xanh chỉ một giá trị X \(điểm số\) và để biết những ai có điểm &lt; X, ta cộng số người ở tất cả các cột nằm bên tay trái của X.

{% hint style="info" %}
Tổng User Count ở các cột &lt; X / Tổng số người tham gia = 80%
{% endhint %}

* Ta đọc rằng: 80% mẫu có giá trị nhỏ hơn X. Hay, 80% mẫu có điểm "Dị" thấp hơn tôi. Hay, tôi có gout nghe nhạc lạ hơn 80% người tham gia khảo sát.
* Nếu mẫu có tính ngẫu nhiên \(và đủ lớn\), ta có thể kết luận: Tôi có gout nghe nhạc lạ hơn 80% người Việt Nam.

{% hint style="warning" %}
Theo bạn, có những yếu tố gì khiến mẫu như trên không đảm bảo tính Ngẫu Nhiên?
{% endhint %}

## Phân phối hình chuông

> Một người bạn ở Mỹ vừa sinh một đứa bé \(đủ 9 tháng 10 ngày\), cân nặng 2.91 kg. Mọi người đều bảo em bé nhẹ hơn mất trung bình, có đáng lo? Mức cân nặng này có bình thường không?

Thống kê và Xác suất có thể giúp bạn trả lời câu hỏi trên. Đi theo các bước tương tự như phân phối về Gout nhạc, ta có:

\(a\) Dựa vào thống kê trên mẫu hơn 1,096,277 trẻ, ta có thể vẻ được biểu đồ cột thể hiện **phân phối tần suất**

\(b\) Phân phối này đi theo dạng hình chuông \(**Phân phối chuẩn**\), ta sẽ vẽ được đường màu xanh đi qua các cột. Phân phối chuẩn được mô tả bằng hai chỉ số thống kê: _Trung Bình_ \(giá trị trung tâm/giá trị đại diện/giá trị kỳ vọng\) và _Độ Lệch Chuẩn_ \(đo độ "dàn trải" của phân phối xung quanh quá trị đại diện\). Đường màu đỏ là giá trị cân nặng của đứa trẻ - con người bạn, 2910 grams.

\(c\) Trên phân phối, ta có các đường chấm-gạch \(**Phân vị - Percentiles**\). Ý nghĩa tương tự như con số 80% bên trên, phân vị 90% nghĩa là có 90% mẫu có giá trị thấp hơn giá trị tại điểm đó \(cắt trục ngang\). _Phân vị 50%_, chính là _giá trị trung bình_, 50% mẫu có giá trị thấp hơn giá trị trung bình \(trong phân phối chuẩn\)

\(d\) Tỷ lệ trẻ em có cân nặng thấp hơn 2910 grams, phần tô đỏ, tương ứng 11%. Hay nếu nói theo ngôn ngữ xác suất, nếu "bốc" một đứa trẻ mới sinh bất kỳ, thì có đến 89% có cân nặng cao hơn đứa trẻ con người bạn.

![Source: David Spielgelharter. The Art of Statistics: Learning from Data.](../../.gitbook/assets/image%20%2865%29.png)

## Trở lại: Giá trị Kỳ Vọng

Trở lại với giá trị Kỳ Vọng mà ta từng đề cập trong [**Datatalk\#2**](../2-everyone-can-read-data/)\*\*\*\*

> Như chính tên gọi, **Giá trị kỳ vọng** là giá trị "best guess" cho một cá thể bất kỳ bốc ra từ một tập thể.

Như vậy, giá trị Kỳ vọng là giá trị \(cố gắng\) diễn tả giá trị trung tâm của một phân phối. Nếu thử ngẫu nghiên bốc các mẫu từ quần thể, thì khi số lần bốc tăng lên ta sẽ "tiến gần" về giá trị kỳ vọng.

{% tabs %}
{% tab title="Hoạt Động \#3" %}
**Hoạt Động \#3**

1. Theo bạn tung đồng xu \(công bằng\) 10 lần ta được bao nhiêu % mặt Sấp?
2. Tung 100 lần, bao nhiêu % mặt Sấp?
3. Tung 200 lần, bao nhiêu % mặt Sấp?
4. Tung 1000 lần, bao nhiêu % mặt Sấp?
{% endtab %}

{% tab title="Hints" %}
\*\*\*\*

* Khi số lần tung xu càng tăng lên, ta càng có tỷ lệ "tiến gần" về 0.5.
* 0.5 là giá trị kỳ vọng khi tung một đồng xu ra mặt sấp
* Dù rằng nó không nhất thiết có ý nghĩa thực tế. Trong thực tế, đồng xu chỉ nhận hoặc sấp hoặc ngửa, không có giá trị 0.5 sấp. Tương tự, mỗi người chỉ có 1, 2, 3 mối tình. Nhưng giá trị kỳ vọng có thể là 2.5 người bộ.
{% endtab %}
{% endtabs %}

Tương tự với bài toán trung xí ngầu, ta biết các giá trị có thể nhận được: 1, 2, 3, 4, 5, 6. Và xác suất ta các mặt là đều nhau: 1/6 + 1/6 + 1/6 + 1/6 + 1/6 + 1/6 = 1 = 100%.

{% hint style="info" %}
Ta có giá trị Kỳ vọng là: 1/6 x 1 + 1/6 x 2 + 1/6 x 3 + 1/6 x 4 + 1/6 x 5 + 1/6 x 6 = 3.5
{% endhint %}

Ta thử tung [xí ngầu 200 lần](https://seeing-theory.brown.edu/basic-probability/index.html)\*\*\*\*[:](https://seeing-theory.brown.edu/basic-probability/index.html)

![https://seeing-theory.brown.edu/basic-probability/index.html](../../.gitbook/assets/image%20%2871%29.png)

* Trục ngang: Số lần tung xí ngầu từ 0 đến 200
* Trục dọc: Giá trị trung bình của kết quả của X lần tung. Ví dụ, khi ở lần tung đầu tiên ta dc 6 nút, nhận giá trị 6 nút trục dọc 1 lần tung trục ngang. Ở lần tung thừ 75, ta lấy trung bình 75 lần trước đó được 3.69
* Ta thấy khi số lần tung tăng lên, ta tiệm cận về giá trị kỳ vọng 3.5

![https://seeing-theory.brown.edu/basic-probability/index.html](../../.gitbook/assets/image%20%2876%29.png)

{% hint style="info" %}
Quay trở lại **Phân phối chuẩn**, nếu ta cũng làm tương tự, nhân giá trị cho tần suất, ta sẽ được _giá trị Kỳ Vọng_ đúng bằng _giá trị Trung bình_ \(đồng thời là _Phân vị 50%_\) điểm chính giữa của phân phối
{% endhint %}

## Giả-thuyết-không

Vậy ta dùng **Thống kê và Xác suất** để trả lời các câu hỏi như thế nào, khi nào thì ta biết một quan sát là có ý nghĩa \(về mặt thống kê\).

### Thế nào là Giả thuyết?

Giả thuyết là một cách giải thích được đặt ra cho một hiện thượng. Không hoàn toàn là sự thật, mà là một phiên bản luỹ tiến, được phép chỉnh sửa và củng cổ theo thời gian, có tính tương đối dựa trên một số mặc định \(assumptions\).

Ta cần một quy trình chứng minh giả thuyết bằng thực nghiệm, hay nói cách khác là dùng Data và Thống kê để chứng mình một quan sát là có cơ sở. Cần chứng minh thực nghiệp để đảm bảo tính khách quan, bởi con người cũng thường có trí tưởng tượng ảo diệu, hay nhìn thấy những quy luật vốn thuần tuý là ngẫu nhiên.

{% hint style="info" %}
Ý niệm về \(tiệm cận\) chân lý trong thực nghiệm Thống kê rất đơn giản, **điều gì liên tục lặp đi lặp lại đủ nhiều** thì nó là một quy luật có ý nghĩa, thì nó tiệm cận sự thật \(tương tự như câu chuyện tung đầu xu 1,000 lần hay liên tục lấy mẫu quan sát từ quần thể gốc trong phần trên\). Còn những sự ngẫu nhiên sẽ chỉ có tần suất thấp, và dường như tự triệt tiêu khi ta tăng số lần quan sát lên.
{% endhint %}

### Giả-thuyết-không

Các ta chứng minh một giả thuyết ít khi nào là chứng minh giả thuyết đó đúng, mà chỉ là giả thuyết đó không thể chối bỏ \(ví dụ, ở mức ý nghĩa 5%\).

Giả-thuyết-không \(Null hypothesis\) là khái niệm trung tâm của quy trình chứng minh đó.

Giả thuyết không được cho là sự thật cho đến khi, ta có thể bác bỏ nó bằng dữ liệu. Ví dụ:

* Không có sự chênh lệch nào về lương ở Nam và Nữ
* Không có sự chênh lệch nào về điểm số giữa học sinh ở thành phố và nông thôn

> **Giả-thuyết-không**, tự bản thân nó, là một câu chuyện buồn. Vì đó là giả thuyết được đặt ra mà người đặt không hề mang theo nổ lực hay ý định gì để chứng minh nó. Giả-thuyết-không được đặt ra để được/bị bác bỏ, nhằm tìm ra một phát hiện mới \(ở giả thuyết đối lập\). Khi một phát hiện đã được công nhận, bấy giờ nó lại trở thành giả-thuyết-không trong các nghiên cứu về sau để "bị" bác bỏ. Đó là quá trình diễn tiến của khoa học, phủ định của phủ định.

Nếu có thể bác bỏ các giả-thuyết-không:

* Không có sự chênh lệch nào về lương ở Nam và Nữ
* Không có sự chênh lệch nào về điểm số giữa học sinh ở thành phố và nông thôn

Thì có nghĩa là điều ngược lại có cơ sở đúng:

* Có sự chênh lệch về lương ở Nam và Nữ
* Không có sự chênh lệch nào về điểm số giữa học sinh ở thành phố và nông thôn

Phát hiện của khoa học ở đâu không phải là kết luận điều gì đúng, mà là điều gì có cơ sở đúng dựa vào số liệu. Trên nền tảng không phải chứng minh, mà là bác bỏ.

### Khoản Tin Cậy, Mức Ý Nghĩa, Kích thước mẫu

{% hint style="info" %}
**Hoạt Động \#4**

1. Truy cập: [https://seeing-theory.brown.edu/frequentist-inference/index.html\#section2](https://seeing-theory.brown.edu/frequentist-inference/index.html#section2)
2. Chọn phân phối chuẩn: `Normal`
3. Chọn mức sample size \(n\) và Mức Ý Nghĩa \(alpha\) - Mức Tin Cậy \(1-alpha\)
4. Nhấn `Start Sampling`
5. Thử nhiều giá trị n và alpha khác nhau
{% endhint %}

![https://seeing-theory.brown.edu/frequentist-inference/index.html\#section3](../../.gitbook/assets/image%20%2868%29.png)

Trong minh hoạ này, ta thấy:

* Ta có phần phối gốc tô màu cam, nhận giá trị trung bình \(giá trị kỳ vọng\) là mu
* Dựa nào số lượng mẫu n ta chọn, mỗi lần sẽ thả xuống n quan sát lấy ngẫu nhiên từ mẫu gốc
* Ta lấy trung bình lại giá trị của n quan sát, sẽ được điểm tròn ở giữa \(tiếp tục rơi xuống\), đường ngang vẽ ra hai bên từ chấm tròn thể hiện độ "dàn trải" của data xung quanh giá trị trung bình \(Xem lại [**Datatalk\#2**](../2-everyone-can-read-data/du-lieu-ky-vong-and-tin-cay.md)\)
* Tuỳ theo mức ý nghĩa \(alpha\), ta có khoản tin cậy tương ứng. Mức ý nghĩa = 10%, thì khoản tin cậy = 90%
* Chấm màu xanh để chỉ, giá trị trung bình thực \(mu\) có nằm trong khoản tin cậy của mẫu n \(khoản tin cậy giao với đường chấm gạch dóng từ giá trị mu\). Ngược lại màu đỏ nghĩa là không nằm trong khoản tin cậy. Ta cũng có biểu đồ thể hiện tỷ lệ bao gồm và không bao gồm
* Khi **thay đổi giá trị alpha**, ta thấy độ dài trải ra hai bên thu hẹp/dãn rộng. Khi mức ý nghĩa alpha càng bé, khoản tin cậy càng rộng, tỷ lệ bao gồm giá trị mu càng lớn. Và, ngược lại.
* Giữ nguyên một mức giá trị alpha 0.90, ta thay đổi n, ta thấy khi n càng nhỏ thì khoản tin cậy càng rộng, và ngược lại n càng lớn thì khoản tin cậy càng hẹp lại.

Vì sao quan sát này lại thú vị? Nó đang xâu chuỗi lại nhiều ý tưởng quan trọng trong Thống kê và kiểm chứng thực nghiệm.

* **Problem:** Có sự chênh lệch về lương giữa Nam và Nữ?
* **Giả-thuyết-không:** Không có sự chênh lệch về lương giữa Nam và Nữ. Thể hiện bằng phương trình: Chênh lệch lương của Nam và Nữ = 0 \(mu\)
* Giả sử: Chênh lệch lương đó cũng phân phối theo một phân phối như phần màu cam bên trên. Có giá trị kỳ vọng là mu, nghĩa là trong trường hợp này giả-thuyết-không không nên bị bác bỏ
* Bằng việc quan sát giá trị trên các mẫu rút ra từ phân phối gốc, ta biết được xác suất quan sát mu không nằm trong khoản tin cậy của mẫu. Hiện tại, mu là giá trị thật, nên dù lấy mẫu ngẫu nhiên nhiều lần, giá trị mu vẫn nằm trong đa số các khoản tin cậy của mẫu bất kỳ. Với xác suất \(ví dụ &gt;90%\), ta không thể nói việc mu xuất hiện trong mẫu là sự ngẫu nhiên.
* Ngược lại, nếu số lần "reject" \(% mu không nằm trong khoản tin cậy\) lớn hơn \(ví dụ &gt; 90%\), ta cho rằng Giả-thuyết-không không phải là sự thật \(bác bỏ\)

> Ý niệm về \(tiệm cận\) chân lý trong thực nghiệm Thống kê rất đơn giản, **điều gì liên tục lặp đi lặp lại đủ nhiều** thì nó là một quy luật có ý nghĩa

* Bằng việc thay đổi mức ý nghĩa và khoản tin cậy, ta tăng/giảm số lần "reject" giả-thuyết-không và từ đó thay đổi kết luận
* Khi số lượng mẫu tăng lên, khoản tin cậy thu ngắn lại, ta bớt "mông lung" hơn.

## Recap

* **Phân phối tần suất:** Thể hiện tần suất xuất hiện của các giá trị khác nhau.
* Tính ngẫu nhiên đảm bảo việc ta có thể "tái tạo" lại phân phối tần suất gốc trên phân phối của một mẫu nhỏ
* Giá trị Kỳ vọng là giá trị \(cố gắng\) diễn tả giá trị trung tâm của một phân phối. Nếu thử ngẫu nghiên bốc các mẫu từ quần thể, thì khi số lần bốc tăng lên ta sẽ "tiến gần" về giá trị kỳ vọng
* Ý niệm về \(tiệm cận\) chân lý trong thực nghiệm Thống kê rất đơn giản, **điều gì liên tục lặp đi lặp lại đủ nhiều** thì nó là một quy luật "tiệm cận" sự thật
* Bằng việc thay đổi mức ý nghĩa và khoản tin cậy, ta tăng/giảm số lần "reject" giả-thuyết-không và từ đó thay đổi kết luận
* Khi số lượng mẫu tăng lên, khoản tin cậy thu ngắn lại, ta bớt "mông lung" hơn.

