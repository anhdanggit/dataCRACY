# Datatalk\#3 - Data Thinking

![](../../.gitbook/assets/image%20%2866%29.png)

## Dẫn nhập

> Đừng bao giờ tin vào những ấn tượng khái quát, anh bạn ạ, hãy tập trung vào chi tiết — Sherlock Holmes.

Xin được phép bắt đầu phần này bằng một câu của Holmes. Lý do câu này được trích dẫn ở đây, vì nó có vẻ là tóm gọn cho kiểu suy luận **Diễn Dịch** _\(Deduction Reasoning\)_, tịnh tiến logic từ một tiền đề khái quát đến một kết luận trong một tình huống cụ thể. Suy luận từ Data lại đi theo chiều ngược lại, **Quy Nạp** \(_Inductive Reasoning_\), từ những tình huống cụ thể "lội ngược dòng" tạo thành nên một quy luật khái quát.

Đó có lẽ chính là cái khó nhất, trừu tượng nhất, và mông lung nhất của việc **Suy Luận bằng Data**.

Trong **Datatalk\#2**, chúng ta đã từng đề cập đến một lối diễn đạt gây ngộ nhận của không ít báo chí truyền thông rằng: 90% người Việt Nam trong cuộc khảo sát trả lời họ cảm thấy hạnh phúc ⇒ 10% không cảm thấy hạnh phúc + Dân số Việt Nam là 96 triệu người ⇒ 9.6 triệu người dân Việt Nam không hạnh phúc.

Cũng trong chính buổi Datatalk\#2, có bạn đã hỏi: Với những kết quả như vậy có phải là chúng ta đi hỏi tất cả người dân Việt Nam, hay người dân trên thế giới không?

Đó là một nhiệm vụ bất khả thi. Thực tế, càng nghiên cứu và khảo sát chỉ làm trên một mẫu nhỏ. Vậy thì, câu hỏi tiếp theo là: _Làm thế nào ta biết được những kết quả ta quan sát được trong một mẫu có tính phổ quát cho một nhóm dân số lớn hơn?_

Rồi nhìn theo một chiều khác: _Làm sao có thể tổng hợp những thứ ta quan sát ở thời điểm hiện đại và tiên đoán lên tương lai?_

Trong hai câu hỏi trên, ta đã đi từ mô tả đến dự đoán, và đỉnh cao nhất của Dữ liệu và Thống kê: Làm sao để biết điều gì dẫn đến điều gì? Nếu ta trả lời được câu hỏi nếu-thì, ta có thể từ đó thay đổi "nếu" để có "thì", thay đổi nguyên nhân để thay đổi kết quả. Không rõ là đáng mừng hay đáng buồn \(hoặc có lẽ là sự an ủi\), **Ngoại Suy Nhân Quả** \(_Causal Inference_\) vẫn là "chén thánh" kể cả trong thời đại của Big Data.

> Data chả hiểu gì về nhân quả; con người thì có. — Judea Pearl, The Book of Why: The New Science of Cause & Effect

Nội dung của **Datatalk\#3**, muốn nói về việc làm sao tổng quát được những quan sát trong Data thành quy luật, bao gồm: Phóng chiếu giữa mẫu và tổng thể, tiên đoán tương lai từ quan sát trong hiện tại, quy nạp về nhân quá từ quan sát về tương quan.

Đó cũng là quá trình biến dữ liệu, thành thông tin, rồi thành hiểu biết, và sau đó là kiến thức.

## Datatalk\#3 - Agenda

{% hint style="info" %}
## Datatalk\#3 - Data Thinking

1. Trước **Datatalk\#3**, Người Tham Gia được khuyến khích đọc trước tài liệu \(Sẽ gửi ra trước ngày tổ chức\)
2. Trong **Datatalk\#3**, buổi workshop sẽ trao đổi và thảo luận dựa trên nội dung của các bài đọc:
   * [Quy trình _Ngoại Suy Quy Nạp \(Inductive Inference\)_ trong Data](data-thinking-quy-nap.md)
   * [Xác suất & Giả-thuyết-không](xac-suat-and-gia-thuyet-khong.md)
   * [Tương quan & Nhân-Quả](tuong-quan-and-nhan-qua.md)
3. **Datatalk\#3**, sẽ kết hợp: \(1\) Trao đổi/hỏi đáp giữa người tham gia - khách mời; \(2\) Các hoạt động Tương tác + DataYourself
4. Sau **Datatalk\#3**, Người Tham Gia được khuyến khích tiếp khám phá & thực hành \(theo hướng dẫn\):
   * Chia sẻ quan điểm và giúp lan truyền thông điệp của dự án với hashtag  `#DATACracy` `#BigO_Datatalk` \#DataLiteracy
   * Theo dõi và đọc các nội dung tiếp theo của **DATACracy**
{% endhint %}

## Nguồn tham khảo

1. Timo Elliott \(2018\). [Predictive is the Next Step in Analytics Maturity? It's More Complicated Than That.](https://timoelliott.com/blog/2018/04/predictive-is-the-next-step-in-analytics-maturity-its-more-complicated-than-that.html)
2. Judea Pearl & Dana Mackenzie \(2018\). The Book of Why: The New Science of Cause and Effect.
3. David Spielgelharter. The Art of Statistics: Learning from Data.

