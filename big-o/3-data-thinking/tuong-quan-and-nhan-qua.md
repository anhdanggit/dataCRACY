# Tương quan & Nhân-Quả

Như đã bàn ở các phần trước, tư duy của dữ liệu và thống kê là tư duy **Ngoại Suy Quy Nạp**, từ những gì quan sát được rút ra kết luận trên những gì không quan sát được:

Ở [phần trước](xac-suat-and-gia-thuyet-khong.md), ta nói nhiều về chọn mẫu, và làm sao để ngoại suy quan sát trên mẫu cho một tổng thể lớn hơn

Ở phần này, ta sẽ nói về hai dạng Ngoại Suy được "thèm khát" hơn: **Ngoại suy tiên đoán, và ngoại suy nhân quả**. Nó không chỉ mô tả quá khứ, mà còn cho phép ta biết điều gì sẽ xảy ra trong tương lai, và phải làm gì để thay đổi tương lai.

Cả ngoại suy dự đoán và ngoại suy nhân quả đều dựa trên một ý tưởng quan trọng về Hệ số tương quan. Dù vậy đây cũng chính là ý tưởng gây nhầm nhọt nhiều nhất.

> Tương quan không hẳn là nhân quả.

Đó là câu thần chú nằm lòng của những ai học Thống Kê, và cũng là câu được lặp đi lặp lại trong suốt các kỳ của DATAcracy đến giờ.

## Tương Quan & Nhân Quả

### Hệ số tương quan

{% hint style="info" %}
**Hệ số tương quan \(correlation coefficients\)** của Pearson giúp "đo" mức độ các điểm trên biểu đồ điểm thể hiện mối quan hệ giữa hai đại lượng \(coi lại [**Datatalk\#2**](../2-everyone-can-read-data/)\) nằm trên một đường thẳng.
{% endhint %}

Ta có một ví dụ về tương quan kích thước đài hoa và cánh hoa trong các loài hoa diễn vĩ \(Iris\)

{% hint style="success" %}
**Hoạt Động \#1 - Tương quan Kích thước Đài Hoa và Cánh hoa**

1. Truy cập: [https://seeing-theory.brown.edu/regression-analysis/index.html\#section1](https://seeing-theory.brown.edu/regression-analysis/index.html#section1)
2. Chọn một loài hoa: Nhìn vào bảng hệ số tương quan \(correlation matrix\)
3. Bấm vào từng giá trị tương quan và quan sát sự thay đổi của biểu đồ
4. Chọn nhiều loài hoa và quan sát
{% endhint %}

![https://seeing-theory.brown.edu/regression-analysis/index.html\#section1](../../.gitbook/assets/image%20%2874%29.png)

![https://seeing-theory.brown.edu/regression-analysis/index.html\#section1](../../.gitbook/assets/image%20%2877%29.png)

* Hệ số tương quan có thể nhận giá trị từ -1 đến 1 \(tương quan âm đến tương quan dương\). Hệ số càng gần 0 \(giá trị tuyệt đối càng nhỏ\) thì tương quan càng yếu ớt.
* Câu chuyện Tương Quan trong bộ dữ liệu hoa Iris:
  * Trong cùng một chủng loại hoa, ta thấy tương quan dương đồng đều hơn, khi đài lá lớn thì cánh hoa lớn. Chiều dài và rộng của đài lá sẽ tương quan mạnh hơn \(do cùng là một bộ phần\) so với tương quan giữa chiều dài của đài lá và chiều rộng của cánh hoa
  * Khi thêm nhiều chủng loại hoa, ta thấy bắt đầu có tương quan âm. Ví dụ: Đài lá càng rộng thì cánh hoa càng ngắn.

Ở đây có một số định nghĩa \(không nhất thiết là chặc chẽ\) xung quanh hệ số tương quan:

Tương quan nghĩa là hai đại lượng có mối quan hệ tuyến tính \(nếu vẽ ra trên biểu đồ chấm thì các chấm nằm trên một đường thẳng\). Điều này không nhất thiết đúng vì có mối tương quan không tuyến tính. Ví dụ, có rất nhiều mối quan hệ trong tự nhiên đi theo U-curve \(như hình bên dưới\)

![](../../.gitbook/assets/image%20%2870%29.png)

### Tương quan không hẳn là nhân quả

Ví dụ bên trên có lẽ là một dẫn nhập tốt để bàn về việc: Tương quan không có nghĩa là nhân quả. Như mối tương quan giữa chiều rộng và chiều dài của lá, chúng xảy ra đồng thời và không hề có mối quan hệ nhân-quả.

Nhân quả, dẫu có thể thể hiện ra những quan sát dưới dạng tương quan, nhưng tương quan chỉ là bề mặt. Nhân quả là cốt lõi - cơ chế vận hành bên trong.

{% hint style="info" %}
**Nhân quả**, đơn giản mà nói, là việc ta làm điều này \(nhân\) và nó dẫn đến/gây ra điều khác \(quả\)
{% endhint %}

Định nghĩa này có vẻ đơn giản và thể hiện được một mục đích lớn \(có phần thực dụng\) trong Ngoại suy nhân quả, nhằm tác động thay đổi "nhân" để có được "quả" mình muốn, từ đó thay đổi được tương lai.

Chính bởi sự khác nhau giữa bản chất và cơ chế như vậy, mà hệ số tương quan chưa đủ độ "sâu" để diễn dịch được mối quan hệ nhân quả. Thực tế, để kết luận về nhân quả là một câu chuyện không đơn giản khác. Vì cuộc sống có quá nhiều tác nhân xuất hiện, diễn ra, tồn tại đồng thời.

## Nhân Quả & Phản Thực

> Cách duy nhất để trả lời một cách chắc chắn về Nhân Quả, là nhìn vào kết quả của những quyết định khác nhau trong nhiều thế giới song song giống hệt.

Hiện thực, ta đã chọn A, và quan sát được kết quả của A. Nhưng để trả lời câu hỏi, mọi thứ khác thế nào nếu ta chọn B, ta vốn không quan sát được. Đó gọi là **Phản Thực \(counter-factual\).**

Vấn đề phức tạp tiếp theo khiến Ngoại Suy Nhân Quả gần như bất khả thi là luôn có rất nhiều yếu tố "nhiễu" \(**Confounder**, nghĩa gốc trong tiếng Anh là yếu tố gây bối rối, sửng sốt, không thể giải thích\) diễn ra đồng thời, cùng có tác động lên kết quả.

Nhiều năm về trước, có một cuộc tranh luận trên mạng xã hội rằng: Học trường thực nghiệm có tốt hay không? Một cách rất data-driven, có người chứng minh bằng cách: Đem số điểm cuối năm của lớp thực nghiệp và lớp không-thực-nghiệm so với nhau. Kết quả rõ ràng điểm của lớp thực nghiệm cao hơn \(có ý nghĩa thống kê\) nhưng chúng không thể chứng minh mối quan hệ nhân quả, rằng tham gia lớp thực nghiệm giúp tăng năng lực của học sinh, vì các **confounders** sau:

1. Vì là lớp thực nghiệm, cách chấm điểm và cho đề có thể khác. Nên nếu so sánh điểm số, thì cần so trên một kỳ thi chuẩn hoá như nhau cho cả hai chương trình \(thực nghiệm và không thực nghiệm\). Ví dụ, kỳ thi chuẩn hoá đầu vào cấp 2.
2. Kể cả khi đó là kết quả của cùng một kỳ thi, cùng cách chấm \(như đã nói ở điểm 1\), ta vẫn lại có 1 confounder khác là: Các bậc cha mẹ biết về chương trình thực nghiệm thường là nhóm quan tâm đến có em, có thể thuộc lớp tri thức hơn, có điều kiện xã hội hơn. Bối cảnh gia đình và cha mẹ cũng ảnh hưởng nhiều đến kết quả học tập của con em.

Danh sách các yếu tố confounders còn có thể kéo dài. Tuy vậy, chúng ta vẫn có những phương pháp để ngoại suy về nhân quả. Trong đó phổ biến nhất là **Thử nghiệm đối chứng ngẫu nhiên - Randomized Controlled Trial** \(RCT\)

### RCT \(Randomized Controlled Trial\)

{% hint style="info" %}
**Hoạt Động \#2 - Sự khác biệt có ý nghĩa**

1. Truy cập: [https://seeing-theory.brown.edu/regression-analysis/index.html\#section1](https://seeing-theory.brown.edu/regression-analysis/index.html#section1)
2. Thí nghiệm chế độ ăn: Rat Feed Experiment. Các nhóm chọn ngẫu nhiên với chế độ ăn khác nhau. So sánh gí trị trung bình để xem các nhóm theo chế độ khác nhau có kết quả cân nặng khác nhau
3. Thử `Amount, Weight` \(lượng thức ăn và cân nặng\)
4. Thử `Diet, Weight` \(chế độ ăn và cân nặng\) **Optional**
5. Click vào từng parameter trên bảng kết quả để đọc thêm thông tin
6. Kéo/Dịch các data points để xem thông số thay đổi không
{% endhint %}

Đây là phương pháp cực kỳ phổ biến trong Y học thực chứng, và đánh giá hiệu quả chính sách:

* Viên thuốc X giúp giảm nguy cơ Y không?
* Chính sách khuyến học giúp cải thiện mức thu nhập không?

Ta lấy ví dụ **Rat Feed Experiment** để minh hoạ cho RCT đại khái được set-up như sau:

1. Chia ngẫu nhiên số lượng chuột thành các nhóm đối chứng
2. Mỗi nhóm nhận một "treatment" khác nhau \(cụ thể ở đây là chế độ ăn\)
3. Sau một thời gian cân chuột trên các nhóm đối chứng, từ đó vẽ được phân phối điểm như đồ thị, bằng việc so sánh giá trị trung tâm và độ dàn trải ta có thể kết luận cân nặng của các nhóm đối chứng có khác nhau "đáng kể" không

Như ở đây, khi so sánh 03 nhóm đối chứng ăn thịt bò, thịt heo, và ngũ cốc, ta thấy chuột nhóm ăn ngũ cốc có cân nặng trung bình nhẹ hơn, nhưng cân nhắc cả độ "dàn trải", theo thống kê, ta kết luận 3 nhóm không có nhiều khác biệt \(giả-thuyết-không rằng không có sự khác biệt không bị bác bỏ\).

![https://seeing-theory.brown.edu/regression-analysis/index.html\#section1](../../.gitbook/assets/image%20%2875%29.png)

Khi nhìn vào một thực nghiệm khác, so sánh giữa nhóm được cho lượng thức ăn nhiều và nhóm được cho ăn ít. Ta thấy sự khác biệt rõ nét hơn, ta có cơ sở để kết luận về nhân-quả: Chuột ăn ít thì sẽ nhẹ cân.

![](../../.gitbook/assets/image%20%2864%29.png)

## Hồi Quy Tuyến Tính

{% hint style="info" %}
**Hồi quy tuyến tính** là một mô hình thống kê. Mô hình, được định nghĩa, là một phiên bản đại diện và đơn giản hoá của thế giới, dưới một vài giả định \(nhằm cho phép sự đơn giản hoá đó\)
{% endhint %}

Lúc trước, khi còn đi học, tôi thường than vãn nhiều về sự phức tạp của các mô hình, với một lố giả định phức tạp đi kèm. Để rồi khi hiểu hơn một chút về bản chất, tôi nhận ra rằng bao cái phức tạp trong hệ thống gia đỉnh, và thiết lập mô hình chỉ để đạt được mục đích là đơn giản hoá cuộc sống. Vì nếu không thì, cuộc sống sẽ quá phức tạp để có thể thuyết minh được bằng một phương trình. Rồi, ta sẽ vờ tin rằng "phiên bản đơn giản" đó có thể cho ta hay về thực tại ở một chừng mực tốt vừa đủ, ta chấp nhận sai số cho phép.

Như vậy thì, một mô hình có thể diễn đạt như sau:

> Giá trị quan sát = Mô hình thuyết minh + sai số

Ta tách những gì quan sát được thành: Phần giải thích được \(mô hình determistics\) và sai số \(residual errors\).

Các nhà thống kê học, khoa học xã hội và kinh tế lượng qua nhiều đời, nỗ lực không ngừng để giải thích được nhiều nhất bằng mô hình, và sau từng công bố mới lại giảm thiểu bớt phần sai số. Mỗi cống hiến là một phát kiến mới để chẻ nhỏ thêm nữa phần sai số kia.

Ta có thể dùng mô hình đó phục vụ nhiều mục đích: **Giải thích, Mô phỏng, hay tiên đoán.**

{% hint style="success" %}
**Hoạt Động \#3 - Vẽ đường thẳng tốt nhất để mô tả "trend"**

1. Theo bạn, thế nào là tốt nhất?
2. Bạn sẽ vẽ như thế nào?
{% endhint %}

![](../../.gitbook/assets/image%20%2866%29.png)

Một trong những phương pháp hồi quy tuyến tính đơn giản là được sử dụng rộng rãi nhất là: **Hồi quy bình phương nhỏ nhất \(Ordinary Least Square - OLS\).**

Như trong minh hoạ của Seeting Theory: [HERE](https://seeing-theory.brown.edu/regression-analysis/index.html#section1)

{% hint style="info" %}
Mô hình hồi quy: `Y_predict = f(X) = a + bX`
{% endhint %}

1. Giá trị tiên đoán \(trên trục Y\) `Y_predict` là điểm trên đường thẳng hồi quy, ứng với giá trị X quan sát được
2. Định nghĩa đường thẳng tiên đoán tốt nhất là giảm thiểu sai số, có khoản cách giữa `Y_predict` và `Y` \(thực tế\) là nhỏ nhất: `Y_predict - Y` = `sai số`
3. Chú ý là có những sai số âm \(Y\_predict &lt; Y\) và sai số dương \(Y\_predict &gt; Y\). Ta cần biến đổi để triệt tiêu âm/dương của chiều sai số, nếu không khi gộp sai số của các quan sát lại, sai số âm và sai số dương sẽ tự triệt tiêu nhau.
4. Ta bình phương sai số: `(Y_predict - Y)^2` = `sai số bình phương`
5. Như tên gọi, phương pháp hồi quy bình phương nhỏ nhất, đơn giản là kẻ đường thẳng sao cho sai số bình phương là nhỏ nhất, hay bình phương khoản cách giữa các điểm quan sát đến đường thẳng là nhỏ nhất.

![](../../.gitbook/assets/image%20%2872%29.png)

## Recap

* Ngoại suy tiên đoán, và ngoại suy nhân quả. Nó không chỉ mô tả quá khứ, mà còn cho phép ta biết điều gì sẽ xảy ra trong tương lai, và phải làm gì để thay đổi tương lai.
* **Hệ số tương quan \(correlation coefficients\)** của Pearson giúp "đo" mức độ các điểm trên biểu đồ điểm thể hiện mối quan hệ giữa hai đại lượng nằm trên một đường thẳng.
* Nhân quả, dẫu có thể thể hiện ra những quan sát dưới dạng tương quan, nhưng tương quan chỉ là bề mặt. Nhân quả là cốt lõi - cơ chế vận hành bên trong.
* Cách duy nhất để trả lời một cách chắc chắn về Nhân Quả, là nhìn vào kết quả của những quyết định khác nhau trong nhiều thế giới song song giống hệt.
* Tuy vậy, chúng ta vẫn có những phương pháp để ngoại suy về nhân quả. Trong đó phổ biến nhất là **Thử nghiệm đối chứng ngẫu nhiên - Randomized Controlled Trial** \(RCT\)
* Hồi quy tuyến tính là một mô hình thống kê. Mô hình, được định nghĩa, là một phiên bản đại diện và đơn giản hoá của thế giới, dưới một vài giả định \(nhằm cho phép sự đơn giản hoá đó\)
* Giá trị quan sát = Mô hình thuyết minh + sai số
* Phương pháp hồi quy bình phương nhỏ nhất \(OLS\), đơn giản là kẻ đường thẳng sao cho sai số bình phương là nhỏ nhất, hay bình phương khoản cách giữa các điểm quan sát đến đường thẳng là nhỏ nhất.

