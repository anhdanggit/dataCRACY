# DataYourself: Your Spotify Data

### Spotify Data

Trong hoạt động DataYourself của phần này, bạn sẽ tìm hiểu và tương tác với data của chính mình từ Spotify. 

{% hint style="info" %}
**Spotify** là ứng dụng streaming âm nhạc và podcast hàng đầu thế giới với lượng người dùng cực kỳ lớn. Bên cạnh kho nhạc bản quyền khổng lồ với chất lượng cao, tính năng ăn tiền của Spotify là Playlist nhạc thông minh _Daily Mixes_ và _Music Weekly Discovery_. 

Tính năng này là một ứng dụng của **Machine Learning - Recommendation System** \(Thuật toán gợi ý\).
{% endhint %}

![Music Weekly Discovery \(&#x1EE8;ng d&#x1EE5;ng Machine Learning Thu&#x1EAD;t to&#xE1;n G&#x1EE3;i &#xDD;\)](../../.gitbook/assets/image%20%281%29.png)

Thuật toán này được xây dựng dựa trên data của hàng triệu người dùng Spotify. Mỗi tương tác bấm vào các bài hát, nghe bài hát, dừng ở giây nào, add vào playlist, follow các artists hay playlists, tìm kiếm các keywords tạo nên một lượng data khổng lồ về hành vi, khẩu vị âm nhạc của mỗi cá nhân. Và, sự trùng lặp giữa các cá nhân.

Spotify biết bạn đã thích điều và những người tương tự như bạn sẽ thích điều gì, rồi gợi ý những lựa chọn “phù hợp” cho bạn. Chữ “phù hợp” được để trong ngoặc kép, vì một thuật toán gợi ý tốt không thể lúc nào cũng chỉ recommend những bài hợp gout bạn, đôi khi một chút “bất ngờ” lại khiến người dùng thích thú. Quan trọng hơn, thuật toán cần gợi ý thế nào để tối ưu được lợi nhuận cho doanh nghiệp.

Thuật toán gợi ý đem lại nhiều lợi ích cho người dùng, giúp cá nhân hoá và hoàn thiện hơn trải nghiệm. Nhưng, “gợi ý” đôi khi và rất có thể là một bước trong việc thao túng \(manipulate\) quyết định của người dùng. Liệu sống trong một thời đại nhan nhản những “gợi ý” nên xem bộ phim nào, nghe bài nhạc nào, kết đôi với ai, mua món hàng gì, có làm loài người chúng ta mất đi khả năng tự tìm kiếm những lựa chọn và tự đưa ra quyết định mà không cần gợi ý? Xin dành câu hỏi mở này để bạn suy nghĩ và tìm đọc thêm về mặt trái của các thuật toán.

Trong session này, hãy cùng xem Spotify có những data của bạn và tương tác với data của chính bạn.

### Organize Your Music

{% tabs %}
{% tab title="Hoạt Động \#1" %}
Truy cập vào [http://organizeyourmusic.playlistmachinery.com/](http://organizeyourmusic.playlistmachinery.com/#)

* [ ] Login qua portal của Spotify
* [ ] `The Track List` Có các thông tin gì đi kèm một bài hát?
* [ ] `The Plot` tự tìm tòi Spotify data của chính bạn qua interactive 
{% endtab %}
{% endtabs %}

### Gout Nhạc của bạn “Dị” đến đâu?

{% tabs %}
{% tab title="Hoạt Động \#2" %}
Truy cập vào [Obscurify Music](https://obscurifymusic.com/home)

* [ ] Truy cập vào [Obscurify Music](https://obscurifymusic.com/home)
* [ ] Login qua portal của Spotify
* [ ] Check Top `Genres` + `Obscurity`  
* [ ] Check tab `About` của [www.obscurifymusic.](www.obscurifymusic.com)
{% endtab %}

{% tab title="Khái niệm" %}
#### Chúng ta sẽ hiểu con số `80%` như thế nào?

![Gout nh&#x1EA1;c c&#x1EE7;a b&#x1EA1;n &quot;D&#x1ECB;&quot; h&#x1A1;n 80% Vietnamese Users on Obscrify](../../.gitbook/assets/image%20%285%29.png)

* Trên **X-axis \(trục hoành\)**: Điểm số của sự “Dị” - `Obscurity Score` \(tính toán trên lịch sử nghe\). Điểm càng cao thì gout nhạc càng dị, và càng thấp nếu gout nhạc đại chúng
* Trên **Y-axis \(trục tung\)**: Số lượng users trên từng mức điểm
* **Con số 80% hiểu như thế nào?** 
  * `Số user có gout nhạc mainstream hơn tôi (ít “dị” - less obscure)` = `Cộng lại số user trên các cột, ứng với giá trị Obscurity Score (X-axis) < Số Score của bạn (màu xanh)` / `Tổng số VN users có data trên webpage (= 6,132 VN users)` = **`80%`**. 
  * **Ý nghĩa:** 80% tổng số VN users có Obscurity Score &lt; Số Obscurity Score của bạn. 
{% endtab %}

{% tab title="Behind the Scene" %}
#### Behind the : Check 

* Data của bạn được lấy về như thế nào?  \(Spotify’s Web API: Lịch sử nghe, top genres, đặc tính của các bài hát: energetic, danceable, happy, etc.\)
* Thông tin của bạn có được bảo mật không?
* How it work?  \(Login =&gt; Cho phép access vào một phần data: User ID, Country, List of artists & tracks =&gt; Lịch sử nghe\)
* Scoring your taste: 
  * \(1\) Dựa vào các chỉ số đặc tính của bài hát; 
  * \(2\) Dựa vào số bài trong từng genres x Genres có “dị” không \(score cao cho độ ít phổ biến - Số lượt nghe của tất cả người dùng website có\)  =&gt; Score = số bài thuộc genres A x “Dị” Score của genres A  =&gt; So sánh bạn với những người dùng khác
* Nếu là bạn, bạn sẽ đo độ “Dị” \(`Obscurity Score` như thế nào\)
{% endtab %}

{% tab title="Bảo vệ Data Cá nhân" %}
#### Data Privacy: 

* [ ] Trên góc phải, mục `Menu`, Click `Remove Obscurify Account`: Bạn sẽ được dẫn tới website chính thức của Spotify. Tại đây Spotify sẽ list tất cả những website/apps đang có access vào data Spotify của bạn
* [ ] Trong trang `Spotify Accounts`, bạn có thể chọn mục `Privacy Settings` 

#### Manage Your Data

{% hint style="info" %}
Spotify đang connect với những thông tin cá nhân nào khác của bạn ngoài Spotify \(Facebook, thông tin để quảng cáo “target” bạn\)
{% endhint %}

![](../../.gitbook/assets/image%20%284%29.png)

#### Download Your 

Ở một số quốc gia, theo quyền bảo mật Data riêng tư, bạn có quyền đòi hỏi bất kỳ doanh nghiệp nào trả cho bạn bảng copy toàn bộ data họ có từ bạn. Đây cũng là cách để biết họ đang track những data nào của bạn. 

Bạn có thể “request” và Spotify trả data cá nhân của bạn trong vòng 30 ngày từ ngày \(Facebook, Instagram, tương tự của có các chính sách này\)   
=&gt; Hãy thử để xem các Apps có thật sự thực thi chính sách data không? Nhiều khi họ chỉ để cho có “hình thức” theo quy định của pháp luật và nghĩ rằng sẽ không có mấy users thật sự quan tâm đến bảo mật và quyền data. Mình đã thử request từ ngày 5 tháng 10 và đến ngày 11 tháng 12 \(hơn 60 ngày sau đó\) vẫn thấy Spotify im hơi lặng tiếng \(Spam checked!\). Nếu bạn như mình đòi hoài không thấy trả data, và bạn đủ rảnh, bạn hoàn toàn có thể khởi kiện Spotify. 

Trên thế giới, có nhiều social activists và tổ chức độc lập được thành lập nhằm mục đích “điều tra” các trường hợp tương tự. Cho nên chúng ta có thể cùng nhau điều tra, bạn có thể thử `Download Your Data` và nếu bạn được trả data hãy báo cho chúng .
{% endtab %}

{% tab title="Data Sceptic" %}
**Data Fallacy: Có gì "kỳ lạ" trong chart sau?**

_Hint: Chú ý đến tên X-axis, Y-axis. Và "concept" của Obscurity Score._

![](../../.gitbook/assets/image%20%285%29%20%281%29.png)
{% endtab %}
{% endtabs %}

