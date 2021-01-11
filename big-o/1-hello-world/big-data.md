---
description: Vì sao Big Data trở thành "màu sắc" của thời đại?
---

# Big Data

Trước khi đến với Big Data, thế nào là Data?

Như ở phần trước về Thuật Toán, sở dĩ Thuật Toán, AI/ML trở nên quyền lực đến mức chi phối và thao túng cách chúng ta sống là bởi chúng trở nên vô cùng tinh vi nhờ lượng Data khổng lồ được dùng để "train" chúng.

Lượng Data khủng đó từ đâu ra?

> Internet-of-Things \(IoT\) → Big Data → Thuật toán, AI/ML

Mỗi chúng ta là một phần tạo lên nó.

## Data trông như thế nào?

Dù đã dốc công tham khảo nhiều sách vở, vẫn không tìm được một định nghĩa thật dễ hiệu cho các bạn. Định nghĩa bên dưới kết hợp bởi "Data" trong từ điển Cambridge và ý kiến chủ quan của người viết:

> **Data \(Dữ liệu\):** Các quan sát, thường dưới dạng sự kiện hoặc số liệu, được lưu trữ nhằm mục đích kiểm tra, tham khảo và phục vụ cho mục đích ra quyết định.

Cho phép tôi bắt đầu nói về Data ở dạng quen thuộc nhất với tất cả chúng ta: **Số và Bảng.** Đó là cách tự nhiên nhất chúng ta thường tương tác với Data, trên: Google Sheet, Sao kê ngân hàng, hay báo cáo thu chi tài chính.

Theo đó, Data quen thuộc với chúng ta, với: **Cột và Dòng.**

Như bên dưới:

* Mỗi dòng là một người
* Mỗi cột là "thuộc tính" gắn với mỗi người: Tên, Thành Phố, Địa chỉ.

![](../../.gitbook/assets/image%20%2830%29.png)

Bảng sau là các bài hát nhạc Pop trên Spotify \(Bạn có thể khám phá trong phần Data Yourself\):

* Mỗi dòng là một bài hát
* Mỗi cột là một "thuộc tính" của bài hát: Ca sĩ, năm phát hành, bpm, engergy, danceability, live, acousticness, popularity

![](../../.gitbook/assets/image%20%2827%29.png)

Để tóm lại, bạn có thể hình dung data là một bảng chữ nhật có:

* **Chiều Dọc \(n\):** Số dòng \(hay số quan sát, số ví dụ, số users\)
* **Chiều Ngang \(p\):** Số tính chất \(features\) được ghi nhận‌

![](../../.gitbook/assets/image%20%2831%29.png)

## Big Data

> Chúng ta được định hình, định tính bằng những con số: Số bạn bè trên mạng xã hội, số likes, số tiền trong tài khoản, số lần cà thẻ, số lượt dịch chuyển trong thành phố. Mỗi tin nhắn của ta có bao nhiêu từ, ta kết thúc bằng dấu chấm hay ba chấm. Mỗi cuộc gọi bao nhiêu phút. Trong một ngày, ta cầm điện thoại lên bao nhiêu lần, mỗi lần bao nhiêu giây, vào buổi sáng hay chiều, trưa hay là tối. Mất bao lâu ta uống hết một chai sữa 1.5 lít, mất bao lâu ta lại phải đặt văn phòng phẩm. Ta đang ngắm nghía tìm kiếm, muốn mua cái áo nào, cái điện thoại nào, chai sữa rửa mặt nào. Bao nhiêu bước chân ban ngày, bao nhiêu calorie tiêu thụ mỗi bữa ăn, bao nhiêu lượt trở mình ban đêm. Cô bất giác liếc nhìn cái smartwatch trên tay, trên đó nhấp nháy hiện lên 8,725 bước cô đã đi trong ngày, 108 nhịp tim cô đập trong một phút, đêm qua cô ngủ không ngon giấc. — Đặng Huỳnh Mai Anh \(2020\). Truyện ngắn "Học Máy"

Big Data là hình chữ nhật `n x p` đó được phóng dãn theo chiều dọc \(**Big "n": nhiều cá thể được quan sát hơn\)** hay theo chiều ngang **\(Big "p": nhiều tính chất được quan sát hơn\).**

Ở nhiều thập kỷ trước, bộ Data khủng nhất là dữ liệu scanner bán hàng trong siêu thị. Để rồi trong những năm gần đây, với sự bùng nổ của Internet:

* Có thể "track" được data của hàng tỷ người trên thế giới ⇒ **Big "n"**
* Mỗi người dùng Internet lại tạo ra lượng data khổng lồ trong mỗi lần đăng nhập, mỗi cái nhấn chuột. Nhờ smartphone, nhiều thể loại data chưa từng thu thập được nay lại trở nên thông dụng: Hình ảnh \(camera/webcam\), Audio \(microphone\), Text \(Mạng Xã Hội\) ⇒ **Big "p"**
* Siêu máy tính \(GPU, TPU\) và công nghệ mới cho phép chúng ta xử lý và lưu trữ một lượng dữ liệu lớn

## Text, Âm thanh, Hình Ảnh

{% hint style="success" %}
1. Trò chuyện một đôi chút với các văn hào nổi tiếng: [LINK](https://experiments.withgoogle.com/talk-to-books)   
2. Kết hợp Hình Ảnh, Text, Âm Thanh: [LINK](https://experiments.withgoogle.com/giorgio-cam)
{% endhint %}

Cả hai ứng dụng AI trên đều dựa trên những dạng data không phải dạng quen thuộc với chúng ta: Không phải **Số**.

Chúng ta cũng thường nghe về "Kỹ thuật số", thời kỳ "Công nghệ số" \(Digital\). Nói cho đơn giản, kỹ thuật số giúp chúng ta chuyển đổi nhiều thứ \(hình ảnh, âm thanh, ký tự\) về dạng số và bảng số \(n x p như trong bảng Excel. Đây là một ý tưởng cốt lõi\).

> Tư duy căn bản của Toán học là: Khi vũ trụ quăng cho bạn một vấn đề quá phức tạp, hãy tìm cách giải quyết một vấn đề khác đơn giản hơn, rồi biến hoá sao cho cái “phiên bản” đơn giản hơn đó gần nhất có thể với “phiên bản” gốc của vũ trụ.

Liên tiếp trong cái ví dụ sau về Data: Hình Ảnh, Âm Thanh, Text và chữ viết. Mục đích cuối cùng là đưa chúng về dạng Số và Bảng \(mà ta đều quen thuộc\).

### Hình Ảnh

Trong ví dụ bên dưới, hình ảnh Sao Kim được số hoá, thành một bảng số liệu có dòng và cột như ta quen thuộc.

**Digitalize** \(Số hoá\) như sau:

* Ảnh hai chiều được chia thành các pixel
* Ở đây trong từng pixel là giá trị của grayscale vùng diện tích bên trong pixel đó

Con người nhìn hình ảnh như bức ảnh trên-cùng-bên-trái, còn Máy nhìn như ma trận số dười-cùng-bên-phải.

![](../../.gitbook/assets/image%20%283%29.png)

Còn màu sắc thì sao?

Các màu sắc ta thấy là sự chồng lên nhau của ba lớp màu Đỏ - Xánh Lá - Xanh Dương \(RGB: Red-Green-Blue\). Với kỹ thuật chia pixel tương tự như trên, ta có được các lớp màu và chồng lên nhau thành hình ảnh quan sát được và màu sắc.

![](../../.gitbook/assets/image%20%2828%29.png)

### Âm Thanh

Tương tự cũng có những kỹ thuật để biết sống âm thành Số, như bên dưới: Đo bước sóng và cao độ. Kết hợp nhiều bước chuyển đổi phức tạp, có thể có được bảng số như Spotify, mỗi bài hát được đính với các số đo đạc: `Acousticness`, `Popularity`, `Danceablity` \(Mỗi thông số có thể lấy input từ các thông tin khác nhau của sóng âm, ví dụ bước sóng ngắn - cao độ cao thì sẽ có Energy bài hát lớn hơn\).   


![](../../.gitbook/assets/image%20%282%29.png)

![B&#xE0;i h&#xE1;t c&#x1EE7;a Chi Pu v&#x1EDB;i c&#xE1;c th&#xF4;ng s&#x1ED1;](../../.gitbook/assets/image%20%2840%29.png)

### Text

{% tabs %}
{% tab title="Hoạt Động \#1" %}
Truy cập: [https://databasic.io/en/wordcounter](https://databasic.io/en/wordcounter)

* [ ] Input một đoạn text có chủ đề bạn quan tâm \(lyrics, news, wikipedia\)
* [ ] Bạn thấy gì từ kết quả?
* [ ] Bạn có thể download file CSV và phân tích thêm trên google 
{% endtab %}

{% tab title="Chú Giải" %}
* **Bigrams:** Cụm text 2 chữ
* **Stopwords:** hững từ sẽ "ignore" trong text analysis, ví dụ "this", "that", "and", "but"
* **Trigrams:** Cụm text 3 chữ
* **Word Cloud:** Dạng minh hoạ với các từ, độ to nhỏ của từ phụ thuộc tần suất xuất 
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Hoạt Động \#2" %}
Truy cập: [https://databasic.io/en/samediff](https://databasic.io/en/samediff)

* [ ] Bạn thấy gì từ kết quả?
{% endtab %}

{% tab title="Chú Giải" %}
* Từ kết quả của word counts, mỗi bài hát ta đếm được Top 10 từ, và cụm ký tự \(Bigrams, Trigrams\). Một cách đơn giản và "ngây thơ" để đo xem 2 lời bài hát có giống nhau trong số lần lặp lại của các từ và số ký tự. Nói cách khác, phương pháp trong WordCount đã tạo ra input cho Thuật Toán này \(So Sánh\)

![](../../.gitbook/assets/image%20%2825%29.png)
{% endtab %}
{% endtabs %}

* **Word Clouds** là cách biểu diễn data, để xem từ/chuỗi ký tự nào xuất hiện nhiều nhất \(Càng từ/chuỗi ký tự xuất hiện càng thường xuyên sẽ có kích thước càng to\): Số từ thường xuyên xuất hiện trong bài hát của riêng Beyonce, của riêng Aretha Franklin, và các từ thường giống nhau \(`Love` và `Baby` có vẻ là từ lặp lại nhiều nhất, khiến thuật toán này nhận định Lời của Beyonce và Franklin giống nhau đến 0.84 điểm.

![](../../.gitbook/assets/image%20%286%29.png)

{% hint style="info" %}
Các kỹ thuật số hoá là ý tưởng nền tảng cho Thời Đại Số, cho việc thêm nhiều "features" \(Big "p"\) tạo nên Big Data. Từ đó, tạo nên những Thuật Toán khủng phác hoạ, mô phỏng hành vi con người.
{% endhint %}

## Data tiết lộ gì về chúng ta

> “Tiền bạc. Quan hệ. Và, sự cô độc”.   
> “Phải. Là ba thứ”.   
> _Lịch sử giao dịch. Lịch sử điện thoại. Và, tương tác mạng xã hội. — Đặng Huỳnh Mai Anh \(2020\). Truyện ngắn "Học Máy"_

Trong Kinh Tế Học - Hành Vi, xu hướng của con người là tập trung vào cái ngắn hạn và không ý thức về kết cuộc dài hạn trong một quyết định, hành động, một cuộc đổi chác.

Người dùng luôn tập trung vào cái lợi trước mặt của sự tiện lợi \(Internet cho tôi đúng cái tôi đang cần\), cho số điện thoại để được tích điểm, share thông tin để sử dụng cái ứng dụng miễn phí. Chúng ta đều ít nhiều, một lần hay nhiều lần bị "mua" bởi cái giá rẻ mạt.

> “Chân dung của chúng ta, trong thời đại này, chỉ là những con số. Cô không đồng ý sao?”   
> “Nhưng chúng ta có thể làm gì hơn?”   
> Nên nhớ là chúng ta cho họ tất cả những thông tin đó, đổi lại những tiện ích miễn phí. Khi chúng ta đón nhận những thứ miễn phí, tự chúng ta sẽ biến mình thành hàng hoá. Mỗi ứng dụng tải về đều là một bản hợp đồng, ta ký bằng một cái nhấn nút. Ấy nghĩa là ta cho phép họ truy cập vào toàn bộ dữ liệu về mình. Tự nhìn lại xem, chúng ta có bao nhiêu lần đọc kỹ những điều khoản, để ý xem những thông tin nào của chính chúng ta đang bị rò rỉ. — Đặng Huỳnh Mai Anh \(2020\). Truyện ngắn "Học Máy"

Cách đây nhiều năm, mẹ tôi hí hửng cầm về nhà chiếc thẻ khách hàng thân thiết của CoopMart. Từ đó, mỗi lần mua gì, bà đều cầm theo chiếc thẻ nhựa màu xanh đó, scan hết giỏ hàng, sẽ scan chiếc thẻ tích điểm. Đến cuối năm, có thể đổi điểm và voucher mua hàng.

Trong một vùng trời khác của Địa Cầu, nhiều năm về trước - 1993, Tesco chuỗi siêu thị của Anh cũng giới thiệu chiếc thẻ tương tự: **ClubCard**. Chiếc thẻ đó đem lại cho Tesco nhiều thông tin hơn về khách hàng. Sau báo cáo từ ClubCard, chủ tịch hội đồng quản tri thốt lên: "Đáng sợ. Những gì ta biết được sau 3 tháng này còn nhiều hơn những hiểu biết của tôi về khách hàng của chúng ta trong 30 năm".

Nhờ thông tin đó, thói quen mua sắm của khách hàng trở nên dễ nắm bắt và "định hướng" hơn.

### Tính Riêng Tư và Nhạy Cảm

Trong những ngày đầu tiên giới thiệu online shopping, Tesco có một tính năng **"My Favourites"** đơn giản: Đưa lên "top" những sản phẩm mà khách hàng thường mua \(và được ghi nhận bằng thẻ Clubcard\). Một người phụ nữ liên hệ với Tesco, phàn nàn rằng data có vẻ bị sai. Vì cô thấy "condom" trong mục "My Favourites" của cổ, dù cô và chồng hoàn toàn không dùng "condom". Nhân viên Tesco kiểm tra lại cơ sở dữ liệu của họ, thấy không hề sai. Nhưng không lẽ bóng gió rằng chồng cô ngoại tình đó cô ơi. Họ chọn cách giải quyết "thảo mai & dĩ hoà vi quí" rằng data bị sai - chúng tôi vô cùng xin lỗi. 

Có những dữ liệu tưởng vô thưởng vô phạt mà lại đầy riêng tư và nhạy cảm. Lịch sử mua sắm và giao dịch không chỉ để kiểm kê bạn tiêu xài cái gì. Chúng có thể nói lên bạn là ai? Một cách không mong muốn.

### Hiểu bạn hơn cả chính bạn

Cho phép tôi được tiếp tục câu chuyện về Tesco và dữ liệu mua sắm của họ.

Họ thực hiện một chiến dich Target marketing. Tesco nhận ra những khách hàng sắp làm mẹ là đối tượng cực kỳ tiềm năng. Dựa vào lịch sử mua sắm của rất nhiều khách hàng, Tesco có thể suy ra khách hàng nào vừa trở thành mẹ: Họ sẽ mua đồ đạc, sữa, tã, quần áo cho trẻ em. Dịch góc nhìn vào thời điểm 8-9 tháng trước, họ thường mua những gì: Que thử thai, các loại thuốc và thực phẩm chất năng cho giai đoạn đầu thai nghén. Với các thông tin đó, có thể xây dựng một thuật toán tiên đoán được khách hàng nào đang bước vào thai kỳ, rồi gửi brochure, voucher, quảng cáo cho họ về các sản phẩm cho phụ nữ đang mang thai, rồi hưởng luôn nguồn tiền của việc mua sắm về sau: Nuôi dưỡng một đứa nhỏ là công cuộc dài lâu và tốn kém.

Khi thuật toán đó đi vào sử dụng, một ông bố có cô con gái tuổi teen đùng đùng lao tới cửa hàng Tesco gần nhất khiếu nại, rằng con gái ông nhận được voucher, coupon cho phụ nữ mang thai.

Vài tháng sau, trên New York Times, người bố phải xin lỗi vì con gái ông thật sự có thai.

Đáng sợ phải không bạn?  
Khi một thuật toán có thể hiểu đứa con hơn cả cha mẹ của họ.

Các thuật toán tương tự: Để dự đoán ai đang có thai, ai đang cần hẹn hò, ai đang dòm ngó mẫu smartphone mới ra - Ngày nay chúng ở khắp nơi trên mạng xã hội, chầu trực quanh ta.

{% hint style="info" %}
**Thuật toán có thể thao túng bạn nhiều hơn bạn nghĩ**  
Khả năng thao túng đó lại càng kinh khủng hơn với lượng data nhận được. Một số vấn đề để suy ngẫm:   
1. Hệ thống điểm xã hội \(Trung Quốc\)   
2. Cambrige Analytica: Dùng dữ liệu likes & dislikes để dự đoán các tuýp tính cách, dùng đó để "target" và thay đổi quan điểm của cử tri, từ đó thay đổi kết quả bầu cử.   
_Đọc thêm:_ [_Học Máy_](truyen-ngan-hoc-may.md)\_\_
{% endhint %}

## Bảo vệ Dữ Liệu Cá Nhân

{% hint style="danger" %}
**Có 03 điều tạo nên sự đáng sợ của Data & Thuật toán:**

1. Lượng thông tin khổng lồ mà từ đó nhiều thuật toán được xây dựng để hiểu về bạn, tiên đoán về bạn, gợi ý cho bạn, và thao túng bạn.
2. ID chung \(Advertising ID\) trên tất cả các apps và webs để xâu chuỗi lại toàn bộ bức tranh về một người dùng
3. Không có luật và quyền về giới hạn của việc khai thác và kết hợp/trao đổi/buôn bán data 
{% endhint %}

Trong phần này chúng tôi dẫn chứng nhiều luật **Bảo Vệ Thông Tin của EU \(GDPR\)**, nhưng luật thông tin của nhiều nước trên thế giới bao gồm Việt Nam cũng đi theo các điểm tương tự. Chúng tôi chọn đề cập đến GDPR làm góc vì nhiều ứng dụng và websites hiện nay được thiết kế theo chuẩn này.

## Thông tin cá nhân là gì?

> EU GDPR \(General Data Protection Regulation\) định nghĩa thông tin cá nhân là tất cả thông tin liên quan đến một người có thể trực tiếp hoặc gián tiếp định danh người đó.

![](../../.gitbook/assets/image%20%2838%29.png)

### Đào Data & Buôn Data

> Khi bạn dùng một sản phẩm miễn phí, chính bạn sẽ trở thành sản phẩm.

Trong rất nhiều tài liệu cũ về các chiến lược Data \(cũ ở đây nghĩa là trước [GDPR](https://vi.wikipedia.org/wiki/Quy_%C4%91%E1%BB%8Bnh_b%E1%BA%A3o_v%E1%BB%87_d%E1%BB%AF_li%E1%BB%87u_chung)\), có một mục **Data "monetization"** - Nghĩa là "làm tiền" / tạo ra lợi nhuận từ data, thường bằng cách bán data cho một bên khác.

Thỉnh thoảng, nếu bạn nhận được một cuộc gọi từ một công ty bất động sản, bảo hiểm hay dịch vụ mà bạn chưa từng mảy may hay biết, thì nghĩa là... bạn \(data của bạn\) đã bị bán. Mỗi lần bạn để lại số điện thoại để tích điểm thưởng, liên hệ với bên trung gian rằng bạn đang cần kiếm nhà/xe và để lại thông tin liên lạc - Rất có thể những thông tin đó sẽ được bán cho một bên khác.

Lịch sử liên lạc điện thoại, lịch sử giao dịch, lịch sử ngân hàng - Có vô số các bên thèm khá để có những thông tin đó.

Nếu không phải bạn chủ động cung cấp, vẫn có những tay đào data từ mạng xã hội - Facebook, Instagram, Linkedln. Họ có những kỹ thuật để "nối-chéo" data từ nhiều nguồn, xác định bạn là ai và tạo nên một hồ sơ hoàn chỉnh về bạn, thông qua những dấu vết Internet.

### Advertising ID

{% hint style="info" %}
**Bạn có bao giờ tự hỏi vì sao những ads ta xem ở apps trước lại theo ta sang apps sau, hoặc một key words ta search trên trang nay ngay sau đó xuất hiện trên một apps khác?** 

Mỗi chiếc thiết bị di động trong tay ta, có một số Advertising ID. Như tên gọi, ngành Quảng Cáo mạng \(đặc biệt là Personalized Marketing\) xoay quanh số ID này - Một chuỗi số cho phép các dịch vụ và ứng dụng xác định hành vi của người dùng: Trên iOS là **IDFA** \(Apple’s Identifier for Advertisers\), trên Android là **GAID** \(Google Advertising ID\). Số ID này gán cố định cho một thiết bị trên tất cả các apps, vì vậy bằng Advertising ID có thể map lại toàn bộ hành trình, lịch sử tương tác của chúng ta trên thiết bị đó. Nhờ vậy, có thể xác định được hành vi người dùng để quảng cáo một cách hiệu quả.
{% endhint %}

1. Số IDFA được để mặc định như luật bất thành văn của hệ thống Quảng Cáo mạng. Người dùng có thể tắt theo dõi **IDFA** trong mục **setting Privacy** của iPhone \(tầm &lt;5% users tắt tracking IDFA\)
2. Đến tháng 9/2020, iOS14 quyết định chuyển IDFA từ `mặc-định-trong-lặng-lẽ` thành `thông-báo-công-khai` với users rằng họ đang bị "theo dõi" trên tất cả các apps và websites, nhằm mục đích quảng cáo \(Thông tin không được "thân thiện" mấy như bên dưới\) ⇒ Đó là cú "hit" cho toàn ngành Quảng cáo, sau upgrade lên iOS14, 50% users không còn tracking IDFA.

![](../../.gitbook/assets/image%20%2839%29.png)

### Ý thức tự bảo vệ mình

> “Chân dung của chúng ta, trong thời đại này, chỉ là những con số. Cô không đồng ý sao?” “Nhưng chúng ta có thể làm gì hơn?” Nên nhớ là chúng ta cho họ tất cả những thông tin đó, đổi lại những tiện ích miễn phí. Khi chúng ta đón nhận những thứ miễn phí, tự chúng ta sẽ biến mình thành hàng hoá. Mỗi ứng dụng tải về đều là một bản hợp đồng, ta ký bằng một cái nhấn nút. Ấy nghĩa là ta cho phép họ truy cập vào toàn bộ dữ liệu về mình. Tự nhìn lại xem, chúng ta có bao nhiêu lần đọc kỹ những điều khoản, để ý xem những thông tin nào của chính chúng ta đang bị rò rỉ. — Đặng Huỳnh Mai Anh \(2020\). Truyện ngắn "Học Máy"

Sẽ có rất nhiều thứ đê nói về quyền của người dùng và việc bảo vệ thông tin cá nhân, **DATAracy** muốn tập trung vào 2 điểm:

1. Bảo vệ thông tin cá nhân bằng: Ý thức về các chế độ trong setting Privacy trên các thiết bị và ứng dụng Internet. [DataYourself: Spotify & Private Settings](d-aty-spotify-data.md)
2. Ý thức về các quyền và luật đang tồn tại để bảo vệ thông tin người dùng

### Luật Công Nghệ Thông Tin Việt 

Việt Nam: **Khoản 1 Điều 21, Luật CNTT** \(Công Nghê Thông Tin\): 

> “thu thập, xử lý và sử dụng TTCN của người khác trên môi trường mạng phải được người đó đồng ý trừ trường hợp pháp luật có quy định khác”

1. Thông báo cho người đó biết về hình thức, phạm vi, địa điểm và mục đích của việc thu thập, xử lý và sử dụng TTCN của người đó
2. Sử dụng đúng mục đích TTCN thu thập được
3. Chỉ lưu trữ những thông tin đó trong một khoảng thời gian nhất định theo quy định của pháp luật hoặc theo thoả thuận giữa hai bên
4. Tiến hành các biện pháp quản lý, kỹ thuật cần thiết để bảo đảm TTCN không bị mất, đánh cắp, tiết lộ, thay đổi hoặc phá huỷ
5. Tiến hành ngay các biện pháp cần thiết khi nhận được yêu cầu kiểm tra lại, đính chính hoặc hủy bỏ theo quy định tại khoản 1 Điều 22 của Luật này; không được cung cấp hoặc sử dụng TTCN liên quan cho đến khi thông tin đó được đính chính lại”

### GDPR Infor

Các điều khoản của GDPR có thể tóm gọn lại, rằng mỗi doanh nghiệp lưu trữ thông tin khách hàng phải trả lời được các câu hỏi sau:  


![](../../.gitbook/assets/image%20%2836%29.png)

![](../../.gitbook/assets/image%20%2835%29.png)

## Recap

* Sở dĩ **Thuật Toán, AI/ML** trở nên quyền luật đến mức chi phối và thao túng cách chúng ta sống là bởi chúng trở nên vô cùng tinh vi nhờ lượng **Data khổng lồ** được dùng để "train" chúng.
* **Data \(Dữ liệu\):** Các quan sát, thường dưới dạng sự kiện hoặc số liệu, được lưu trữ nhằm mục đích kiểm tra, tham khảo và phục vụ cho mục đích ra quyết định.
  * **Chiều Dọc \(n\):** Số dòng \(hay số quan sát, số ví dụ, số users\)
  * **Chiều Ngang \(p\):** Số tính chất \(features\) được ghi nhận‌
  * Big Data là "hình chữ nhật" n x p đó được phóng dãn theo chiều dọc \(**Big "n": nhiều cá thể được quan sát hơn\)** hay theo chiều ngang **\(Big "p": nhiều tính chất được quan sát hơn\)**
  * Chúng ta cũng thường nghe về "Kỹ thuật số", thời kỳ "Công nghệ số" \(Digital\). Nói cho đơn giản, kỹ thuật số giúp chúng ta chuyển đổi nhiều thứ \(hình ảnh, âm thanh, ký tự\) về dạng số và bảng số \(n x p như trong bảng Excel. Bảng sẽ thấy đây là một ý tưởng cốt lõi\)
* Người dùng luôn tập trung vào cái lợi trước mặt của sự tiện lợi \(Internet cho tôi những quảng cáo đúng cái tôi đang cần\), cho số điện thoại để được tích điểm, share thông tin để sử dụng cái ứng dụng miễn phí. Chúng ta đều ít nhiều, một lần hay nhiều lần bị "mua" bởi cái giá rẻ mạt.
* Chúng ta cần ý thức về: Tính Riêng Tư & Nhạy cảm của Data, và khả năng thao túng của Thuật Toán.

