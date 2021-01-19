# Thuộc tính padding trong CSS

Thuộc tính padding cho phép bạn xác định khoảng không gian giữa nội dung hiển thị của một phần tử với đường viền của nó.

Giá trị của thuộc tính padding có thể ở dạng chiều dài (đơn vị px, pt, cm, …) , dạng %, hoặc từ khóa inherit. Nếu giá trị của thuộc tính là inherit, thì phần tử sẽ kế thừa giá trị của thuộc tính padding này từ phần tử cha của nó. Nếu giá trị là dạng %, thì đó là tỉ lệ phần trăm với hộp chứa phần tử này.

Với CSS, bạn không những có thể xác định padding cho toàn bộ phần không gian bao quanh nội dung, mà còn có thể xác định padding cho từng phần không gian này, ví dụ như phần trên, phần dưới, cạnh trái hoặc cạnh phải. Dưới đây là các thuộc tính trong CSS giúp bạn thực hiện việc này:

Thuộc tính **padding-bottom** xác định phần padding bên dưới của một phần tử.
Thuộc tính **padding-top** xác định phần padding bên trên của một phần tử.
Thuộc tính **padding-left** xác định phần padding bên trái của một phần tử.
Thuộc tính **padding-right** xác định phần padding bên phải của một phần tử.
Thuộc tính **padding** giúp bạn xác định toàn bộ các thuộc tính trên, tức là có thể xác định toàn bộ phần không gian padding bao quanh một phần tử.


# margin

Thuộc tính margin khi sử dụng sẽ thêm khoảng không gian bên ngoài thành phần, khoảng không gian này không cộng dồn thêm vào chiều rộng hoặc chiều cao của thành phần.

Dạng cơ bản gồm 4 thuộc tính:

**margin-top**: thêm khoảng không gian bên ngoài phía trên thành phần.
**margin-right**: thêm khoảng không gian bên ngoài phía bên phải thành phần.
**margin-bottom**: thêm khoảng không gian bên ngoài phía dưới thành phần.
**margin-left**: thêm khoảng không gian bên ngoài phía bên trái thành phần.

# float
Định nghĩa
- Thuộc tính float: xác định sự trôi nổi của thành phần.
- Thành phần nào sử dụng float sẽ được giải phóng vùng không gian, vùng không gian này sẽ trở thành vùng trống, và sẽ bị vùng không gian của những thành phần liền kề nó lập tức chiếm lấy.
- Khi sử dụng float, các thành phần không chồng chập lên nhau, mà sẽ sắp xếp vị trí tùy thuộc vào chiều rộng của vùng trống.
- Khi sử dụng float: left, vùng không gian của thành phần sẽ được giải phóng và thành phần sẽ trôi sang trái.
- Khi sử dụng float: right, vùng không gian của thành phần sẽ được giải phóng và thành phần sẽ trôi sang phải.

# clear

Thuộc tính clear: ngăn chặn thành phần A chiếm vùng không gian của thành phần B (với thành phần B là thành phần sử dụng float).
Thuộc tính clear có các giá trị sau:
    Thuộc tính **clear: left**:- ngăn chặn thành phần B chiếm chỗ thành phần A, khi thành phần A có sử dụng float: left;.
                           - không có tác dụng khi thành phần A sử dụng float: right;.
    Cách sử dụng clear: right; tương tự như clear: left;.
    Thuộc tính **clear: right**; - ngăn chặn thành phần B chiếm chỗ thành phần A, khi thành phần A có sử dụng float: right;.
                                 - không có tác dụng khi thành phần A sử dụng float: left;.
    Thuộc tính **clear: both**: - Khi cả 2 thành phần A và thành phần B sử dụng float, chúng ta không thể sử dụng clear: left; 
                                hay clear: right; để ngăn chặn thành phần C chiếm vùng không gian còn trống, trong trường hợp này ta sử dụng thuộc tính clear: both; để ngăn chặn sự chiếm vùng của thành phần C.
                                - Thuộc tính clear: both; có thể ngăn chặn sự chiếm vùng không gian cả khi chỉ có một thành phần sử dụng float (left hoặc right) hoặc nhiều thành phần sử dụng float.
    Thuộc tính **clear: none**; là dạng phục hồi khi Thành phần sử dụng thuộc tính clear.

# position
Thuộc tính position xác đinh vị trí tương đối và tuyệt đối cho thành phần, vị trí này phụ thuộc vào các giá trị khai báo của thành phần và thành phần bao ngoài nó.
Vị trí này có gốc được tính phía trên, bên phải, phía dưới và bên trái thành phần.
Các giá trị của thuộc tính position:
position: relative
position: absolute
position: fixed
position: static

## Cấu trúc
- Thuộc tính position đứng độc lập hoặc kèm theo các cặp giá trị định vị trí (theo chiều ngang và theo chiều thẳng đứng).
- Vị trí này được thể hiện thông qua các thuộc tính vị trí như:
    top: định vị trí bên trên của thành phần.
    right: định vị trí bên phải của thành phần.
    bottom: định vị trí bên dưới của thành phần.
    left: định vị trí bên trái của thành phần.
    Những vị trí này có thể sử dụng giá trị dương hay âm đều được

## position: relative
Thuộc tính position: relative; định vị trí tương đối cho thành phần, khi sử dụng thuộc tính này thành phần sẽ định vị trí theo mốc vùng hiển thị của chính nó, vị trí này không phụ thuộc vào vùng không gian, vùng không gian vẫn được giữ như ban đầu.
## position: absolute
Thuộc tính position: absolute; định vị trí tuyệt đối cho thành phần, khi sử dụng thuộc tính này vùng không gian của thành phần sẽ biến mất (trở thành vùng trống), thành phần sẽ thoát khỏi vùng không gian của nó, gốc của thành phần lúc này sẽ được tính theo các tính chất sau:

    - Trường họp 1: Nếu không có các thuộc tính định vị trí (top, right, bottom, left) thì thành phần sẽ lấy gốc theo vùng hiển thị với giá trị mặc định top: 0 và left: 0.
    - Trường họp 2: Nếu có sử dụng các thuộc tính định vị trí, thì thành phần sẽ lấy gốc theo vùng không gian của trình duyệt đây cũng chính là vùng văn bản HTML.
    - Trường hợp 3: Nếu có thành phần bao ngoài được định vị trí tương đối (position: relative;) thì gốc của nó (thành phần sử dụng thuộc tính position: absolute;) sẽ được tính theo vùng hiển thị của thành phần bao ngoài nó.

# Kích cỡ trong CSS
Để thay đổi kích cỡ, bạn có thể sử dụng các thuộc tính trong CSS sau:
- Thuộc tính **height** xác định chiều cao của hộp.
- Thuộc tính **width** xác định độ rộng của hộp.
- Thuộc tính **line-height** xác định chiều cao của một dòng văn bản.
- Thuộc tính **max-height** thiết lập chiều cao tối đa của một hộp.
- Thuộc tính **min-height** thiết lập chiều cao tối thiểu của một hộp.
- Thuộc tính **max-width** thiết lập độ rộng tối thiểu của một hộp.
- Thuộc tính **min-width** thiết lập độ rộng tối thiểu của một hộp.