# CSS

- CSS viết tắt của từ Cascading Style Sheets, được dùng để trang trí, định dạng, bố cục cho trang web, không có ý 
  nghĩa trong việc thể hiện nội dung.
- CSS là một file có phần mở rộng là .css, nhiệm vụ của nó là tách riêng phần định dạng (style) ra khỏi nội dung trang HTML.

# Cú pháp CSS

  CSS được tạo thành từ các Style Rule. Các rule này được thông dịch bởi trình duyệt và sau đó được áp dụng tới các phần tử tương ứng trong tài liệu của bạn. Style Rule bao gồm ba phần:

  **Selector: (hiểu nôm na là bộ chọn phần tử)** Một selector là một thẻ HTML mà tại đó một bạn áp dụng một style cho nó. Đó có thể là bất kỳ một thẻ HTML nào, như thẻ div, thẻ span, thẻ p, …

  **Property: (thuộc tính)** Là property của một kiểu thuộc tính của thẻ HTML. Nói một cách đơn giản thì tất cả các thuộc tính trong HTML được chuyển đổi thành các CSS property. Đó có thể là color, border....

  **Value**: Là các giá trị được gán cho các property. Ví dụ, color có thể có các giá trị là red #F1F1F1 etc.
  Dưới đây là cú pháp CSS chung:

     selector { property: value } hoặc selector { property: value; property2: value2; }

  Mỗi khối khai báo này bao gồm một tên của CSS property và một giá trị được gán cho property đó.
  Bạn cần chú ý một điều rằng, một khai báo CSS luôn luôn kết thúc với một dấu chấm phảy và phần khai báo này sẽ được bao quanh bởi cặp dấu ngoặc ôm.

## Các loại Selector trong CSS

### Bộ chọn theo tên id

 **tag#tênid { thuộc tính: giá trị; }**

  - Bắt buộc phải có ký tự dấu "#" và tênid
        div#content { width: 600px; }

### Bộ chọn theo tên class

 **tag.tênclass { thuộc tính: giá trị; }**

- Bắt buộc phải có ký tự dấu "." và tênclass
        div.navi { background: #333333; }

### Bộ chọn theo cấp bậc

 **[tag cha] [tag con] [tag cháu] { thuộc tính: giá trị; }**

 - Cấu trúc này không bắt buộc, tuy nhiên cấu trúc này sẽ thuận tiện trong việc điều chỉnh các thành phần con bên trong, và cũng để 
    xác định thứ tự ưu tiên trong CSS.
- Trong file HTML bên trên, trong phần content và navi đều có tồn tại thành phần < p> nếu sử dụng cách chọn tag { thuộc tính: giá trị;}
  thì ta sẽ không thể nào chọn được đâu là thành phần thuộc content, đâu là thành phần thuộc navi, tuy nhiên sử dụng cách chọn theo cấp bậc thì việc này lại rất dễ dàng:
        div#content p { color: #333333; } /* Chon thanh phan p theo content*/
        div.navi p { background: #333333; } /* Chon thanh phan p theo navi*/
        div#content ul li { display: inline; } /* Chon thanh phan li theo content*/

### Cách viết một comment trong file CSS
- Comment là một dạng ghi chú, giúp người viết code giải thích nghĩa cho từng đoạn code,
 cách viết một comment trong CSS như sau:
        > /* Đây là dòng comment */

## Background trong CSS
- Thuộc tính background-color: thuộc tính này được sử dụng để thiết lập màu nền của một phần tử.
- Thuộc tính background-image: thuộc tính này được sử dụng để thiết lập hình nền cho một phần tử.
- Thuộc tính background-repeat: thuộc tính này được sử dụng để điều khiển sự lặp đi lặp lại của một hình ảnh nền theo chiều dọc 
  hoặc chiều ngang.
- Thuộc tính background-position: thuộc tính này được sử dụng để điều khiển vị trí của một hình ảnh nền.
- Thuộc tính background-attachment: thuộc tính này được sử dụng để xác định xem có hay không một hình nền là cố định hoặc 
  có thể scroll với phần còn lại của trang.
- Thuộc tính background: sử dụng thuộc tính này nếu bạn muốn viết ít code hơn mà vẫn xác định được tất cả 
  các thuộc tính liên quan tới background ở trên cho hình nền.

## Font trong CSS

- Thuộc tính font-family: được sử dụng để thay đổi bề mặt font.
- Thuộc tính font-style: được sử dụng để tạo một font chữ nghiêng hoặc chếch.
- Thuộc tính font-variant: được sử dụng để tạo những chữ hoa nhỏ (small-cap).
- Thuộc tính font-weight: được sử dụng để tăng giảm độ đậm của font.
- Thuộc tính font-size: được sử dụng để xác định kích cỡ font.
- Thuộc tính font: sử dụng thuộc tính này nếu bạn muốn viết ít code hơn mà vẫn xác định được các thuộc tính liên quan tới font ở trên.

### Thiết lập Font Family trong CSS

- Trong CSS, có hai loại Font Family:
1. generic family: một nhóm các Font Family có bề mặt khá tương tự nhau. Ví dụ Serif hoặc Monospace.
2. font family: một font family cụ thể, ví dụ như Time New Roman hoặc Arial.
- Để thay đổi bề mặt font của một phần tử nào đó, bạn có thể sử dụng thuộc tính font-family trong CSS.
- Nói chung, khi sử dụng thuộc tính font-family, bạn nên xác định nhiều hơn một giá trị. Nếu trình duyệt không hỗ trợ 
  giá trị font đầu tiên, nó sẽ thử giá trị tiếp theo, … Bắt đầu với giá trị font mà bạn muốn và kết thúc với một generic family để 
  trình duyệt chọn một font tương tự trong generic family nếu không có font nào có sẵn.

     > Ghi chú: Nếu tên font có nhiều hơn một từ, thì bạn phải đặt trong trích dẫn kép, ví dụ như: "Times New Roman".

### Thiết lập Font Style trong CSS

  Thuộc tính font-style trong CSS thường được sử dụng khi bạn muốn xác định một font chữ nghiêng. Các giá trị 
  mà thuộc tính này có thể nhận là: normal, italic hoặc oblique. Trong đó, normal là hiển thị văn bản như bình thường, 
  italic và oblique thì khá giống nhau, để hiển thị dạng nghiêng. Tuy nhiên, oblique ít được hỗ trợ hơn.

### Thiết lập Font Variant trong CSS

  Để tạo các chữ hoa nhỏ (dạng small-cap), bạn sử dụng thuộc tính font-variant trong CSS. 
  Thuộc tính này nhận hai giá trị là normal và small-caps.


## Text trong CSS

- Thuộc tính color được sử dụng để thiết lập màu cho văn bản.
- Thuộc tính direction được sử dụng để thiết lập hướng cho văn bản.
- Thuộc tính letter-spacing được sử dụng để thêm hoặc bớt khoảng cách giữa các chữ cái trong một từ.
- Thuộc tính word-spacing được sử dụng để tăng hoặc giảm khoảng cách giữa các từ trong một câu.
- Thuộc tính text-indent được sử dụng để tạo độ thụt của văn bản trong một đoạn văn.
- Thuộc tính text-align được sử dụng để căn chỉnh văn bản trong một tài liệu.
- Thuộc tính text-decoration được sử dụng để tạo cách dấu gạch ở chân, ở trên, ở giữa văn bản.
- Thuộc tính text-transform được sử dụng để chuyển văn bản thành chữ hoa hoặc chữ thường.
- Thuộc tính white-space được sử dụng để định dạng và điều khiển phần khoảng trắng của văn bản.
- Thuộc tính text-shadow được sử dụng để thiết lập hình bóng (shadow như trong word) xung quanh văn bản.

### Thiết lập màu trong CSS

- Để thiết lập màu cho văn bản trong CSS, bạn sử dụng thuộc tính color. Giá trị của thuộc tính này là bất kỳ tên màu 
  hoặc định dạng màu hợp lệ nào.

### Xác định hướng văn bản với thuộc tính direction trong CSS

  Để xác định hướng cho văn bản trong CSS (từ trái sang phải hay từ phải sang trái), bạn sử dụng thuộc tính direction.
  Thuộc tính này nhận một trong hai giá trị: ltr (trái sang phải) hoặc rtl (phải sang trái).

- Thiết lập khoảng cách giữa các chữ cái với thuộc tính letter-spacing trong CSS

  Giữa các chữ cái trong một từ nên có khoảng cách bằng bao nhiêu là hợp lý nhất. Để thiết lập khoảng cách này, 
  bạn sử dụng thuộc tính letter-spacing trong CSS. Thuộc tính này có thể nhận giá trị: normal hoặc một số cụ thể

### Thiết lập khoảng cách giữa các từ với thuộc tính word-spacing trong CSS

- Thiết lập khoảng cách giữa các từ trong một tài liệu một cách hợp lý sẽ giúp cho Webpage của bạn dễ đọc hơn. 
  Để thiết lập khoảng cách này, bạn sử dụng thuộc tính word-spacing trong CSS. 
  Thuộc tính này có thể nhận giá trị: normal hoặc một số cụ thể.

### Thiết lập độ thụt văn bản với thuộc tính text-indent trong CSS

- Trong một Website chất lượng, trong một đoạn văn hay một khối, từ đầu tiên của dòng đầu tiên nên được 
  thiết lập độ thụt dòng hợp lý. Điều này sẽ khiến Website của bạn đẹp và chuyên nghiệp hơn. Để thiết lập độ thụt dòng này, 
  bạn nên sử dụng thuộc tính text-indent trong CSS. Thuộc tính này có thể nhận các giá trị: % hoặc một số cụ thể.

### Căn chỉnh văn bản với thuộc tính text-align trong CSS

- Giống như trong Word, CSS có thuộc tính text-align để giúp bạn trong việc căn chỉnh văn bản. 
  Thuộc tính này có thể nhận một trong các giá trị :left, right, center, justify.

### Trang trí văn bản với thuộc tính text-decoration trong CSS
- Để tạo các dấu gạch ngang ở chân, ở trên hoặc ở giữa một đoạn văn bản, bạn sử dụng thuộc tính text-direction trong CSS. 
  Thuộc tính này có thể nhận giá trị: none, overline (dấu gạch ở trên), underline (gạch chân), line-through (gạch ngang) hoặc blink. 

