# Data Thinking: Quy Nạp

Trong [**Datatalk\#2**](../2-everyone-can-read-data/), ta đã đề cập đến mô hình giải quyết vấn đề bằng data: PPDAC.

Thế nhưng câu hỏi lớn hơn đó là: Ta không chỉ muốn biết những điều nhìn thấy được trong data, ta muốn hiểu những điều bên ngoài Data ta đang có, ta muốn dự đoán, và ta muốn hiểu được lý do \(như một thôi thúc tự nhiên nhất của con người\).

> Thống kê như một người phụ nữ đẹp — lấp lửng vừa đủ và không bao giờ có thể biết được chắc chắn.

## Học từ Data: Qua trình ngoại suy Quy Nạp

Data cho ta biết những gì đã xảy ra, về cơ bản, ta không thể thay đổi quá khứ. Nhưng tương lai, ta có thể thay đổi, bằng các hiểu và học từ \(Data\) quá khứ.

Bên dưới là biểu đồ các cấp độ của phân tích data:

1. Đi từ trái sang phải \(trục ngang\): Là sự tăng tiến của mức độ phức tạp
2. Đi từ dưới lên trên \(trục ngang\): Là giá trị của phân tích data đem lại

Khao khát của mọi doanh nghiệp, tổ chức, nghiên cứu, người phân tích dữ liệu, là bước được lên các nấc cao hơn. Như bạn thấy, việc mô tả, minh hoạ, tìm được các thông tin thú vị như trong phần lớn ví dụ của [**Datatalk\#2**](../2-everyone-can-read-data/) chỉ mới là hai bậc thấp nhất: **Phân tích Mô Tả** _- Điều gì đã xảy ra? \(Descriptive Analytics\)_ và **Phân tích Chẩn Đoán** _- Vì sao chúng xảy ra? \(Diagnostic Analytics\)._

Chúng cho ta biết về quá khứ, nhưng hiểu biết đó chỉ có ý nghĩa khi chúng giúp ích được ta trong tương lai: **Phân tích Dự đoán** _- Điều gì sẽ xảy ra \(Predictive Analytics\)_ và **Phân tích Đề Xuất** _- Điều gì sẽ dẫn đến điều gì? Ta làm gì để điều này xảy ra \(Prescriptive Anaytics\)._

![Source: STAGES OF DATA ANALYTICS MATURITY \(ADAPTED FROM DAVENPORT &amp; HARRIS 2007 / GARTNER 2012\)](../../.gitbook/assets/image%20%2879%29.png)

Việc trích xuất hiểu biết và thông tin từ Data, là quá trình ngoại suy Quy Nạp. Ta khái quát hoá những gì trực tiếp quan sát được trong một mẫu data thu thập được, thành những thông tin \(phỏng đoán\) về những quan sát nằm bên ngoài mẫu mà ta không quan sát được. Ví dụ: Quan sát quá khứ ⇒ Dự đoán tương lai; Quan sát những ca bệnh trong quá khứ ⇒ Chẩn đoán cho ca mới; Khảo sát mẫu vài chục ngàn người ⇒ Rút ra kết luận về xu hướng của cả thị trường tiêu dùng.

## Từ Data đến bên-ngoài-Data

> Một người Việt Nam trên 18 tuổi trung bình sẽ trải qua mấy mối tình?

Xin mượn bài toán trên làm một ví dụ để minh hoạ tính Ngoại Suy Quy Nạp ta đang đề cập.

Một sự thật là để trả lời câu hỏi trên, ta không thể đi hỏi tất thảy hơn 90 triệu người Việt Nam. Ta sẽ chỉ đủ tài nguyên để hỏi một Mẫu \(nhóm người được chọn để thu thập dữ liệu\) - nhỏ hơn rất nhiều so với con số 90 triệu người.

Bài toán quy nạp đặt ra là: Ta phải đi từ nhỏ đến to, từ Data trên một tập mẫu, suy rộng ra, để đến một kết luận cho toàn thể người Việt Nam.

Đây là một ví dụ, nhưng rất nhiều cuộc khảo sát khác cũng diễn ra tương tự... và gặp phải những vấn đề tương tự.

### 04 tầng Ngoại Suy

![](../../.gitbook/assets/image%20%2878%29.png)

{% hint style="info" %}
Như biểu đồ bên trên, ta chia quá trình ngoại suy từ **quan sát trên một mẫu nhỏ** ra **kết luận trên một quần thể lớn,** thành 4 tầng:

1. **Data \(dữ liệu\):** câu được khai báo \(số mối tình\) ta thu thập được từ mẫu các đối tượng được hỏi. Ví dụ: Ta thu thập được câu trả lời của 1,000 người Viêt Nam trên 18 tuổi, tình cờ bắt gặp trên đường \(Tp. Hồ Chí Minh\).
2. **Mẫu:** câu trả lời thực tế của những đối tượng trong mẫu. Lưu ý ở đây: Có thể có sự khác biệt giữa C_âu trả lời được khai báo_ và C_âu trả lời thực tế_.
3. **Quần thể nghiên cứu:** câu trả lời thực tế của các đối tượng có thể nhận dạng và lấy mẫu. Là hàng triệu người Việt Nam trên 18 tuổi, ta có thể gặp trên đường để hỏi \(nhưng ta và họ đã không có duyên gặp nhau\)
4. **Quần thể mục tiêu:** câu trả lời thực tế của các đối tượng trong phạm vi nghiên cứu. Ở đây là hàng triệu người Việt Nam trên 18 tuổi, gồm cả những người ta dễ gặp trên đường hay những không dễ gặp trên đường \(nguyên thủ quốc gia hay tù nhân, người bịnh, người Việt Nam sống ở nước ngoài, vân vân\).
{% endhint %}

Nguyên tắc chung là: Khi bạn đi từ to đến nhỏ, từ nhiều thông tin đến giản thể của thông tin, suy luận có thể tuyệt đối. Nhưng theo chiều ngược lại, đi từ nhỏ đến to, ngoại suy thông tin cho những điều không quan sát, bạn phải trám vào đó bằng những giả thuyết và phỏng đoán nhất định. Điều đó khiến **mọi thống kê đều mang tính tương đối**.

Thiếu sót rất dễ xảy ra khi chuyển dịch từ tầng này sang tầng khác, dẫu cho nỗ lực của Khoa học Thống kê là giảm thiếu thiếu sót và chuyển tầng êm mượt nhất có thể.

> Có 03 loại nói dối: Nói dối, nói dối nghiêm trọng, và... những con số thống kê. — Benjamin Disraeli

### \(1\) Sai sót thu thập

Khi ngoại suy từ kết quả trên Data lên "sự thật" trên Mẫu, ta phải "tin" rằng dữ liệu thu thập được của người tham gia khảo sát là đúng đắn.

Dù vậy, không có nghĩa là người trả lời luôn nói thật. Trong các cuộc khảo sát tương tự ở Mỹ và Anh, người ta nhận ra Đàn Ông có xu hướng nói quá lên số mối tình của mình, còn Phụ Nữ thì có xu hướng nói giảm xuống. Vì nhiều lý do: Đàn ông muốn khoác lác về độ trăng hoa của mình, Phụ nữ chỉ tính các mối tình nghiêm túc hoặc các mối họ muốn quên đi cho rồi, có người không nhớ chính xác, có người làm tròn lên, có người làm tròn xuống.

Người được phỏng vấn không bị ảnh hưởng tâm lý bởi người phỏng vấn, hoặc không có **lỗi-hệ-thống** nào đến từ bảng hỏi hay cách hỏi. Năm 2017, hãng hàng không giá rẻ Ryanair công bố rằng 92% hành khách hài lòng với trải nghiệm bay cùng họ. Rốt cuộc người ta phát hiện ra bảng khảo sát của Ryanair chỉ cho khách hàng các sự lựa chọn sau: Tuyệt vời, Cực kỳ tuyệt vời, Tốt, Hài Lòng, OK. Trong một cuộc khảo sát khác, Ryanair nằm chót bảng trong số 20 hãng hàng không ở Châu Âu.

### \(2\) Sai sót chọn mẫu

Đi từ Mẫu lên quần thể nghiên cứu có lẽ là bước dễ xảy ra sai sót nhất, vì đảm bảo để chọn mẫu đúng là việc không dễ dàng.

Nguyên tắc chọn mẫu lại nghe cực kỳ đơn giản: **Đảm bảo sự** **Ngẫu nhiên.**

Như thế nào là Ngẫu nhiên? Giống như khi ta quay xổ số hay lô tô, ngẫu nhiên đích thực là khi không có bất kỳ một khuynh hướng thiên về kết quả/lựa chọn nào, không thiên vị bất kỳ ai.

Tại sao sự **Ngẫu nhiên** lại quan trọng?

Có một ví dụ hình tượng cho tính Ngẫu nhiên trong chọn mẫu. Quần thể nghiên cứu của bạn là một nồi súp, bạn cần nêm nếm để gia giảm gia vị. Nhưng bạn, dĩ nhiên, không thể húp hết nồi. Bạn nếm thử một muỗng súp \(mẫu\), mùi vị bạn cảm nhận được trên muỗng súp đó đại diện cho nồi vị của cả nồi súp. Bạn gia giảm gia vị dựa trên "quan sát" của mẫu đó.

Trước khi nếm, bạn cần khuấy đều \(cũng giống như khi nhặt bóng sô trong lô tô, người ta phải quay lồng bóng\). Khuấy đều để đảm bảo rằng phần súp bên dưới hay bên trên đều có khả năng được "múc", nếu không thì sẽ chỉ có lớp bên trên có một xác suất cao hơn hẳn được chọn, vậy thì lúc này bạn phạm rủi ro rằng "muỗng súp" bạn múc không mang tính đại diện cho cả nồi súp \(có thể nồi súp bị trên mặn dưới ngọt\).

Việc lựa chọn cá thể người trong mẫu cũng vậy. Tính Ngẫu Nhiên giúp ta đảm bảo rằng mẫu mang tính đại diện, và những quan sát trên mẫu có thể ngoại suy cho tổng thể.

Trong thực tế có rất nhiều yếu tố dẫn đến một thiên hướng nào đó ta không lường trước được, và điều đó phá vỡ sự Ngẫu Nhiên, ví dụ:

* Khảo sát về số lượng bạn tình, ta lại vô tình đứng khảo sát ở phố đèn đỏ
* Khảo sát về thu nhập, tiến hành gửi khảo sát qua email
* Những người tình nguyện tham gia một cuộc khảo sát về sức khoẻ, thường vốn đã quan tâm về sức khoẻ

{% hint style="success" %}
**Hoạt Động\#1:** Thử nghĩ xem các trường hợp trên sẽ làm sai lệch kết luận của chúng ta như thế nào?
{% endhint %}

### \(3\) Sai sót... lạc đề

Cuối cùng, là kiểu sai sót "lạc đề", giữa: Quần thể nghiên cứu và Quần thể mục tiêu. Vì dụ, muốn trả lời câu hỏi: Một người Việt Nam trên 18 tuổi trung bình sẽ trải qua mấy mối tình? Lại đi hỏi ở trường tiểu học.

Ngoài ra, có những khác biệt nhất định giữa Quần thể nghiên cứu \(nếu ra chọn cách phỏng vấn ngẫu nhiên trên đường phố\) và Quân thể mục tiêu \(ví dụ ta không thể tiếp cận tù nhân, người bịnh, người Việt Nam sống ở nước ngoài\). Chúng ta có thể muốn biết sự thật "toàn vẹn" trên tất cả mọi người, nhưng điều này là bất khả thi trong thống kê.

## Tính tương đối của Thống Kê

Chúng ta đã nói về tư duy Ngoại Suy Quy Nạp trong Data, sau khi bàn qua tất cả những sai sót có thể xảy ra, hẳn sẽ khiến bạn phải nhiều mày hoài nghi trước bất kỳ kết luận khái quát nào.

Tôi có một cuốn sách Thống Kê ưa thích thường đặt trên bàn làm việc, tôi đọc đi đọc lại, gần như thuộc mọi chỗ chú thích bằng bút chì bên lề giấy. Có lúc tôi đọc lại vài chương, có khi vài trang. Nhưng phần tôi đọc lại nhiều nhất là trang đầu tiên, lời đề viết rằng:

> “Viết cho những nhà thống kê học ở khắp mọi nơi, với những phẩm chất của họ: Tính kỷ luật, sự bao dung, tính chính trực, và niềm khát khao được dùng dữ liệu một cách tốt nhất - có thể” — David Spielgelharter. The Art of Statistics: Learning from Data.

Một câu xúc tích như đầy đủ những cái cần: Tính kỷ luật để hạn chế sai sót. Dù vậy sai sót là không thể tránh khỏi, nên cần Sự Bao Dung với Data và với chính mình. Tính chính trực để thừa nhận những sai sót và hạn chế. Cuối cùng, khao khát để mỗi ngày làm mọi thứ tốt hơn từng chút một, tiệm cận đến sự tốt nhất ta có thể.

Dữ liệu và thống kê cho ta một ước lượng mang tính tương đối, vì cuộc sống có lẽ quá phức tạp để diễn tả một cách tuyệt đối.

Cũng vì thế Thống Kê thường đi cùng Xác Suất, vì nếu Thống Kê là ngành khoa học của việc đúc kết nên những sự thật tương đối, vì Xác Suất là đại lượng của sự tương đối.

## Recap

* Có 4 cấp bậc của phân tích dữ liệu, từ đơn giản đến phức tạp: **Phân tích Mô Tả** _- Điều gì đã xảy ra? \(Descriptive Analytics\),_ **Phân tích Chẩn Đoán** _- Vì sao chúng xảy ra? \(Diagnostic Analytics\),_ **Phân tích Dự đoán** _- Điều gì sẽ xảy ra \(Predictive Analytics\),_ **Phân tích Đề Xuất** _- Điều gì sẽ dẫn đến điều gì? Ta làm gì để điều này xảy ra \(Prescriptive Anaytics\)._
* Việc trích xuất hiểu biết và thông tin từ Data, là quá trình ngoại suy Quy Nạp. Ta khái quát hoá những gì trực tiếp quan sát được trong một mẫu data thu thập được, thành những thông tin \(phỏng đoán\) về những quan sát nằm bên ngoài mẫu mà ta không quan sát được.
* Ta chia quá trình ngoại suy từ **quan sát trên một mẫu nhỏ** ra **kết luận trên một quần thể lớn,** thành 4 tầng:
  1. **Data \(dữ liệu\):** câu được khai báo \(số mối tình\) ta thu thập được từ mẫu các đối tượng được hỏi.
  2. **Mẫu:** câu trả lời thực tế của những đối tượng trong mẫu.
  3. **Quần thể nghiên cứu:** câu trả lời thực tế của các đối tượng có thể nhận dạng và lấy mẫu.
  4. **Quần thể mục tiêu:** câu trả lời thực tế của các đối tượng trong phạm vi nghiên cứu.
* Ở mỗi bước chuyển, có cái sai sót có thể khiến việc Ngoại Suy Quy Nạp không chính xác. Điều đó khiên Thống kê là một phiên bản "sự thật" tương đối. Cũng vì vậy, Thống Kê đi liền với Xác suất - như một đại lượng cho sự tương đối.

