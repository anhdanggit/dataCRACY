---
description: 'Câu hỏi mở đầu: Thuật Toán là gì?'
---

# Thuật Toán

## Thuật Toán

### Thuật Toán là gì?

OK. Vậy **Thuật Toán** là gì? Định nghĩa gốc của Thuật Toán có thể đơn sơ hơn rất nhiều so với cách nó được "thần thánh" hoá.

> **Thuật toán** là tập hợp một chuỗi hướng dẫn/lệnh logic để \(Máy Tính\) giải quyết một vấn đề nào đó hay đưa ra một kết quả nào đó.

Theo một định nghĩa rộng hơn \(và dễ hiểu hơn\), Thuật toán là một chuỗi các bước - Có Mở Đầu, Có Kết Thúc. Để thực hiện một task \(tác vụ\) cụ thể. Nếu không giới hạn ở chỉ Máy Tính, thì:

* Công thức nấu ăn ⇒ Là một Thuật Toán
* Đi từ Văn Phòng về nhà, qua ngã tư ngã 5 ngã 7 ⇒ Là một Thuật Toán
* Tấm lựa đậu: Đậu Đỏ bỏ rổ bên phải, đậu xanh bỏ rổ bên trai ⇒ Rất đơn giản, nhưng cũng là một thuật toán

### Thử viết Thuật Toán: Robot giao hàng

![](../../.gitbook/assets/image%20%2819%29.png)

{% tabs %}
{% tab title="Hỏi" %}
Chuỗi lệnh bên: `Phải-Lên-Phải-Phải-Lên`. Sẽ đưa Robot giao hàng đến nhà màu hồng. Lưu ý: Robot chỉ bay được trên các ô trắng:

* Bạn thử viết chuỗi lệnh để Robot giao đến nhà màu Đỏ?
* Có nhà màu nào Robot không thể giao đến không?
{% endtab %}

{% tab title="Hints" %}
`Phải-Lên-Lên-Trái-Trái`
{% endtab %}
{% endtabs %}

### IF-ELSE-THEN: Ngôn Ngữ của Máy Tính

Bạn đã điền qua [Trắc Nghiệm Data Persona](https://www.notion.so/Big-O-d543563c16d14409bf9c204228bfec3f)? Đây chính là một Thuật Toán.

* Mỗi người tham gia trắc nghiệm sẽ đi theo một chuỗi câu hỏi khác nhau
* Câu trả lời trước sẽ ảnh hưởng đến câu tiếp theo mà bạn được hỏi
* Kết quả cuối cùng là:
  * Phân bạn vào một nhóm Persona \(Người Quan tâm, Người Đọc Hiểu, Người Suy Luận, hay Người Theo Đuổi\) ⇒ Đây là **Thuật Toán Phân Cụm** Đơn Giản \(`Clustering Algorithm`\)
  * Gợi ý các nội dung phù hợp với bạn ⇒ Đây là **Thuật Toán Gợi Ý** Đơn Giản \(`Recommendation Algorithms`\)

![Nh&#x1EEF;ng g&#xEC; x&#x1EA3;y ra Ph&#xED;a sau Tr&#x1EAF;c Nghi&#x1EC7;m Data Persona](../../.gitbook/assets/image%20%283%29.png)

Khi đi sau vào setting của Trắc Nghiệm này, bạn sẽ thấy Giao Diện như trên:

1. Phần bên phải màn hình: **Logic Map \(dạng cây\)** tuần tự theo các bước, trong mỗi bước sẽ có những điều kiện Logic cụ thế khiến người tham gia sẽ rẽ sang nhanh nào
2. Bên trái màn hình: **Chuỗi Điều kiện Logic**. Ví dụ: Nếu bạn không tự tin giải thích khái niệm trung vị ⇒ Bạn nên tham gia Datatalk\#2 - Đọc-Hiểu. Nếu bạn tự tin ⇒ bạn nên tham gia Datatalk\#3 - Tư Duy Data.
3. Bạn sẽ thấy \(1\) và \(2\) thật ra là cùng một câu chuyện: Cây Logic có thể được diễn đạt dưới dạng 1 chuỗi **IF** ... **ELSE** ... **THEN**

Máy tính cũng có ngôn ngữ riêng, thường là ngôn ngữ **Logic** và **Toán Học**. Các mệnh đề IF-ELSE, các mô tả điều kiện, các hướng dẫn để máy hiểu sẽ ở dưới dạng: So sánh &lt; &gt; =, biến đổi toán học đơn giản cộng-trừ-nhân-chia, cho đến phức tạp như Tích Phân, Đạo Hàm, Xác xuất.

{% hint style="info" %}
Ví dụ, trong trắc nghiệm Data Persona, có điều kiện: Nếu người trả lời đã biết nhiều Data nên gợi ý họ tham gia các **Datatalk\#3 và \#4** có kiến thức sâu hơn và bỏ qua các Datatalk đơn giản **\#1 và \#2**. Để diễn dịch nó cho máy tính:

1. **Số hoá "mức-độ-biết"** thành **Điểm** của người trả lời, qua các câu hỏi 1-3, cho điểm theo từng lựa chọn
2. **IF** Điểm &gt; 3 **THEN** người trả lời nên tham gia Datatalk\#3 và \#4, có thể skip \#1 và \#2
3. **ELSE** Datatalk\#1 và \#2 ⇒ Thuật toán phải có tính "Toàn vẹn", luôn trả kết quả \(gì đó\)
{% endhint %}

## Đến... Trí Tuệ Nhân Tạo \(AI\)

![](../../.gitbook/assets/image%20%2820%29.png)

Trở lại với Robot giao hàng của chúng ta, và bài toán giống-giống mà khác:

![](../../.gitbook/assets/image%20%286%29.png)

{% tabs %}
{% tab title="Hỏi" %}
**Bạn thấy có điểm chung của 2 "ứng dụng" đã tương tác bên trên?**

* Máy Tính: Nhận `input` gì từ bạn?
* Máy Tính: Trả ra `output` gì?
* Bạn nghĩ có thể thương mại hoá các ứng dụng trên như thế nào?
{% endtab %}

{% tab title="Hints" %}
* **Điểm chung:** Thuật toán nhận một input từ con người, và trả ra một output.
* **Input:** Hình vẽ, Video
* **Output:** Đoán đồ vật được vẽ, cho điểm "khẩu hình" khớp lời
{% endtab %}
{% endtabs %}

* **Hãy viết "thuật toán" mới để Robot giao đến Nhà màu Hồng?**

Bạn có thấy phiền không? Và nếu chúng ta có một vạn ngôi nhà màu hồng ở các địa hình khác nhau? Chúng ta phải viết một vạn thuật toán Trái-Phải-Lên-Xuống như vậy?

> Nếu chúng ta có thể đơn giản chỉ cần nói: Robot giao đến nhà màu hồng? Và, nó tự tìm con đường của riêng nó?

Đặt vấn đề như vậy, chúng ta đã chuyển từ các Thuật Toán đơn giản lên **Trí Tuệ Nhân Tạo**.

{% hint style="success" %}
**Hoạt Động \#1**

1. Vẽ vời một chút: [Quick, Draw!](https://quickdraw.withgoogle.com/)
2. Thử thách nhép miệng chuẩn theo bài: [Lipsync Scoring](https://experiments.withgoogle.com/lipsync)
{% endhint %}

Bạn có nhận ra: Bạn vừa tương tác với **Trí Tuệ Nhân Tạo**?

> **Trí tuệ nhân tạo:** máy móc có khả năng mô phỏng, bắt chước các chất năng "nhận thức" của con người: Nghe, nhìn, đọc, giao tiếp, chơi cờ, sáng tác nghệ thuật, ra quyết định \(gợi ý nội dung, đánh giá rủi ro, dự đoán tương lai\)...

## ML: Máy học thế nào?

> “Tôi nói đến đâu rồi nhỉ. À, Học Máy, nó cũng giống như cách con người học thôi. Người ta dạy máy móc y như cách con người được dạy dỗ”. \[...\] À, vậy thì hãy dạy máy như dạy một đứa trẻ. “Cô nghĩ một đứa trẻ học về thế giới như thế nào?”, hắn hỏi. \[…\] “Người ta cho chúng những ví dụ”, hắn tự đáp. Đây là một con chó, đây cũng là một con chó, đây là một con chó khác. Chỉ cho đứa trẻ một trăm lần, và gọi đó là con chó. Đứa trẻ rồi sẽ học được đó là chó. — _Đặng Huỳnh Mai Anh \(2020\). Truyện ngắn "Học Máy"_

Vậy cái Trí Tuệ Nhân Tạo làm cách nào mà nhìn được cái hình vẽ xấu ỉn trên là một **Máy Rửa Chén.** Dám cá là còn Sáng tạo hơn khối chúng ta.

À, vì Thuật toán đằng sau `Quick, Draw!` đã "học" **147,814 bức vẽ** Máy Rửa Chén từ đèm đẹp đến xấu banh của người dùng Internet. Đây là các "ví dụ" nó đã học.

![](../../.gitbook/assets/image%20%2823%29.png)

Mỗi khi so phải giải thích về **Machine Learning \(ML\)** thật dễ hiểu, tôi ưa lấy ví dụ bằng: Thay vì một chuỗi mệnh đề IF-ELSE cổ điển, ta dạy máy móc như một đứa trẻ. Việc cho máy tính xem 147,814 bức vẽ cái máy giặt làm tôi liên tưởng đến việc dạy cho những đứa trẻ nhận biết đồ vật, chữ cái, hình học bằng việc chỉ cho chúng xem những thẻ hình.

Và, sau khi chúng trả lời, bảo chúng "Đúng rồi!" \(Hoan hô\) hoặc "Sai rồi" \(Mặt buồn\).

Máy thật sự cũng học như vậy.

## Dạy mô hình ML của bạn

{% hint style="success" %}
**Train mô hình Machine Learning của bạn**

1. Truy cập: [https://teachablemachine.withgoogle.com/train](https://teachablemachine.withgoogle.com/train)
2. **Class 1** & **Class 2** là các nhóm muốn phân loại. Tuỳ theo ý của bạn, có thể đổi lại tên, nhưng trong trường hợp của mình, mình muốn phân loại: `Class 1 - Sách Hai-Mươi-Bảy` và `Class 2 - Sổ ghi chép`
3. Qua Camera, xoay trở Sách và Sổ ở nhiều góc độ \(Bạn có thấy giống cách iPhone học nhận diện gương mặt bạn?\) ⇒ Hình dung là chúng ta đang tự tạo ra thẻ hình để dạy "đứa trẻ"
4. Bấm **"Training"**
5. Sau khi train xong, ở khung **Preview** sẽ nhận diện hình ảnh của bạn \(`Input`\). Mình giơ thử sách Hai-mươi-bảy để xem Máy Tính có nhận ra không? ⇒ Mình đưa sách ở góc nghiêng \(hơi làm khó\) - Máy Tự tin Máy đúng: 84%
{% endhint %}

![](../../.gitbook/assets/image%20%2821%29.png)

Giống như "đứa trẻ" tiến bộ nhờ feedback của cha mẹ: "Đúng rồi! Hoan hô" - "Sai rồi. Lại nè". Thì Máy cũng vậy.

![](../../.gitbook/assets/image%20%2824%29.png)

{% hint style="success" %}
Bấm vào **`Under the hood`** trong cột **Training**.
{% endhint %}

* Khi bạn bấm `train`, máy sẽ chia hình ảnh của bạn thành **Training sample** \(đưa cho "đứa trẻ" học\) và **Test sample** \(đưa để kiểm tra "đứa trẻ"\)
* **Accuracy per class \(Độ chính xác trên mỗi nhóm\)**: % lần mô hình đoán đúng trên tập Test
* **Confusion Matrix:** Tương quan giữa kết quả mô hình đoán và kết quả thực tế
* Accuracy được đo trên Training sample và Test sample ⇒ Để coi đứa nhỏ có học "vẹt" không \(Đoán rất tốt trên training sample, nhưng đoán tệ trên test sample\)
* Máy sẽ nỗ lực học cho đến khi tối ưu được các chỉ số để đo tính đúng đắn \(Accuracy bên trên không phải là chỉ số duy nhất. Đọc thêm: [AUC-ROC](https://noron.vn/post/tim-hieu-chi-tiet-ve-auc---roc-trong-machine-learn-1fz9nhqo5ut)\)

## Ứng dụng trong Cuộc Sống

Cuối cùng, để nói về ứng dụng của Thuật Toán \(AI & ML\) trong đời sống, ta hãy điểm qua các chủ đề phồ biến và ứng dụng của chúng.

{% hint style="warning" %}
Thuật toán không nhất thiết là ML hay AI, thuật toán có thể là những logic đơn giản do con người thiết lập \(**Rule-based**\)
{% endhint %}

Với các chủ đề bên dưới, bạn sẽ thiết kế một thuật toán rule-based như thế nào?

### Các chủ đề phổ biển

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left">M&#xF4;</th>
      <th style="text-align:left">&#x1EE8;ng d</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">&#x1AF;u ti&#xEA;n (Prioritization)</td>
      <td style="text-align:left">Ranking c&#xE1;c l&#x1EF1;a ch&#x1ECD;n &#x111;&#x1EC3; t&#xEC;m ra l&#x1EF1;a
        ch&#x1ECD;n t&#x1ED1;t nh&#x1EA5;t (theo ti&#xEA;u ch&#xED; c&#x1EE5; th&#x1EC3;)</td>
      <td
      style="text-align:left">
        <ul>
          <li>K&#x1EBF;t qu&#x1EA3; Google Search</li>
          <li>Th&#x1EE9; t&#x1EF1; &#x1B0;u ti&#xEA;n trong Gmail</li>
          <li>G&#x1EE3;i &#xFD; &#x111;&#x1B0;&#x1EDD;ng ng&#x1EAF;n nh&#x1EA5;t, h&#xE3;ng
            bay r&#x1EBB; nh&#x1EA5;t</li>
          <li><a href="https://ichi.pro/vi/cach-alphago-cua-deepmind-tro-thanh-ky-thu-co-vay-hang-dau-the-gioi-100224644496746">AlphaGo: c&#x1EDD; v&#xE2;y</a>
          </li>
        </ul>
        </td>
    </tr>
    <tr>
      <td style="text-align:left">Ph&#xE2;n lo&#x1EA1;i (Classification)</td>
      <td style="text-align:left">D&#x1EF1;a v&#xE0;o c&#xE1;c thu&#x1ED9;c t&#xED;nh (features) quan s&#xE1;t
        &#x111;&#x1B0;&#x1EE3;c c&#x1EE7;a c&#xE1; th&#x1EC3; (observations) ph&#xE2;n
        v&#xE0;o c&#xE1;c nh&#xF3;m kh&#xE1;c nhau</td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>Ph&#xE2;n lo&#x1EA1;i ng&#x1B0;&#x1EDD;i tham gia/kh&#xE1;ch h&#xE0;ng
            (t&#x1B0;&#x1A1;ng t&#x1EF1; nh&#x1B0; Data Persona)</li>
          <li>Ph&#xE2;n lo&#x1EA1;i th&#x1B0; r&#xE1;c (spam)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">T&#x1B0;&#x1A1;ng quan (Link)</td>
      <td style="text-align:left">T&#xEC;m ra m&#x1ED1;i t&#x1B0;&#x1A1;ng quan</td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>Thu&#x1EAD;t to&#xE1;n Dating c&#x1EE7;a Tinder</li>
          <li>Youtube g&#x1EE3;i &#xFD; c&#xE1;c b&#xE0;i nh&#x1EA1;c li&#xEA;n quan</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">L&#x1ECD;c (Filtering)</td>
      <td style="text-align:left">L&#x1ECD;c nhi&#x1EC5;u v&#xE0; t&#x1EAD;p trung v&#xE0;o c&#xE1;c th&#xF4;ng
        tin quan tr&#x1ECD;ng</td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>X&#x1EED; l&#xFD; &#xE2;m thanh, h&#xEC;nh &#x1EA3;nh</li>
          <li>News feed c&#x1EE7;a Facebook</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

{% hint style="success" %}
**Hoạt Động \#2**

1. Minh hoạ thuật toán Phân loại \(Clustering\): Audio Clustering [LINK](https://experiments.withgoogle.com/ai/drum-machine/view/)
2. AI và Ngôn ngữ cơ thể bạn: [LINK](https://experiments.withgoogle.com/billtjonesai)
3. Từ 04 nhóm thuật toán, bạn sẽ thiết kế ra các ứng dụng nào?
{% endhint %}

### Trí tuệ Người & Máy 

* **Rule-based** \(bởi con người\) không nhất thiết kém hiệu quả hơn ML/AI. Có rất nhiều bài toán \(nhất là khi Data còn hạn chế\), rule-based sẽ hợp lý và hiệu quả hơn
* **Rule-based** còn có ưu điểm là dễ hiểu, dễ thực hiện. Nhưng vì vậy, rule-based chỉ áp dụng được trong những trường hợp con người hiểu tốt vấn đề của họ.
* **Machine Learning** lại phù hợp cho các bài toán không thể viết thành list IF-ELSE. Dù vậy con người không nhất thiết hiểu chuỗi logic cụ thể bên trong quyết định của chúng. Một câu chuyện kinh điển: Quân đội Mỹ phát triển một thuật toán nhận biết xe tăng địch. Kết quả rất tốt trên training/test samples, nhưng trong thực tế lại kém chính xác. Họ cũng quan sát được là vào những ngày nhiều mây, thuật toán có xu hướng nhận định mọi xe tăng chúng quan sát được là xe tăng địch. Sau đó, nhóm phát triển phát hiện ra họ vô tình chụp sample xe tăng địch vào những ngày nhiều mây ⇒ Thuật toán đã học bầu trời nhiều mây hay trời nắng đẹp \(rất lãng mạn\), chứ không chịu học phân biệt xe tăng \(rất phẩn chiến\)

Thế thật nghĩ là Máy Móc cũng có những hạn chế của chúng, lần này hoặc lần khác ta lại thấy Google Maps chỉ đường "ngu" cho mình, hoặc là mình "ế" mốc cả ra mà cứ ngày đêm quảng cáo thuốc ngừa thai.

> Nhưng chúng ta, con người chúng ta, càng ngày lại càng dựa dẫm và có niềm tin mù quáng vào con người. Ta luôn nghĩ những gì Máy Móc và Thuật Toán gợi ý luôn thông minh, ưu việt và ít sai sót hơn của con người.

Search Engines \(như Google\) có khả năng thao túng cách chúng ta nhìn nhận thế giới. Có câu nói đùa rằng: `Chỗ kín đáo nhất trên thế giới, là trang thứ 2 của kết quả tìm kiếm Google`. Bao nhiêu trong chúng ta sẽ lao vào kết quả đầu tiên của Google, và dừng lại ở 10 kết quả đầu tiên.

> Thuật toán, ML, AI cho con người chúng ta những sự tiện lợi. Thật dễ dàng để sai bảo chúng, kể cả sai bảo chúng chịu trách nhiệm ra quyết định, lựa chọn dùm chúng ta, và con người chẳng cần suy nghĩ nữa.

Mong rằng hiểu thêm một chút về Thuật Toán để tất cả chúng ta đều nhận ra máy móc cũng có những hạn chế và con người cũng có những hạn chế. Và, nếu được, thỉnh thoảng hãy "hoài nghi" lại các kết quả máy móc đưa cho bạn: Đi ra ngoài list nhạc được Spotify suggest, dừng lại và dùng suy luận con người xem con đường Google Maps gợi ý có phải là ngắn nhất, và các sản phẩm hiện ra đầu tiên khi bạn tìm kiếm trên Google đã là tốt nhất và rẻ nhất cho bạn chưa?

Máy móc có thể hỗ trợ, nhưng không thể hoàn toàn thay thế cách chúng ta lựa chọn trong cuộc sống.

Như một đứa trẻ, càng cho chúng xem nhiều ví dụ chúng càng thông minh. Thuật toán, ML/AI trở quyền lực như vậy, nhờ: **Big Data**. Lượng thông tin cá nhân, hành vi, digital footprint hàng tỷ người để lại trên mạng Xã hội, giúp chúng hiểu chúng ta hơn cả chúng ta hiểu chính mình. Khiến công nghệ đứng trước những câu hỏi nền tảng về xã hội và loài người.

