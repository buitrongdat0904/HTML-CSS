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
- Trong file HTML bên trên, trong phần content và navi đều có tồn tại thành phần <p> nếu sử dụng cách chọn tag { thuộc tính: giá trị;}
  thì ta sẽ không thể nào chọn được đâu là thành phần thuộc content, đâu là thành phần thuộc navi, tuy nhiên sử dụng cách chọn theo cấp bậc thì việc này lại rất dễ dàng:
        div#content p { color: #333333; } /* Chon thanh phan p theo content*/

        div.navi p { background: #333333; } /* Chon thanh phan p theo navi*/

        div#content ul li { display: inline; } /* Chon thanh phan li theo content*/

### Cách viết một comment trong file CSS
- Comment là một dạng ghi chú, giúp người viết code giải thích nghĩa cho từng đoạn code,
 cách viết một comment trong CSS như sau:
        /* Đây là dòng comment */

  

