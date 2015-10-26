# Tổng quan về Semantic UI

## Phần 1: Giới thiệu chung về Semantic UI.

Hiện nay, Bootstrap và Foundation là hai front-end framework được các
lập trình viên web sử dụng nhiều nhất. Nhưng lịch sử luôn cho thấy rằng
sẽ luôn có một thứ tốt hơn sẽ xuất hiện và thay thế tất cả. Và điều đó
sẽ không còn xa vời sự xuất hiện của Semantic UI, một modern front-end
development framework.

Semantic UI được dựng trên [LESS](http://lesscss.org/) và jQuery. Mục
tiêu của framework là cho phép designer và developer có khả năng chia
sẻ UI thông qua 1 ngôn ngữ chung. Điều đó được thể hiện qua cách sử
dụng ngôn ngữ mô tả để đặt tên cho các lớp và các quy chuẩn thay thế cho
việc sử dụng các từ viết tắt ở các framework khác. Yếu tố này khiến cho
Semantic UI gần gũi hơn với cộng đồng sử dụng tiếng anh. Ngoải ra còn
phải kể đến một điểm cộng nữa của Semantic UI, nó được thiết kế phẳng
với kiểu dáng đẹp, tinh tế mang lại cho người dùng cảm giác gọn nhẹ đúng
với xu hướng thiết kế hiện đại ngày nay.

### Features

Semantic UI đặc biệt ở 2 điểm. Đầu tiên là phương thức framework được
cấu thành. Nó sử dụng 5 hạng mục mô tả để định nghĩa các thành phân UI
có khả năng tái sử dụng

- UI Element là một khối dựng cơ bản. Nó có thể xuất hiện một mình hay
  một nhóm thống nhất. Ví dụ như 1 button đọc lập hoặc một nhóm các
button.
- UI Collection là một nhóm các loại thuộc tính khác nhau có sự liên
  kết. Ví dụ 1 form có thể có các button, input, checkbox, icon ...
- UI View là đại diện cho một phần của nội dung website. Ví dụ như feed
  hoặc comment.
- UI Module là thành phần tương tác với các chức năng dựa trên
  JavaScript. Ví dụ accordion, dimmer, modal ...
- UI Behavior là môt thành phần không thể tồn tại độc lập, nhưng thay
  vào đó nó được sử dụng để them các chức năng vào các thành phần khác.
Ví dụ, form validation cung cấp chức năng xác nhận cho form.

Hầu hết các thành phần đều có type, state và variation. Ví dụ, loại của
button bao gồm: nút cơ bản, nút với icon, nút có hiệu ứng, hoặc nút có
thể được active, disabled, hay đang ở trạng tháng loading. Hơn nữa, 1
nút có thể thay đổi kích thước, màu sắc và có thể dịnh dạng như basic,
social, fluid, toggle ...

Semantic UI không những sử dụng các từ có ý nghĩa và cấu trúc tốt để đặt
tên lớp, mà còn sử dụng chúng trong việc đặt tên, xác định và mô tả cho
các thành phần của nó. Việc này được thấy nhiều hơn so với Bootstrap hay
Foundation.

Điểm đăc biệt thứ hai về Semantic UI là nó cung cấp một số tính năng và
thành phần không có trên các framework khác. Ví dụ, Feed và Comment ở UI
Views hay SideBar hay Shape của UI Modules. Ngoài ra, khi tương tác với
các thành phần của Semantic UI, ta có thể dễ dàng debug. Chỉ cần mở web
console sẽ thấy chính xác cách các thành phần của Semantic hoạt động.

Một điểm mạnh khác của Semantic UI là sử dụng phong cách tối thiểu giản
và trung tính, điều này giúp người lập trình dễ dàng trong việc tùy
chỉnh. Thêm nữa các thành phần của framework có tính chất linh động và
độc lập do đó người lập trình có thể dễ dàng lấy và sử dụng khi cần
thiết.

Semantic UI sử dụng `em` và `rem` làm đơn vị cho các thuộc tính của
mình. Điều này làm cho nó hoàn toàn đáp ứng và thích hợp với các kích
thước bất kỳ. Việc người lập trình cần làm chỉ là thay đổi kích thước
font chữ và mọi thứ sẽ tự đọng điều chỉnh kích cỡ cho phù hơp.

### Tiện lợi và ví dụ tương ứng

#### Concise HTML

Semantic UI coi các từ và lớp như các khái niệm trao đổi. Các lớp sử
dụng cú pháp như ngôn ngữ tự nhiên với sự quan hệ của các danh từ hay
trợ từ.

Ví dụ:

```html
<div class="ui three buttons">
  <button class="ui active button">One</button>
  <button class="ui button">Two</button>
  <button class="ui button">Three</button>
</div>
```

#### Intuitive Javascript

Semantic sử dụng các cụm từ đơn giản như là hành vi kích hoạt chức năng.
Mọi quyết định trong các thành phần như là thiết lập để các lập trình
viên có thể tùy chỉnh.

Ví dụ:

```js
$('select.dropdown')
  .dropdown('set selected', ['meteor', 'ember'])
;
```

```html
<select name="skills" multiple="" class="ui fluid dropdown">
  <option value="">Skills</option>
  <option value="angular">Angular</option>
  <option value="css">CSS</option>
  <option value="ember">Ember</option>
  <option value="html">HTML</option>
  <option value="javascript">Javascript</option>
  <option value="meteor">Meteor</option>
  <option value="node">NodeJS</option>
</select>
```

#### Simplified Debugging

Với Semantic, lập trình viên có thể dễ dàng debug

Ví dụ:

```js
$('.sequenced.images .image')
  .transition({
    debug     : true,
    animation : 'jiggle',
    duration  : 500,
    interval  : 200
  })
;
```

![Debug](http://i.imgur.com/m86njdo.gif)

### Kết luận

Trên đây mình đã giới thiệu qua với các bạn về semantic UI. Chi tiết về
từng thành phần mình sẽ giới thiệu trong các phần tiếp theo. Bài viết
được tìm hiểu vào tổng hợp từ
[http://semantic-ui.com/](http://semantic-ui.com/)
