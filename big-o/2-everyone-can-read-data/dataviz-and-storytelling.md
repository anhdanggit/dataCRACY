---
description: DataViz = Data Visualization
---

# DataViz & Storytelling

> The numbers have no way of speaking for themselves. We speak for them. We imbue them with meaning. — Nate Silver, The Signal and the Noise.

Ở phần trước, chúng ta đã đề cập một số khái niệm căn bản: Phần Trăm, Số Trung Bình, Khoản Tin Cậy. Các dạng dữ liệu phân loại và số.

Chúng ta đã sẵn sàng để "nhâm nhi" một vài câu chuyện qua data. Đừng lo lắng vì chúng tôi sẽ đi cùng với bạn.

## PPDAC

Ngày trước khi còn đi dạy IELTS dạo, tôi thường để mọi người bắt đầu bằng kỹ năng "nghĩ": Xây dựng dàn bài. Một nội dung truyền tải, là bài đọc/bài nghe \(bởi người khác\), bài viết/bài nói \(bởi mình\) đều đi theo một vài logic touch-points \(Mở bài, luận điểm, triển khai, Kết bài...\) mà nếu mình nắm được việc hiểu ý đồ của người truyền tải sẽ tốt hơn.

Để phổ cập về data, chúng ta hãy đi theo hướng tiếp cận tương tư: Các touch-points và cách mà data được thu thập, phân tích, rồi "storytelling".

Đây cũng là cách tiếp cận của giáo dục thống kê hiện đại, trọng tính problem-solving nhiều hơn là cách truyền thống mà bao thế hệ đã "xác chết thống kê" với một danh sách các công thức, khái niệm, định lý mà không hiểu chúng được dùng thế nào, và tại sao cần chúng để trả lời các câu hỏi bằng data.

* **Problem:** Xác định vấn đề quan tâm, ta cần trả lời những câu hỏi gì?
* **Plan:** Cho vấn đề đó ta cần "đo đếm" những thông tin, sự kiện, tính chất nào? Vậy cần thu thập những dữ liệu đó ra sao?
* **Data:** Tiến hành thu thập xử lý
* **Analysis:** Phân tích, bao gồm: Tạo bản data \(cột và dòng\), dùng các hàm gộp, so sánh-tính toán, vẽ biểu đồ, tìm các quy luật, tạo thành các giả thuyết
* **Conclusion:** Diễn dịch, kết luận, truyền đạt, hoặc thêm các câu hỏi mới \(xác minh giả thuyết\) trở lại bước P.

![](../../.gitbook/assets/image%20%2863%29.png)

Source: [The University of Auckland](https://www.stat.auckland.ac.nz/~wild/d2i/articles/1.4%20Place%20of%20data%20analysis%20in%20problem%20solving_ARTICLE.pdf)

## Đọc biểu đồ

Ta có thể bắt đầu đọc một báo cáo số liệu bằng cách "áp" chúng vào framework PPDAC như vậy. Một báo cáo tốt là báo cáo làm tốt từng bước trong chu trình đó

> Chúng ta phải thừa nhận rằng chúng ta đang kể một câu chuyện. Câu chuyện thì không phải là chân lý. Khó tránh khỏi những đánh giá có thể có, dù ta chỉ muốn trao đổi chứ không hề có ý thuyết phục hay chứng minh chân lý. Dù sao cách tốt nhất ta có thể làm là thiết kế tốt và cảnh báo trước những sai sót có thể có. — The Art of Statistics, David Spiegelharter.

Cách đọc biểu đồ \(một biểu đồ tốt cần đủ các thông tin sau\):

1. Nhìn vào tiêu đề: Chủ đề gì \(Problem\)? Các chú thích về các đại lượng để đo lường trên Trục ngang \(Trục X/Trục hoành\) và Trục dọc \(Trục Y/Trục tung\)?
2. Mẫu quan sát: Thời gian, các chủ thể trong mẫu
3. Trục ngang: Đại lượng gì, đơn vị?
4. Trục dọc: Đại lượng gì, đơn vị?
5. Các chú giải khác
6. Các tính năng tương tác kèm theo: Animation theo năm, thêm/bớt các nhóm, đổi đơn vị
7. Nguồn

## Hạnh Phúc

Tiếp tục câu chuyện về [Hạnh Phúc của phần trước](du-lieu-ky-vong-and-tin-cay.md#hanh-phuc-bien-phan-loai),

### Tiền và Hạnh Phúc

* **Problem:** Tiền có đem lại cho ta hạnh phúc? Các sự kiện trong cuộc đời ảnh hưởng thế nào đến sự hạnh phúc?
* **Plan:**
  * Ta cần đo được sự Hạnh Phúc ⇒ Chỉ số hạnh phúc \(Thang Cantril\)
  * Ta cần đo được sự giàu có \(Tiền bạc\) ⇒ GDP per capita \(GDP trên đầu người\)
  * Ta cần một tập quan sát \(mẫu\): Các quốc giá trên thế giới
* **Analysis:**
  * Ta thấy các nước có mức thu nhập bình quân đầu người cao có xư hướng có chỉ số trung bình hạnh phúc cao hơn. Nói cách khác, những người được phỏng vấn ở các nước giàu có xu hướng khai rằng họ có mức thoả mãn trong cuộc sống cao hơn những người ở nước nghèo
  * Ở đây biểu đồ chấm được dùng để thể hiện **mối liên quan giữa hai đại lượng trên cột X và Y**: Chỉ số hạnh phúc cantril từ 0-10\(trục dọc\) và GDP per capita đã điều chỉnh lạm phát và khác biệt giá trên từng nước \(trục ngang\)
  * Mỗi chấm thể hiện một quốc gia
  * Các quốc gia lại phân theo châu lục, quy định bằng màu
  * Mức độ to/nhỏ theo dân số được thể hiện bằng độ to nhỏ của chấm tròn. Các chấm có một độ "trong" để không chấm to \(China\) không che khuất các chấm nhỏ khácc
* **Conclusion:**
  * Có sự tương quan giữa quốc gia giàu/nghèo và mức thoả mãn trung bình
  * Nhưng, tương quan không hẳn là nhân quả
  * Có những sự tương quan chỉ mang tính tình cờ \(Ta sẽ bàn trong [**Datatalk\#3**](../coming-soon./3-data-thinking.md)\) 

![](../../.gitbook/assets/image%20%2859%29.png)

### Sóng Gió Cuộc Đời

> Trải qua một cuộc bể dâu, Những điều trong thấy mà đau đơn lòng — Truyện Kiều, Nguyễn Du

![](../../.gitbook/assets/image%20%2861%29.png)

{% hint style="info" %}
Full-size chart [HERE](https://ourworldindata.org/happiness-and-life-satisfaction#how-do-common-life-events-affect-happiness)
{% endhint %}

* **Problem:** Các sóng gió trong cuộc bể dâu ấy \(Mất việc, kết hôn, hôn nhân tan vỡ, gáo bụa, sinh con\) ảnh hưởng thế nào đến hạnh phúc? Ta mất bao năm để "bình thường" trở lại?
* **Plan:**
  * Chỉ số hạnh phúc \(Thang Cantril\)
  * Quan sát các sự kiện \(Mất việc, kết hôn, hôn nhân tan vỡ, gáo bụa, sinh con\)
  * Để có thể trả lời câu hỏi sự kiện đó ảnh hưởng thế nào, ta cần cơ sở để so sánh, cần quan sát được Chỉ số Hạnh Phúc \(trước X năm so với mốc sự kiện\)
  * Để trả lời câu hỏi ta mất bao năm để "bình thường", cần quan sát được \(thêm Y năm soi với mốc sự kiện\)
  * Như vậy ở mỗi cá thể, ta cần phỏng vấn/thu thập được cảm nhận của họ về Hạnh Phúc trong X+Y năm \(đây là một nghiên cứu tốn kém\)
* **Analysis:** Hãy đọc phần chú thích bên dưới tên biểu đồ, chú thích trên 2 trục của biểu đồ
  * Trên cột dọc,
    * Là mức thay đổi của Chỉ số Hạnh Phúc. Ví dụ: -1.6 nghĩa là chỉ số hạnh phúc giảm đi 1.6 điểm. Đây là con số ước lượng \("estimate"\) hiểu nôm na là lấy **Giá trị Kỳ Vọng** của một nhóm người cùng trải qua sự kiện đó \(thất nghiệp\) vào cùng một năm - X năm trước sự kiện
    * Đường ngang đứt gạch ở mức "0", là quy ước về sự bình thường - **baseline** \(có thể mức trung bình của nhóm trải qua sự kiện đó trong một khung thời gian dài\) ⇒ Hãy đọc phần Nguồn bên dưới, bạn sẽ biết bạn cần tìm keywords gì để có thể đọc thêm về phương pháp của họ
  * Trên cột ngang,
    * Số năm trước và sau sự kiện, ví dụ: -4 nghĩa là 4 năm trước sự kiện, 4 nghĩa là 4 năm sau sự kiện
  * Mỗi điểm trên biểu đồ là giá trị trung bình của nhóm người trải qua cùng sự kiện đó, trong cùng một năm. Các điểm là một giá trị "ước lượng" - nên về hai phía của điểm có các thanh nhỏ, thể hiện **Khoản Tin Cậy**.
  * Các điểm này nối lại tạo thành đường thể hiện xu hướng \(**trendline**\)
* **Conclusion:**
  * Với sự kiện thất nghiệp, sự "hạnh phúc" của Phụ nữ giảm 0.6 điểm, trong khi đàn ông giảm 0.8 điểm. Có thể nói, **hạnh phúc của phụ nữ ít bị tác động bởi việc thất nghiệp hơn so với đàn ông**. So hai khoản tin cậy 95%, ta thấy với khoản của phụ nữ ở vị trí cao hơn \(gần đường baseline hơn\) và không có "overlap" với khoản tin cậy của đàn ông. Nói bằng ngôn ngữ thống kê, sự "ít bị tác động hơn này" có ý nghĩa thống kê \(statistically significant\). Suy diễn thêm, ta dễ thấy điều này có lý: Vì "thất nghiệp" ở phụ nữ, có thể đơn giản là họ chọn ở nhà để chăm sóc gia đình. Nếu vậy, việc gom những phụ nữ "thất nghiệp" vì họ theo chồng bỏ cuộc chơi với những phụ nữ "thất nghiệp" dù không theo ai tạo ra sự nhiễu trong kết luận. Ở tình huống này, ta sẽ cần đi lại vòng PPDAC để cân nhắc thêm: Lý do thất nghiệp.
  * Ở sự kiện Hôn Nhân Tan Vỡ, xem chừng cả hai phái đều bình thản khi sự kiện xảy ra. Dù trước sự kiện một vài năm, họ đều có chỉ số hạnh phúc thấp hơn mức baseline. Đàn ông có vẻ "đau đớn lòng" trong cuộc bể dâu này hơn chị em phụ nữ. Tuy nhiên, xét vào 2-4 năm trước ly hôn, có đoạn trùng ở hai khoản tin cậy nên chưa thể kết luận một-cách-thống-kê là đàn ông khổ sở hơn. Sự khổ sở này chỉ bắt đầu có ý nghĩa thống kê vào 1 năm trước ly hôn \(**chạm đáy nỗi đau**\). Để ngay lập tức khi ly hôn, hai bên vui trở lại. Đàn ông có dấu hiệu phấn chấn hẳn dù phụ nữ thì bình thản hơn. Nhưng baseline "0" nằm trong khoản tin cậy, nên quan sát này không có ý nghĩa thống kê. **Khuyến cáo:** Điều này không có nghĩa khuyến khích ly hôn. Không thể giật tít, ly hôn làm người ta hạnh phúc. Một tít bớt ảo hơn là, ly hôn làm người ta bớt khổ, nhưng hãy chỉ làm vậy khi bạn đã chạm đáy nỗi đau.
  * Với sự kiện chồng/vợ qua đời, sự kiện ảnh hưởng mạnh mẽ đến "Hạnh Phúc". Nhưng, đàn ông chỉ mất 1 năm để hồi phục \(1 năm sau sự kiện, khoản tin cậy đã giao lại với basline\), trong khi phụ nữ mất 2 năm. **Khuyến cáo:** Nhưng liệu điều đó có chính xác, sự kiện có phải là yếu tố duy nhất ảnh hưởng đến chỉ số của họ. Một năm trước khi chồng/vợ qua đời, phụ nữ vốn đã có chỉ số thấp hơn: Vì sao khi mà sự kiện còn chưa xảy ra? Họ chăm sóc chồng 1 năm trên giường bình? Lại trở lại bước P trong PPDAC.
  * Sự ra đời của một đứa trẻ, cha mẹ chúng đều khá viên mãn trong vòng 4 năm trước khi đứa trẻ ra đời. Đứa trẻ ra đời trong niềm vui của cha mẹ, nhưng có một hoài nghi nhỏ khi kết luận đứa trẻ ra đời khiến cha mẹ chúng hạnh phúc, vì cha mẹ chúng vốn đã hạnh phúc sẵn rồi. Khi một đứa trẻ ra đời, bao thứ phải lo toan, 3 năm đầu đời la giai đoạn nhiều vất vả thức khuya dậy sơm, cha mẹ chúng đều có sự giảm nhẹ trong thoả mãn cuộc sống, nhưng đến năm thứ 4-5 sau sinh sẽ trở về mức bình thường. Khuyến cáo: thoả mãn không nhất thiết là hạnh phúc, bậc cha mẹ ta có thể không thấy "tiện lợi" khi mang vác theo một nhóc tì suốt ngày ngoa ngoa khóc, nhưng... họ hạnh phúc \(tôi tin\).

## Cách ta trải qua Thời Gian

Thời gian là vàng. Và, thời gian cũng là thứ hiếm hoi trên đời công bằng cho tất cả chúng ta. Bất kể giàu ngheo, sang hèn, màu da sắc tộc, mỗi chúng ta có: 24 giờ một ngày, và 365 ngày một năm.

Ta đã trải qua một năm thế nào?

Thời gian của chúng ta trải đều cho những hạn mục giống nhau: Ăn, Ngủ, Làm việc và Thư giãn. Nhưng việc phân bổ thời gian thế nào lại là tự do của chúng ta, ta dành thời gian cho điều quan trọng nhất với mình. Những quan sát về cách dùng thời gian, cho ta biết thêm về chất lượng cuộc sống trên toàn thế giới.

Trong phần tiếp theo, ta sẽ trả lời thêm những câu hỏi về cách chúng ta trải qua thời gian của chúng ta.

{% hint style="success" %}
Với mỗi câu hỏi tiếp theo, bạn hãy thử đi theo mô hình **PPDAC** để hiểu về câu chuyện biểu đồ muốn truyền tải. Chúng mình sẽ đi thẳng vào các điểm chính.
{% endhint %}

Dữ liệu về Thời gian biểu có thể được thu thập bằng cách ngây thơ \(tương tự như chủ đều hạnh phúc\), hỏi trực tiếp: "Bạn dùng bao nhiều tiếng một ngày cho những việc gì?". Cho đến những hệ thống tracking phức tạp.

Ta sẽ tìm hiểu thông quá bài phân tích [Time Use \(Esteban Ortiz-Ospina, Charlie Giattino and Max Roser\)](https://ourworldindata.org/time-use#how-do-people-across-the-world-spend-their-time-and-what-does-this-tell-us-about-living-conditions) trên OurWorldinData.org

### Ta dùng thời gian thế nào

![](../../.gitbook/assets/image%20%2854%29.png)

* Con người chúng ta, trên toàn thế giới dành phần lớn thời gian để: Làm việc và Ngủ.
* Giữa các quốc gia và văn hoá lại có những khác biệt:
  * Người Ý \(vốn mang tiếng là lười\) chỉ làm việc bằng một nửa người Trung Quốc. Người Pháp \(cũng có tiếng trong top lười\) theo ngay sau người Ý.
  * Các nước Châu Á và đang phát triển, có xu hướng làm việc nhiều hơn. Có thể do họ chăm chỉ, hoặc họ buộc phải làm việc vất vả hơn vì điều kiện kinh tế chung của đất nươc.
  * Ngoài ra, ta cũng thấy những yếu tố văn hoá thể hiện qua đây: Hàn Quốc là thời lượng cao đáng kể dành cho việc học. Người Pháp dành nhiều thời gian cho việc ăn hơn tất cả các nước còn lại. Người Nauy, trong phần trước vốn có Chỉ Số Hạnh Phúc cao, dành nhiều thời gian cho các sở thích hơn các quốc giá khác.
* Ở đây, ta làm quen với biểu đồ cột chồng. Khác với các biểu đồ thông thường, các cột của chúng có độ cao bằng nhau \(chúng ta đều có một khoản thời gian như nhau\). Nhưng, thành phần phân bổ cho các hạng mục lại khác nhau. Một dạng biểu đồ khác cũng thể hiện sự phân bổ cho các thành phần là biểu đồ tròn. Nhưng, biểu đồ tròn không giúp ta minh hoạ hiệu quả sự so sánh tương quan phân bổ đó trên nhiều nhóm khác nhau. Biểu đồ cột chồng cho phép chúng ta làm điều đó.

### Đàn Ông, Phụ Nữ & Sự Hưởng Thụ

Một trong những khác biệt thường xuyên được quan tâm nhất là khác biệt giữa Đàn Ông và Phụ Nữ. Đàn Ông và Phụ Nữ ai có xu hướng dành nhiều thời gian cho các hoạt động giải trí hưởng thụ hơn?

Dạng biểu đồ rất được "ưa chuộng" cho mục đích so sánh này là biểu đồ cột: Với một cột là nam, một cột nữ, chiều cao của cột là thời gian trung bình cho hoạt động giải trí. Và ta vẽ 146 cặp cột nam-nữ như vậy cho 146 quốc gia.

Ta có một cách xử lý ít "cồng kềnh" hơn.

Hai trục của biểu đồ thường là tương quan của hai giá trị mà ta quan tâm. Ta để thời gian cho giải trí của phụ nữ lên cột dọc, và của đàn ông lên cột ngang.

Ta vẽ một đường chéo đi qua các toạ độ: \(200, 200\), \(250, 250\)... Các điểm nằm trên đường này sẽ có giá trị của phụ nữ = giá trị của đàn ông, nên đây gọi là đường "ngang bằng" \(Gender Parity Line\).

Nếu các chấm, nằm gần đường này, nghĩa là thời gian giải trí của đàn ông và phụ nữ gần như ngang nhau \(Normay, cả nam và nữ xấp xỉ 370 phút một ngày\). Và càng xa đường "ngang bằng" về phía cột ngang \(đàn ông\) thì thời gian giải trí của đàn ông cao hơn hẳn phụ nữ, và ngược lại. Ở các nước \(thường mang tiếng trọng nam khinh nữ\) như Trung Quốc và Ấn Độ, đàn ông dành nhiều thời gian giải trí hơn hẳn phụ nữ. Ở Trung Quốc, đàn ông trung bình dành 250 phút một ngày để giải trí, trong khi phụ nữ trunh bình chỉ có tầm 200-210 phút. Ở Ấn Độ, đàn ông trung bình có 270-280 phút giải trí, trong khi phụ nữ có dưới 250 phút.

![](../../.gitbook/assets/image%20%2850%29.png)

### Niềm vui cuộc sống

Tại sao sự khác biệt trong phân bổ thời gian này lại đáng quan tâm. Vì chúng cho ta biết chất lượng cuộc sống của con người. Chúng ta có những mức độ thoả dụng khác nhau trong từng hoạt động. Lại có một cuộc điều tra của UK Time Use Survey, để hỏi mọi người đánh giá mức độ thoả mãn trong từng hoạt động của họ trên thời gian biểu, trên mức 1-7.

> Kinh Tế Học định nghĩa Lao Động làm hao trừ thoả dụng, còn Nghỉ ngơi, giải trí sẽ làm tăng mức thoả dụng. Vì vậy, ta được trả lương để lao động \(như một cách bù đắp sự hy sinh\), và phải trả tiền để mua các trải nghiệm giải trí.

Biểu đồ bên dưới không khác mấy với định nghĩa của Kinh Tế Học trên và niềm tin của rất nhiều người trong số chúng ta. Những công việc kém "tận hưởng" nhất là làm việc, học tập, làm việc nhà \(trong đó làm bài tập là mệt mỏi nhất\).

Thời gian cho công việc thứ hai là có độ lệch lớn \(khoản tin cậy rộng\), đó bởi có những người làm công việc thứ hai để mưu sinh, có người thì được chọn nó vì "đam mê".

Nhóm các hoạt động vui chơi, giải trí, thư giãn, hưởng thụ sẽ cho mức độ thoả dụng cao nhất.

> Mục tiêu của Kinh Tế Học, cũng như nhiều ngành Xã Hội Học khác là tối đa hoá mức độ thoả dụng \(không phải tiền bạc\) của một người. Nhưng ta có thể dùng tiền mua lấy độ thoả dụng.

![](../../.gitbook/assets/image%20%2851%29.png)

## Thiếu sót của Data

Dọc theo hai bài viết, ở mỗi biểu đồ, người viết có cố gắng đưa ra những khuyến cáo và gợi nhắc về những ngộ nhận có thể xảy ra. Ý thức chuyện này để không bị "lừa" bởi truyền thống, và không mắc lừa chính mình bởi việc nhảy thẳng đến kết luận mà không nhìn ra những thiếu sót của thông tin.

Dọc theo bài viết, tác giả cũng thường xuyên cố gắng để "Hạnh Phúc" trong ngoặc kép \(đoạn nào không bỏ thì có lẽ vì tác giả... quên\).

### Hạnh Phúc có thể đo được không?

Như có đề cập về sự ngây thơ trong cách tiếp cận ngay từ đầu. Bản thân việc đi hỏi thẳng mọi người về Hạnh Phúc có những thiếu sót: Mỗi người có những định nghĩa và chuẩn mực khác nhau về Hạnh Phúc, cũng như đối với chính mỗi người câu trả lời cũng có thể lúc này lúc khác. Nhiều người cũng có thể nói dối. Điều này tạo nên sai lệch giữa Data và Thực Tế.

> Thực tế phức tạp không thể diễn tả trọn vẹn qua Data.

Để cải thiện tính khách quan, ta cũng có thể dùng các yếu tố quan sát được mang tính khách quan hơn thông tin tự khai báo. Các quan sát này cũng có thể phân loại/dán nhãn và dùng như một chỉ số để đo đạc sự Hạnh Phúc:

1. Hay mỉm cười
2. Mỉm cười thành thật \(cười bằng mắt\)
3. Đánh giá qua bạn bè
4. Hay nói các từ khoá lạc quan
5. Chất lượng giấc ngủ
6. Thu nhập

Như bạn có thể thấy, để đo đạc một vấn đề, ta có thể đo đạc các yếu tố có liên quan mật thiết với vấn đề gốc. Dữ liệu và thống kê nhìn chung là ngành khoa học chấp nhận sai số. Bên dưới là biểu đồ thể hiện sự tương quan giữa Chỉ Số Hạnh Phúc và việc thường xuyên cười/mỉm cười.

![](../../.gitbook/assets/image%20%2852%29.png)

### Hạnh phúc = Thoả mãn?

Nhớ lại phần trước, chỉ số Hạnh Phúc Cantril không hỏi về Hạnh Phúc, mà hỏi về Sự Thoả Mãn.

> Hãy tưởng tượng trước mặt bạn là một cái thang, có 10 bậc trên đó: 0 là bậc thấp nhất, 10 là bậc cao nhất. Bậc cao nhất là cuộc sống tuyệt với nhất bạn có thể chạm tới, và bậc thấp nhất là vực thẳm cuộc sống. Hiện tại bạn cảm thấy mình đang ở bậc thứ mấy? — \(Đây còn được gọi là Thang Cantril\)

Bên dưới là biểu đồ tương quan của Hạnh Phúc và Thoả Mãn. Thoả mãn mang tính cơ học hơn, trong khi Hạnh Phúc là phạm trù rộng lớn gồm cảm xúc và tinh thần, trong đó thoả mãn chỉ là một phạm trù của Hạnh Phúc.

Chắc bạn còn nhớ, trong phần trên, ta có bàn về việc: Chỉ số thoả mãn của bậc cha mẹ ta giảm trong 5 năm đầu đời của đứa trẻ, nhưng... không có nghĩa họ hạnh phúc.

### Tracking

Vấn đề tương tự xảy ra với cả các biến định lượng \(như thời gian\), việc "tracking" chính xác và đầy đủ thời lượng trong một ngày của mỗi người là một việc không dễ.

Nhưng với sự ra đời của smart devices và các ứng dụng theo dõi, ta có một lượng data mới, với độ chính xác và độ giàu hơn bất kỳ cuộc khảo sát đắt đỏ nào trước tay.

Lượng Data đó có thể sử dụng bởi chính chúng ta, thông báo cho chúng ta những góc nhìn mới về chính chúng ta.

#### Theo dõi cảm xúc

Với concept tương tự những gì ta đã bàn, nhưng smart device và ứng dụng cho phép cuộc khảo sát về cảm xúc diễn ra mỗi ngày, với mỗi người, trong suốt nhiều năm. Bên dưới là hình ảnh của app Daylio. Các dữ liệu và biểu đồ sẽ cho bạn biết cảm xúc của bạn thay đổi thế nào qua năm tháng, vui vẻ / khó ở vào ngày nào trong tuần, trong tháng. Điều gì thường làm bạn vui?  


![](../../.gitbook/assets/image%20%2862%29.png)

#### Giấc ngủ và những cái trở mình

Đến những thứ vốn từng rất khó tracking, nay cũng cho phép ta đo đếm và có được data. App Sleep Cycle, đo tiếng động \(tiếng ngáy, nói mớ\), đếm số lần bạn trở mình, thời lượng giấc ngủ, cho phép bạn "đánh nhãn" về chất lượng giấc ngủ. Từ đó, dự đoán cái chu kỳ trong giấc ngủ, cho bạn lời khuyên để cải thiện. So sánh tương quan chất lượng giấc ngủ của bạn với bạn bè năm châu.

Tôi sẽ dừng ở đây, và đi đọc lại bài đọc của [**Datatalk\#1 về Big Data**](../1-hello-world/big-data.md#data-tiet-lo-gi-ve-chung-ta).  


![](../../.gitbook/assets/image%20%2858%29.png)

## Recap

* Để đọc và hiểu data, chúng ta có thể đi theo mô hình giải quyết vấn đề của Data PPDAC \(Problem-Plan-Data-Analysis-Conclusion\): Các touch-points sẽ giúp ta nắm được dụng ý, cách tiếp cận, và sai sót có thể có.
* Khi đọc một biểu đồ ta cần chú ý: Tiêu đề, chú thích dưới tiêu đề, chú thích trên các trục, thời gian và mẫu quan sát, các chú thích khác, và nguồn.
* Data là nỗ lực diễn dịch lại thế giới phức tạp. Bản thân data có những sai sót bản chất, khi định lượng và đo lượng các sự kiện và sự vật.
* Công nghệ Smart Devices, Ứng dụng mobile đang cho phép ta giảm sai sót đó.

