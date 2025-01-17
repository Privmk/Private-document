# HTML DUMBLE
###### *Created: Minh Quang Pham* 
###### Các nguồn tham khảo: Freecodecamp, OpenAI-GPT4o
---
# 0. Menu
> Title list
- [1. Title tag](#1-h1--h6-title-element-tag)
- [2. Paragraph tag](#2-p-paragraph-element-tag)
- [3. Comment syntax](#3-comment-syntax)
- [4. Main element](#4-main-semantic-element)
- [5. Technical: Nesting](#5-technical-nesting)
- [6. Image element](#6-img-element)
- [7. Anchor element](#7-a-anchor-element)
- [8. Technical: Nesting `<a>` into `<p>`](#8-technical-nesting-a-into-p)
- [9. Technical: Wrapping content in anchor tags](#9-technical-wrapping-content-in-anchor-tags)
- [10. Section element](#10-section-semantic-element)
- [11. Unordered list element](#11-ul-list-element)
- [12. Figure element](#12-figure-semantic-element)
- [13. Emphasis element](#13-em-emphasis-element)
- [14. Ordered list element](#14-ol-list-element)
- [15. Strong element](#15-strong-element)
- [16. Form element](#16-form-semantic-element)
- [17. Input element](#17-input-element)
- [18. Placeholder attribute](#18-placeholder-attribute)
- [19. Required attribute](#19-required-attribute)
- [20. Button element](#20-button-element)
- [21. Radio attribute](#21-radio-attribute)
- [22. Label element](#22-label-semantic-element)
- [23. id attribute](#23-id-attribute)
- [24. Fieldset & Legend element](#24-fieldset-and-legend-semantic-element)
- [25. checked attribute](#25-checked-attribute)
- [26. Header element](#26-header-semantic-element)
- [27. Footer element](#27-footer-semantic-element)
- [28. HTML5 template](#28-html5-html5-template)
- [29. metadata](#29-meta-metadata)
- [30. Link document to html](#30-link-link-document)
- [31. Style element](#31-style-css-element)
- [32. Article (semantic element)](#32-article-semantic-element)
- [33. Div (semantic element)](#33-div-semantic-element)

# 1. `<H1> ... <H6>` (title element tag)

> Các phần tử HTML có thẻ mở như `<h1>` và thẻ đóng như `</h1>`. Văn bản mà một phần tử sẽ hiển thị được đặt giữa thẻ mở và thẻ đóng của nó. 

**Theory:**

* **Phần tử HTML:** Là một khối xây dựng cơ bản trong HTML, đại diện cho một loại nội dung cụ thể trên trang web (ví dụ: tiêu đề, đoạn văn, hình ảnh).
* **Thẻ mở:** Thẻ bắt đầu một phần tử HTML.
* **Thẻ đóng:** Thẻ kết thúc một phần tử HTML.

Ví dụ:

```html
<h1>Đây là một tiêu đề cấp 1</h1> 
```

Trong ví dụ trên:

* `<h1>` là thẻ mở của phần tử tiêu đề cấp 1 (`h1`).
* `</h1>` là thẻ đóng của phần tử tiêu đề cấp 1.
* "Đây là một tiêu đề cấp 1" là văn bản sẽ được hiển thị bên trong phần tử tiêu đề.


> Các phần tử tiêu đề từ `<h1>` đến `<h6>` được sử dụng để thể hiện mức độ quan trọng của nội dung bên dưới chúng. Số càng nhỏ, mức độ quan trọng càng cao, do đó phần tử `<h2>` có mức độ quan trọng thấp hơn phần tử `<h1>`.

> **Ví dụ Code:**

> ```html
> <h1>tiêu đề quan trọng nhất</h1>
> <h2>tiêu đề quan trọng thứ hai</h2>
> <h3>tiêu đề quan trọng thứ ba</h3>
> <h4>tiêu đề quan trọng thứ tư</h4>
> <h5>tiêu đề quan trọng thứ năm</h5>
> <h6>tiêu đề ít quan trọng nhất</h6>
> ```

> Chỉ sử dụng một phần tử `<h1>` cho mỗi trang và đặt các tiêu đề có mức độ quan trọng thấp hơn bên dưới các tiêu đề có mức độ quan trọng cao hơn.

**Theory:**

* **Cấu trúc phân cấp:** Các thẻ tiêu đề HTML tạo thành một cấu trúc phân cấp, với `<h1>` là cấp cao nhất và `<h6>` là cấp thấp nhất.
* **Mức độ quan trọng:** Cấp cao hơn (số nhỏ hơn) thể hiện nội dung quan trọng hơn.
* **Sử dụng đúng cách:** Nên sử dụng một `<h1>` chính cho mỗi trang và sử dụng các thẻ tiêu đề thấp hơn để phân chia nội dung thành các phần nhỏ hơn.

- [0. Menu](#0-menu)

# 2. `<p>` (paragraph element tag)
> Phần tử `p` được sử dụng để tạo ra một đoạn văn bản trên trang web.

**Theory:**

* **Phần tử `p`:** Đại diện cho một đoạn văn bản trong HTML.
* **Đoạn văn:** Một khối văn bản thường được phân tách với các khối văn bản khác bằng khoảng trắng hoặc thụt đầu dòng.

**Ví dụ:**

```html
<p>Đây là một đoạn văn bản.</p>
```

Trong ví dụ trên, phần tử `p` chứa nội dung "Đây là một đoạn văn bản." và sẽ được hiển thị trên trang web dưới dạng một đoạn văn.

```html
<h1>This is a heading</h1> 
```

- [0. Menu](#0-menu)

# 3. Comment syntax

Chú thích (Commenting) cho phép bạn để lại thông điệp mà không làm ảnh hưởng đến hiển thị trên trình duyệt. Nó cũng cho phép bạn làm mã không hoạt động. Một chú thích trong HTML bắt đầu với `<!--`, chứa bất kỳ số lượng dòng văn bản nào và kết thúc với `-->`.

Dưới đây là một ví dụ về chú thích với nội dung TODO: Xóa h1:

```html
<!-- TODO: Remove h1 -->
```

- [0. Menu](#0-menu)

# 4. `<main>` (semantic element)

HTML5 có một số phần tử dùng để xác định các khu vực nội dung khác nhau. Những phần tử này giúp HTML của bạn dễ đọc hơn và hỗ trợ Tối ưu hóa Công cụ Tìm kiếm (SEO) cũng như khả năng truy cập (accessibility).

Phần tử `<main>` được sử dụng để đại diện cho nội dung chính của phần thân (body) trong tài liệu HTML. Nội dung bên trong phần tử `<main>` nên là duy nhất cho tài liệu và không nên lặp lại ở các phần khác của tài liệu. 

Ví dụ:

```html
<main>
  <h1>Welcome to CatPhotoApp</h1>
  <p>This is where you will find the best cat photos on the internet!</p>
</main>
```

- [0. Menu](#0-menu)

# 5. Technical:  Nesting

**Nesting** trong HTML (lồng nhau) là việc đặt một thẻ HTML bên trong một thẻ khác. Điều này rất phổ biến và cần thiết để tạo cấu trúc trang web hợp lý. 

### Quy tắc cơ bản của nesting
1. **Thẻ phải được đóng đúng thứ tự**: Nếu một thẻ được mở bên trong một thẻ khác, nó phải được đóng trước khi thẻ bên ngoài đóng.
   ```html
   <!-- Đúng -->
   <div>
       <p>Đây là đoạn văn</p>
   </div>

   <!-- Sai -->
   <div>
       <p>Đây là đoạn văn</div>
       </p>
   ```

2. **Nội dung hợp lệ**: Một số thẻ chỉ được chứa các thẻ con cụ thể. Ví dụ:
   - `<ul>` chỉ chứa `<li>`.
   - `<table>` chỉ chứa các thẻ như `<thead>`, `<tbody>`, `<tr>`, `<td>`, v.v.

   ```html
   <!-- Đúng -->
   <ul>
       <li>Phần tử 1</li>
       <li>Phần tử 2</li>
   </ul>

   <!-- Sai -->
   <ul>
       <div>Phần tử không hợp lệ</div>
   </ul>
   ```

3. **Tránh lồng quá sâu**: Nesting quá nhiều thẻ có thể làm cho mã khó đọc và khó bảo trì.

### Ví dụ về nesting
#### Danh sách lồng nhau:
```html
<ul>
    <li>Mục 1</li>
    <li>Mục 2
        <ul>
            <li>Mục 2.1</li>
            <li>Mục 2.2</li>
        </ul>
    </li>
    <li>Mục 3</li>
</ul>
```

#### Form với thẻ lồng nhau:
```html
<form action="/submit" method="post">
    <label for="username">Tên người dùng:</label>
    <input type="text" id="username" name="username">
    
    <label for="password">Mật khẩu:</label>
    <input type="password" id="password" name="password">
    
    <button type="submit">Đăng nhập</button>
</form>
```

#### Sử dụng thẻ `<div>` và `<span>`:
```html
<div>
    <h1>Tiêu đề chính</h1>
    <p>Đây là đoạn văn với <span style="color: red;">một từ được tô màu đỏ</span>.</p>
</div>
```

### Lưu ý
- Sử dụng thụt lề để mã dễ đọc.
- Tuân thủ quy tắc đóng thẻ để tránh lỗi hiển thị hoặc không tương thích giữa các trình duyệt.

- [0. Menu](#0-menu)

# 6. `<img>` (element)

Thẻ `<img>` trong HTML được sử dụng để hiển thị hình ảnh trên trang web. Đây là thẻ không có thẻ đóng và yêu cầu một số thuộc tính để hoạt động hiệu quả.

---

### **Cấu trúc cơ bản của thẻ `<img>`**
```html
<img src="URL_hoặc_đường_dẫn_đến_hình_ảnh" alt="Mô tả_hình_ảnh">
```

---

### **Các thuộc tính quan trọng của thẻ `<img>`**

1. **`src`** (source - nguồn): 
   - Đây là thuộc tính bắt buộc.
   - Chỉ định URL hoặc đường dẫn của hình ảnh.
   - Hình ảnh có thể từ nguồn nội bộ hoặc bên ngoài (external).

   Ví dụ:
   ```html
   <img src="images/logo.png" alt="Logo của công ty">
   <img src="https://example.com/image.jpg" alt="Hình ảnh từ trang web khác">
   ```

2. **`alt`** (alternative text - văn bản thay thế):
   - Văn bản mô tả nội dung của hình ảnh.
   - Hiển thị khi hình ảnh không tải được hoặc dành cho trình đọc màn hình (truy cập web cho người khiếm thị).
   - Cần viết ngắn gọn và mô tả ý nghĩa của hình ảnh.

   Ví dụ:
   ```html
   <img src="images/photo.jpg" alt="Ảnh chụp hoàng hôn trên biển">
   ```

3. **`width` và `height`**:
   - Đặt kích thước hình ảnh theo pixel (px) hoặc phần trăm (%).
   - Không nên chỉnh kích thước trực tiếp bằng HTML nếu không cần thiết; thay vào đó sử dụng CSS để kiểm soát.

   Ví dụ:
   ```html
   <img src="images/photo.jpg" alt="Ảnh" width="300" height="200">
   ```

4. **`title`**:
   - Hiển thị văn bản chú thích khi người dùng di chuột qua hình ảnh.

   Ví dụ:
   ```html
   <img src="images/logo.png" alt="Logo công ty" title="Logo chính thức của công ty">
   ```

5. **`loading`**:
   - Kiểm soát việc tải hình ảnh.
   - Các giá trị:
     - `lazy`: Chỉ tải hình ảnh khi nó xuất hiện trong vùng hiển thị của trình duyệt.
     - `eager`: Tải ngay lập tức.
     - `auto`: Trình duyệt tự quyết định.

   Ví dụ:
   ```html
   <img src="images/photo.jpg" alt="Ảnh" loading="lazy">
   ```

6. **`crossorigin`**:
   - Được dùng khi tải hình ảnh từ nguồn bên ngoài (CORS).
   - Giá trị:
     - `anonymous`: Không gửi thông tin xác thực.
     - `use-credentials`: Gửi thông tin xác thực.

---

### **Ví dụ đầy đủ**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ví dụ thẻ img</title>
</head>
<body>
    <h1>Hình ảnh minh họa</h1>
    <img src="https://via.placeholder.com/300" alt="Hình minh họa" width="300" height="200" title="Hình ảnh mẫu" loading="lazy">
</body>
</html>
```

---

### **Lưu ý khi sử dụng thẻ `<img>`**
1. **Tối ưu hóa hình ảnh**:
   - Sử dụng định dạng ảnh phù hợp như JPEG, PNG, WebP để tối ưu kích thước và chất lượng.
2. **Sử dụng `alt` hiệu quả**:
   - Đừng bỏ trống `alt` trừ khi hình ảnh chỉ mang tính trang trí.
3. **Responsive Image**:
   - Sử dụng CSS để hình ảnh tương thích trên nhiều thiết bị:
     ```css
     img {
         max-width: 100%;
         height: auto;
     }
     ```

     - [0. Menu](#0-menu)

# 7. `<a>` (anchor element)

Thẻ `<a>` trong HTML (anchor tag) được sử dụng để tạo liên kết, cho phép người dùng điều hướng đến các trang web, tài liệu, hoặc vị trí khác trong cùng trang.

---

### **Cấu trúc cơ bản của thẻ `<a>`**
```html
<a href="URL hoặc đường dẫn">Nội dung hiển thị</a>
```

---

### **Các thuộc tính quan trọng của thẻ `<a>`**

1. **`href`** (hyperlink reference - tham chiếu liên kết):
   - Thuộc tính bắt buộc.
   - Chỉ định URL hoặc đường dẫn mà liên kết sẽ dẫn đến.
   - URL có thể là:
     - **Tuyệt đối**: Đường dẫn đầy đủ (bao gồm giao thức như `https://`).
       ```html
       <a href="https://www.google.com">Google</a>
       ```
     - **Tương đối**: Đường dẫn dựa trên vị trí của tệp HTML hiện tại.
       ```html
       <a href="/about.html">Trang Giới thiệu</a>
       ```

2. **`target`**:
   - Xác định nơi hiển thị nội dung của liên kết.
   - Các giá trị phổ biến:
     - `_self` (mặc định): Mở trong cùng tab hoặc cửa sổ.
     - `_blank`: Mở trong tab hoặc cửa sổ mới.
     - `_parent`: Mở trong khung cha (nếu dùng iframe).
     - `_top`: Mở trong cửa sổ toàn bộ (thoát khỏi khung iframe nếu có).
   - Ví dụ:
     ```html
     <a href="https://www.example.com" target="_blank">Mở trong tab mới</a>
     ```

3. **`rel`** (relationship - mối quan hệ):
   - Xác định mối quan hệ giữa trang hiện tại và trang được liên kết.
   - Các giá trị phổ biến:
     - `nofollow`: Ngăn các công cụ tìm kiếm theo dõi liên kết.
     - `noopener`: Tăng cường bảo mật khi sử dụng `target="_blank"`.
     - `noreferrer`: Không gửi thông tin tham chiếu đến trang được liên kết.
   - Ví dụ:
     ```html
     <a href="https://www.example.com" target="_blank" rel="noopener noreferrer">Liên kết an toàn</a>
     ```

4. **`download`**:
   - Cho phép tải xuống tệp khi nhấp vào liên kết.
   - Có thể đặt tên tệp tùy ý.
   - Ví dụ:
     ```html
     <a href="files/document.pdf" download="TaiLieu.pdf">Tải tài liệu</a>
     ```

5. **`title`**:
   - Hiển thị chú thích khi người dùng di chuột qua liên kết.
   - Ví dụ:
     ```html
     <a href="https://www.example.com" title="Trang chủ của Example">Trang chủ</a>
     ```

6. **`type`**:
   - Xác định loại MIME của tài liệu được liên kết (thường không cần thiết).
   - Ví dụ:
     ```html
     <a href="files/document.pdf" type="application/pdf">Tải PDF</a>
     ```

---

### **Ví dụ cơ bản**

#### Liên kết đến một trang web:
```html
<a href="https://www.google.com">Google</a>
```

#### Mở liên kết trong tab mới:
```html
<a href="https://www.wikipedia.org" target="_blank">Wikipedia</a>
```

#### Liên kết tải xuống tệp:
```html
<a href="images/photo.jpg" download="HinhAnh.jpg">Tải hình ảnh</a>
```

#### Liên kết đến một phần cụ thể trong cùng trang:
```html
<!-- Liên kết -->
<a href="#section1">Đi đến Phần 1</a>

<!-- Đích đến -->
<h2 id="section1">Phần 1</h2>
```


---

### **Lưu ý khi sử dụng thẻ `<a>`**
1. **Đảm bảo URL hợp lệ**: Đường dẫn phải đúng và dẫn đến tài nguyên có sẵn.
2. **Thêm `alt` cho liên kết có chứa hình ảnh**: Nếu liên kết chứa hình ảnh, sử dụng thuộc tính `alt` trong thẻ `<img>` để cải thiện khả năng truy cập.
3. **Sử dụng `rel="noopener noreferrer"` với `target="_blank"`**: Điều này giúp bảo mật tốt hơn và ngăn các trang bên ngoài truy cập vào cửa sổ của bạn.
4. **Không lạm dụng liên kết**: Chỉ thêm liên kết khi cần thiết và liên quan đến nội dung.

- [0. Menu](#0-menu)

# 8. Technical: Nesting `<a>` into `<p>` 

Lồng thẻ `<a>` (liên kết) bên trong thẻ `<p>` (đoạn văn) là một cách hợp lý trong HTML vì nó giúp cấu trúc trang web trở nên dễ hiểu hơn và đảm bảo tính hợp lệ của mã HTML. Dưới đây là một số lý do vì sao việc lồng thẻ `<a>` vào trong thẻ `<p>` là hợp lý:

### 1. **Cấu trúc hợp lý và hợp lệ**
   - Thẻ `<p>` đại diện cho một đoạn văn bản, và thẻ `<a>` là thẻ dùng để tạo liên kết. Việc lồng thẻ `<a>` vào trong thẻ `<p>` giúp đảm bảo rằng liên kết sẽ là một phần của nội dung văn bản, làm cho mã HTML trở nên hợp lệ.
   - Theo chuẩn HTML5, bạn có thể lồng thẻ `<a>` trong thẻ `<p>` mà không gặp lỗi. Điều này là hợp lệ và phổ biến khi bạn muốn tạo một đoạn văn có chứa liên kết.

   Ví dụ:
   ```html
   <p>Để tìm hiểu thêm về HTML, bạn có thể tham khảo <a href="https://www.w3schools.com">W3Schools</a>.</p>
   ```

### 2. **Tính tổ chức và dễ đọc**
   - Việc lồng thẻ `<a>` trong thẻ `<p>` giúp duy trì tính tổ chức của nội dung, đặc biệt là khi bạn muốn một liên kết trở thành một phần của đoạn văn bản. Điều này giúp mã HTML dễ đọc và dễ hiểu hơn cho người phát triển và những người khác làm việc với mã.
   - Cấu trúc này làm cho liên kết trở thành một phần tự nhiên của nội dung văn bản thay vì đặt nó tách biệt với các phần khác.

### 3. **Tính tương thích với các công cụ và trình duyệt**
   - Các trình duyệt web và công cụ phân tích mã HTML có thể hiểu và hiển thị liên kết bên trong thẻ `<p>` mà không gặp phải vấn đề tương thích. Điều này giúp đảm bảo rằng liên kết hoạt động như mong muốn trên tất cả các trình duyệt.
   
### 4. **Cải thiện khả năng truy cập**
   - Khi sử dụng thẻ `<p>` để bao quanh một liên kết, bạn giữ cho cấu trúc văn bản rõ ràng và dễ tiếp cận hơn cho người dùng sử dụng trình đọc màn hình. Thẻ `<p>` giúp phân tách các đoạn văn bản, trong khi thẻ `<a>` cho phép người dùng nhấp vào liên kết.

### 5. **Tránh các vấn đề khi lồng ngược lại**
   - Lồng thẻ `<p>` vào thẻ `<a>` là không hợp lệ trong HTML. Việc này có thể gây ra lỗi khi trang web được hiển thị hoặc phân tích cú pháp. Vì vậy, bạn nên luôn đảm bảo rằng thẻ `<a>` được đặt bên trong thẻ `<p>`, chứ không phải ngược lại.

---

### Ví dụ minh họa:

```html
<p>Hãy truy cập vào <a href="https://www.example.com">website của chúng tôi</a> để biết thêm chi tiết.</p>
```

Ở ví dụ trên:
- Liên kết `<a>` là một phần của đoạn văn, giúp người dùng dễ dàng nhấp vào mà không cần phải rời khỏi ngữ cảnh của văn bản.
- Đoạn văn bản này có thể được trình bày tốt trong các trang web, dễ đọc và dễ hiểu.

- [0. Menu](#0-menu)

# 9. Technical: Wrapping content in anchor tags

Việc **gói các thẻ bên trong thẻ `<a>`** là một hành động cần phải cân nhắc kỹ, vì không phải tất cả các thẻ HTML đều hợp lệ khi đặt bên trong thẻ `<a>`. Thẻ `<a>` được thiết kế để tạo ra các liên kết, và có một số quy định nhất định về những thẻ nào có thể lồng vào bên trong thẻ này.

### Các thẻ hợp lệ bên trong thẻ `<a>`
Theo chuẩn HTML5, bạn có thể gói một số thẻ HTML bên trong thẻ `<a>` mà không gặp vấn đề. Dưới đây là các thẻ phổ biến có thể được lồng trong thẻ `<a>`:

1. **Thẻ văn bản**: Các thẻ như `<span>`, `<strong>`, `<em>`, `<b>`, `<i>` đều có thể được sử dụng trong thẻ `<a>`. Điều này cho phép bạn tạo liên kết với các phần tử văn bản đặc biệt.

   ```html
   <a href="https://www.example.com"><span>Click vào đây</span></a>
   ```

2. **Hình ảnh**: Bạn có thể lồng thẻ `<img>` vào thẻ `<a>`, tạo liên kết cho hình ảnh.

   ```html
   <a href="https://www.example.com">
       <img src="logo.png" alt="Logo Example">
   </a>
   ```

3. **Thẻ danh sách**: Thẻ `<li>` có thể nằm trong thẻ `<a>`, tuy nhiên, thông thường thẻ `<a>` sẽ bao quanh các thẻ `<li>` khi bạn muốn các mục trong danh sách có thể nhấp được.

   ```html
   <a href="https://www.example.com">
       <ul>
           <li>Home</li>
           <li>About</li>
           <li>Contact</li>
       </ul>
   </a>
   ```

4. **Thẻ hình học**: Các thẻ như `<svg>`, `<path>`, `<circle>`, v.v., cũng có thể được sử dụng trong thẻ `<a>` để tạo liên kết cho các hình vẽ SVG.

   ```html
   <a href="https://www.example.com">
       <svg width="100" height="100">
           <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
       </svg>
   </a>
   ```

5. **Thẻ nút**: Bạn có thể sử dụng thẻ `<button>` bên trong thẻ `<a>`, mặc dù điều này không phải lúc nào cũng được khuyến khích vì nó có thể gây mâu thuẫn về mặt ngữ nghĩa. Tuy nhiên, trong một số trường hợp, nó có thể hữu ích khi bạn muốn có nút nhấp được và điều hướng.

   ```html
   <a href="https://www.example.com">
       <button>Click me</button>
   </a>
   ```

---

### Các thẻ **không hợp lệ** khi đặt trong thẻ `<a>`
- **Thẻ khối (block-level elements)** như `<div>`, `<p>`, `<form>`, `<header>`, `<footer>`, `<article>`, và các thẻ khối khác **không được phép lồng trong thẻ `<a>`**. Điều này là do thẻ `<a>` vốn là một thẻ **inline** (dòng), trong khi các thẻ khối thường không thể lồng vào nhau theo cách này.

   ```html
   <!-- Sai: không thể gói thẻ <div> vào thẻ <a> -->
   <a href="https://www.example.com">
       <div>Đây là một phần tử div không hợp lệ trong <a></div>
   </a>
   ```

   Thay vào đó, bạn có thể làm như sau:
   ```html
   <a href="https://www.example.com">
       <div>Đây là một phần tử div có thể nhấp vào</div>
   </a>
   ```

---
- Việc **gói các thẻ bên trong thẻ `<a>`** là hợp lệ khi các thẻ đó là các thẻ inline hoặc thẻ nội tuyến như `<span>`, `<img>`, `<strong>`, hoặc các thẻ có thể chứa nội dung văn bản hoặc hình ảnh.
- Tuy nhiên, không nên lồng các thẻ khối như `<div>`, `<p>`, `<header>`, `<footer>` vào thẻ `<a>`, vì chúng không hợp lệ và có thể gây lỗi khi hiển thị hoặc khi phân tích cú pháp HTML.

- [0. Menu](#0-menu)

# 10. `<section>` (semantic element)

Thẻ `<section>` trong HTML là một phần tử cấu trúc được sử dụng để nhóm các nội dung có liên quan lại với nhau trong một phần cụ thể của trang web. Mục đích chính của thẻ `<section>` là phân chia trang thành các phần nhỏ hơn và dễ hiểu hơn, giúp cải thiện khả năng tổ chức nội dung và hỗ trợ cho SEO (tối ưu hóa công cụ tìm kiếm).

### **Cấu trúc cơ bản của thẻ `<section>`**

```html
<section>
    <h2>Tiêu đề phần</h2>
    <p>Nội dung của phần này.</p>
</section>
```

### **Đặc điểm và công dụng của thẻ `<section>`**

1. **Nhóm nội dung liên quan**:
   - Thẻ `<section>` được sử dụng để nhóm các phần nội dung có liên quan, ví dụ như một bài viết, một chủ đề, một đoạn văn bản hoặc một nhóm hình ảnh, bảng biểu. Mỗi phần nội dung trong trang có thể được bao quanh bởi một thẻ `<section>`.
   
2. **Cải thiện khả năng truy cập và SEO**:
   - Việc sử dụng thẻ `<section>` giúp cấu trúc trang web rõ ràng hơn, làm cho nội dung dễ hiểu hơn đối với người dùng và các công cụ tìm kiếm. Các công cụ tìm kiếm có thể sử dụng thẻ này để hiểu rõ hơn về các phần khác nhau của trang web, từ đó cải thiện xếp hạng trang.

3. **Tổ chức nội dung theo chủ đề**:
   - Thẻ `<section>` giúp chia nội dung của trang web thành các phần nhỏ hơn, dễ quản lý hơn. Ví dụ, một bài viết có thể có các phần như "Giới thiệu", "Nội dung chính", "Kết luận", mỗi phần có thể được bao quanh bởi thẻ `<section>`.

4. **Không phải là thẻ khối (block-level element)**:
   - Thẻ `<section>` là một thẻ khối (block-level element), nghĩa là nó sẽ chiếm toàn bộ chiều rộng của phần tử cha và xuất hiện trên một dòng mới.

5. **Thường kết hợp với tiêu đề**:
   - Mỗi thẻ `<section>` thường được kết hợp với một thẻ tiêu đề (`<h1>`, `<h2>`, v.v.) để xác định chủ đề hoặc nội dung của phần đó. Điều này giúp cả người dùng và các công cụ tìm kiếm hiểu rõ hơn về nội dung của phần.

### **Ví dụ về thẻ `<section>`**

#### 1. **Phân chia nội dung của bài viết**
```html
<article>
    <section>
        <h2>Giới thiệu</h2>
        <p>Đây là phần giới thiệu về chủ đề bài viết.</p>
    </section>

    <section>
        <h2>Nội dung chính</h2>
        <p>Phần này chứa nội dung chi tiết của bài viết.</p>
    </section>

    <section>
        <h2>Kết luận</h2>
        <p>Phần kết luận của bài viết.</p>
    </section>
</article>
```

#### 2. **Phân chia một trang thành các phần độc lập**
```html
<section>
    <h2>Giới thiệu về công ty</h2>
    <p>Thông tin giới thiệu về công ty XYZ.</p>
</section>

<section>
    <h2>Dịch vụ của chúng tôi</h2>
    <ul>
        <li>Dịch vụ 1</li>
        <li>Dịch vụ 2</li>
        <li>Dịch vụ 3</li>
    </ul>
</section>

<section>
    <h2>Liên hệ</h2>
    <p>Thông tin liên hệ của công ty XYZ.</p>
</section>
```

#### 3. **Sử dụng trong một trang tin tức hoặc blog**
```html
<article>
    <header>
        <h1>Tin tức mới nhất</h1>
    </header>

    <section>
        <h2>Chủ đề 1</h2>
        <p>Thông tin về chủ đề 1.</p>
    </section>

    <section>
        <h2>Chủ đề 2</h2>
        <p>Thông tin về chủ đề 2.</p>
    </section>

    <footer>
        <p>Ngày đăng: 15/01/2025</p>
    </footer>
</article>
```

### **Lưu ý khi sử dụng thẻ `<section>`**
1. **Không dùng `<section>` thay thế cho thẻ `<div>`**:
   - Thẻ `<section>` không phải là một thẻ thay thế cho `<div>`. Bạn chỉ nên sử dụng thẻ `<section>` khi các nội dung trong đó có liên quan đến một chủ đề hoặc phần cụ thể của trang. Nếu không có sự liên quan, hãy sử dụng thẻ `<div>` để nhóm các phần tử.

2. **Sử dụng thẻ tiêu đề trong mỗi `<section>`**:
   - Mỗi thẻ `<section>` nên có ít nhất một thẻ tiêu đề (`<h1>`, `<h2>`, v.v.) để giúp người dùng và các công cụ tìm kiếm dễ dàng nhận diện chủ đề của phần nội dung đó.

3. **Không dùng thẻ `<section>` cho các phần nhỏ không cần phân chia rõ ràng**:
   - Nếu phần nội dung không cần phải được phân chia thành một chủ đề rõ ràng, thì không nên sử dụng thẻ `<section>`. Thay vào đó, bạn có thể sử dụng các thẻ khác như `<div>` hoặc các thẻ inline.

Thẻ `<section>` là một công cụ mạnh mẽ trong việc tổ chức và phân chia nội dung trên trang web. Việc sử dụng thẻ này giúp cải thiện cấu trúc trang web, làm cho nội dung dễ tiếp cận và dễ hiểu hơn đối với cả người dùng và công cụ tìm kiếm.

- [0. Menu](#0-menu)

# 11. `<ul>` (list element)

Thẻ `<ul>` trong HTML là một phần tử được sử dụng để tạo danh sách không có thứ tự (unordered list). Mỗi mục trong danh sách này được đánh dấu bằng thẻ `<li>`, đại diện cho một mục trong danh sách.

### **Cấu trúc cơ bản của thẻ `<ul>`**

```html
<ul>
    <li>Mục 1</li>
    <li>Mục 2</li>
    <li>Mục 3</li>
</ul>
```

### **Đặc điểm của thẻ `<ul>`**

1. **Danh sách không có thứ tự**:
   - Thẻ `<ul>` tạo ra một danh sách mà các mục trong danh sách không có thứ tự rõ ràng. Các mục trong danh sách được đánh dấu bằng các dấu chấm (hoặc ký hiệu khác tùy theo trình duyệt hoặc kiểu CSS).

2. **Thẻ `<li>` dùng để xác định mỗi mục trong danh sách**:
   - Mỗi mục trong danh sách được đặt trong một thẻ `<li>`, là viết tắt của "list item" (mục danh sách). Thẻ `<li>` có thể chứa văn bản, hình ảnh, liên kết, hoặc các phần tử HTML khác.

3. **Sử dụng cho các mục không theo thứ tự**:
   - Thẻ `<ul>` thích hợp khi bạn muốn tạo một danh sách các mục mà không cần phải sắp xếp chúng theo thứ tự cụ thể. Ví dụ, danh sách các loại thực phẩm, danh sách các công việc cần làm, v.v.

### **Ví dụ về thẻ `<ul>`**

#### 1. **Danh sách không có thứ tự đơn giản**
```html
<ul>
    <li>Apple</li>
    <li>Banana</li>
    <li>Orange</li>
</ul>
```

Kết quả hiển thị sẽ là:
- Apple
- Banana
- Orange

#### 2. **Danh sách với các mục phức tạp hơn**
```html
<ul>
    <li><a href="https://www.example.com">Trang chủ</a></li>
    <li><a href="https://www.example.com/about">Giới thiệu</a></li>
    <li><a href="https://www.example.com/contact">Liên hệ</a></li>
</ul>
```

Kết quả hiển thị:
- Trang chủ
- Giới thiệu
- Liên hệ

#### 3. **Danh sách lồng nhau**
Thẻ `<ul>` cũng có thể chứa các thẻ `<ul>` khác để tạo ra danh sách lồng nhau.

```html
<ul>
    <li>Fruits
        <ul>
            <li>Apple</li>
            <li>Banana</li>
            <li>Orange</li>
        </ul>
    </li>
    <li>Vegetables
        <ul>
            <li>Carrot</li>
            <li>Broccoli</li>
        </ul>
    </li>
</ul>
```

Kết quả hiển thị:
- Fruits
    - Apple
    - Banana
    - Orange
- Vegetables
    - Carrot
    - Broccoli

### **Các thuộc tính của thẻ `<ul>`**

1. **`type`**:
   - Thuộc tính `type` dùng để thay đổi kiểu của dấu đánh dấu trong danh sách. Tuy nhiên, thuộc tính này đã bị deprecated trong HTML5 và không còn được khuyến khích sử dụng.

   ```html
   <ul type="square">
       <li>Apple</li>
       <li>Banana</li>
       <li>Orange</li>
   </ul>
   ```

   Các giá trị của thuộc tính `type` có thể là:
   - `disc`: Dấu chấm (mặc định).
   - `circle`: Dấu vòng tròn.
   - `square`: Dấu vuông.

2. **CSS để thay đổi kiểu danh sách**:
   - Bạn có thể thay đổi kiểu dấu của danh sách bằng CSS, ví dụ:
   
   ```html
   <ul style="list-style-type: square;">
       <li>Apple</li>
       <li>Banana</li>
       <li>Orange</li>
   </ul>
   ```

   Hoặc thay đổi bằng cách sử dụng các thuộc tính khác như `list-style-image` để thay đổi dấu chấm thành một hình ảnh.

3. **`class` và `id`**:
   - Bạn có thể sử dụng thuộc tính `class` hoặc `id` để định danh cho thẻ `<ul>`, giúp áp dụng các kiểu CSS hoặc tương tác JavaScript.

   ```html
   <ul class="fruit-list">
       <li>Apple</li>
       <li>Banana</li>
       <li>Orange</li>
   </ul>
   ```

### **Lưu ý khi sử dụng thẻ `<ul>`**

1. **Không dùng `<ul>` cho danh sách có thứ tự**:
   - Nếu bạn cần tạo một danh sách có thứ tự (sắp xếp theo thứ tự nhất định), bạn nên sử dụng thẻ `<ol>` (ordered list) thay vì `<ul>`. Thẻ `<ol>` sẽ đánh số các mục trong danh sách.

2. **Danh sách có thể chứa các phần tử HTML khác**:
   - Mỗi mục trong danh sách (`<li>`) có thể chứa các thẻ HTML khác như thẻ liên kết (`<a>`), thẻ hình ảnh (`<img>`), hoặc các thẻ văn bản khác.

3. **Sử dụng danh sách để cải thiện cấu trúc nội dung**:
   - Thẻ `<ul>` giúp tạo ra một cấu trúc rõ ràng cho nội dung trang web, dễ dàng cho người dùng đọc và hiểu, đặc biệt khi có nhiều mục cần liệt kê.


Thẻ `<ul>` rất hữu ích khi bạn muốn tạo danh sách các mục không có thứ tự, giúp cải thiện khả năng tổ chức và trình bày nội dung trên trang web. Thẻ này có thể kết hợp với các thẻ khác như `<li>`, `<a>`, và sử dụng CSS để tùy chỉnh kiểu hiển thị.

- [0. Menu](#0-menu)

# 12. `<figure>` (semantic element)

Thẻ `<figure>` trong HTML được sử dụng để nhóm một hình ảnh hoặc nội dung liên quan đến hình ảnh (như chú thích, video, bảng, hoặc đồ họa) và có thể kèm theo một chú thích với thẻ `<figcaption>`. Thẻ `<figure>` giúp cải thiện khả năng truy cập và SEO bằng cách liên kết trực tiếp giữa hình ảnh và chú thích của nó.

Thẻ `<h3>` là thẻ tiêu đề cấp ba trong HTML, được sử dụng để tạo tiêu đề cho các phần nội dung trong trang web. Khi kết hợp với thẻ `<figure>`, bạn có thể tạo một tiêu đề cho một phần nội dung liên quan đến hình ảnh.

### **Cấu trúc cơ bản của thẻ `<figure>` và `<h3>`**

```html
<figure>
    <h3>Tiêu đề hình ảnh</h3>
    <img src="image.jpg" alt="Mô tả hình ảnh">
    <figcaption>Chú thích cho hình ảnh</figcaption>
</figure>
```

### **Giải thích các phần tử:**
1. **`<figure>`**: Dùng để nhóm các phần tử liên quan đến hình ảnh hoặc nội dung đồ họa.
2. **`<h3>`**: Tạo tiêu đề cho phần nội dung bên trong `<figure>`. Thẻ `<h3>` thường được sử dụng cho các tiêu đề cấp ba, nhưng bạn có thể sử dụng các cấp khác như `<h1>`, `<h2>`, v.v. tùy theo cấu trúc của trang.
3. **`<img>`**: Chứa hình ảnh cần hiển thị. Thuộc tính `src` chứa đường dẫn đến hình ảnh và `alt` cung cấp mô tả thay thế cho hình ảnh nếu không thể tải.
4. **`<figcaption>`**: Cung cấp chú thích cho nội dung trong `<figure>`, như mô tả hình ảnh hoặc thông tin bổ sung.

### **Ví dụ về thẻ `<figure>` và `<h3>`**

#### 1. **Hình ảnh với tiêu đề và chú thích**
```html
<figure>
    <h3>Phong cảnh thiên nhiên</h3>
    <img src="landscape.jpg" alt="Phong cảnh thiên nhiên">
    <figcaption>Hình ảnh này mô tả một cảnh đẹp với núi non và mây trời.</figcaption>
</figure>
```

Kết quả hiển thị sẽ có:
- Tiêu đề "Phong cảnh thiên nhiên".
- Hình ảnh "landscape.jpg".
- Chú thích "Hình ảnh này mô tả một cảnh đẹp với núi non và mây trời."

#### 2. **Danh sách hình ảnh với tiêu đề và chú thích**
```html
<figure>
    <h3>Hình ảnh của một chiếc xe</h3>
    <img src="car.jpg" alt="Chiếc xe ô tô">
    <figcaption>Đây là hình ảnh của một chiếc xe ô tô hiện đại.</figcaption>
</figure>

<figure>
    <h3>Hình ảnh của một chiếc máy bay</h3>
    <img src="airplane.jpg" alt="Chiếc máy bay">
    <figcaption>Đây là hình ảnh của một chiếc máy bay đang bay trên bầu trời.</figcaption>
</figure>
```

Kết quả hiển thị sẽ là:
- Hai phần tử `<figure>` với các hình ảnh và chú thích tương ứng.

### **Tính năng và ứng dụng của thẻ `<figure>`**

1. **Cải thiện khả năng tổ chức nội dung**:
   - Thẻ `<figure>` giúp nhóm hình ảnh với các phần liên quan (như tiêu đề, chú thích), giúp cải thiện cấu trúc trang web và dễ dàng cho người dùng hiểu được mối quan hệ giữa hình ảnh và các thông tin đi kèm.

2. **SEO và khả năng truy cập**:
   - Việc sử dụng `<figcaption>` giúp cung cấp thông tin chi tiết về hình ảnh, điều này hỗ trợ SEO và giúp các công cụ tìm kiếm hiểu rõ hơn về nội dung hình ảnh. Chú thích cũng giúp người dùng khiếm thị hiểu được nội dung hình ảnh qua công nghệ đọc màn hình.

3. **Sử dụng trong bài viết hoặc trang blog**:
   - Thẻ `<figure>` rất hữu ích trong các bài viết hoặc blog nơi hình ảnh có vai trò quan trọng trong việc minh họa cho nội dung. Bạn có thể sử dụng `<h3>` để tạo tiêu đề cho mỗi hình ảnh, làm rõ nội dung của hình ảnh trong bối cảnh bài viết.

### **Lưu ý khi sử dụng thẻ `<figure>` và `<h3>`**
- **Đảm bảo sự liên kết giữa tiêu đề và hình ảnh**: Tiêu đề trong thẻ `<h3>` nên rõ ràng và có mối liên hệ trực tiếp với hình ảnh, giúp người đọc dễ dàng hiểu nội dung của hình ảnh.
- **Chú thích nên ngắn gọn và súc tích**: Chú thích trong `<figcaption>` nên cung cấp thông tin bổ sung mà không làm cho người đọc cảm thấy quá tải.


Thẻ `<figure>` kết hợp với thẻ `<h3>` là một cách tuyệt vời để tạo ra cấu trúc rõ ràng và dễ hiểu cho các phần nội dung có hình ảnh trong trang web của bạn. Việc sử dụng `<figure>` giúp tổ chức các nội dung hình ảnh, trong khi thẻ `<h3>` tạo ra tiêu đề rõ ràng, giúp cải thiện khả năng truy cập và SEO.

- [0. Menu](#0-menu)

# 13. `<em>` (emphasis element)

Thẻ `<em>` trong HTML được sử dụng để đánh dấu văn bản cần được nhấn mạnh hoặc nhấn mạnh về mặt ngữ nghĩa, giúp người đọc hoặc công cụ tìm kiếm hiểu rằng nội dung này quan trọng hơn các phần còn lại. Nội dung bên trong thẻ `<em>` thường được hiển thị dưới dạng in nghiêng (italic) trong trình duyệt mặc định, mặc dù kiểu hiển thị có thể được thay đổi bằng CSS.

### **Cấu trúc cơ bản của thẻ `<em>`**

```html
<p>Đây là một ví dụ về thẻ <em>nhấn mạnh</em> trong văn bản.</p>
```

Kết quả hiển thị sẽ là:
- "Đây là một ví dụ về thẻ *nhấn mạnh* trong văn bản."

### **Mục đích và ý nghĩa của thẻ `<em>`**

1. **Nhấn mạnh nội dung**:
   - Thẻ `<em>` được sử dụng để làm nổi bật một phần văn bản, thể hiện rằng phần đó có sự nhấn mạnh hoặc quan trọng trong ngữ cảnh của câu. Việc sử dụng thẻ `<em>` cho phép người đọc dễ dàng nhận ra các từ hoặc cụm từ quan trọng.
   
2. **Ngữ nghĩa trong văn bản**:
   - Mặc dù trình duyệt thường hiển thị văn bản trong thẻ `<em>` bằng kiểu chữ in nghiêng (italic), mục đích chính của thẻ là nhấn mạnh ngữ nghĩa của văn bản thay vì chỉ là việc thay đổi kiểu hiển thị. Do đó, thẻ `<em>` mang tính ngữ nghĩa hơn là chỉ là một kiểu dáng.

3. **Hỗ trợ cho SEO và khả năng truy cập**:
   - Các công cụ tìm kiếm và công nghệ hỗ trợ người khiếm thị (như đọc màn hình) sẽ chú ý đến nội dung trong thẻ `<em>`. Điều này có thể giúp cải thiện khả năng tìm kiếm và khả năng truy cập của trang web.

### **Ví dụ về thẻ `<em>`**

#### 1. **Nhấn mạnh một từ trong câu**
```html
<p>Chúng tôi <em>khuyến khích</em> bạn tham gia khóa học này để nâng cao kỹ năng.</p>
```
Kết quả hiển thị:
- "Chúng tôi *khuyến khích* bạn tham gia khóa học này để nâng cao kỹ năng."

#### 2. **Nhấn mạnh một cụm từ trong đoạn văn**
```html
<p>Việc hoàn thành dự án đúng hạn là rất <em>quan trọng</em> đối với công ty.</p>
```
Kết quả hiển thị:
- "Việc hoàn thành dự án đúng hạn là rất *quan trọng* đối với công ty."

#### 3. **Sử dụng thẻ `<em>` với nhiều từ**
```html
<p><em>Học tập liên tục</em> sẽ giúp bạn phát triển nghề nghiệp một cách bền vững.</p>
```
Kết quả hiển thị:
- "*Học tập liên tục* sẽ giúp bạn phát triển nghề nghiệp một cách bền vững."

### **Sự khác biệt giữa thẻ `<em>` và thẻ `<i>`**

- **`<em>`**: Được sử dụng để nhấn mạnh ngữ nghĩa của văn bản. Nội dung trong thẻ này có thể được trình bày dưới dạng in nghiêng (italic), nhưng mục đích chính là nhấn mạnh ngữ nghĩa, không chỉ thay đổi kiểu dáng.
  
- **`<i>`**: Thẻ `<i>` chỉ thay đổi kiểu dáng văn bản thành in nghiêng mà không mang bất kỳ ngữ nghĩa nhấn mạnh nào. Thẻ này chỉ thay đổi kiểu hiển thị mà không làm thay đổi ý nghĩa của văn bản.

Ví dụ:
```html
<p><em>Nhấn mạnh</em> và <i>in nghiêng</i> là khác nhau.</p>
```
Kết quả hiển thị:
- "*Nhấn mạnh* và *in nghiêng* là khác nhau."

### **Ứng dụng của thẻ `<em>`**

1. **Nhấn mạnh từ khóa quan trọng trong bài viết**:
   - Trong các bài viết hoặc blog, bạn có thể sử dụng thẻ `<em>` để làm nổi bật những từ khóa quan trọng hoặc các cụm từ quan trọng trong nội dung, giúp người đọc dễ dàng nhận ra điểm nhấn.

2. **Tạo sự chú ý trong các bài thuyết trình hoặc thông báo**:
   - Nếu bạn đang tạo một trang web thông báo hoặc bài thuyết trình, thẻ `<em>` giúp làm nổi bật các phần quan trọng mà bạn muốn người đọc chú ý.

3. **Hỗ trợ cho SEO**:
   - Nhấn mạnh các từ hoặc cụm từ quan trọng với thẻ `<em>` có thể giúp các công cụ tìm kiếm hiểu được các điểm trọng tâm trong nội dung của bạn, từ đó cải thiện thứ hạng tìm kiếm.


Thẻ `<em>` là một công cụ hữu ích trong HTML để nhấn mạnh ngữ nghĩa của văn bản, giúp làm rõ nội dung quan trọng trong trang web. Ngoài ra, thẻ này còn hỗ trợ SEO và khả năng truy cập, đồng thời giúp trình bày văn bản một cách hợp lý và dễ hiểu hơn.

- [0. Menu](#0-menu)

# 14. `<ol>` (list element)

Thẻ `<ol>` trong HTML được sử dụng để tạo một danh sách có thứ tự (ordered list). Mỗi mục trong danh sách được đánh số tự động và hiển thị theo thứ tự từ 1 trở đi, hoặc có thể được tùy chỉnh với các loại đánh số khác nhau như số, chữ cái, hoặc chữ số la mã.

### **Cấu trúc cơ bản của thẻ `<ol>`**

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

Kết quả hiển thị sẽ là:
1. Item 1
2. Item 2
3. Item 3

### **Các thành phần trong thẻ `<ol>`**
- **`<ol>`**: Đây là thẻ chính để tạo danh sách có thứ tự.
- **`<li>`**: Mỗi phần tử trong danh sách được đặt trong thẻ `<li>`, đại diện cho một mục trong danh sách.

### **Các thuộc tính của thẻ `<ol>`**

1. **`type`**: Thuộc tính này xác định kiểu đánh số cho danh sách. Có ba giá trị chính:
   - `1`: Đánh số bằng chữ số (mặc định).
   - `A`: Đánh số bằng chữ cái viết hoa (A, B, C, ...).
   - `a`: Đánh số bằng chữ cái viết thường (a, b, c, ...).
   - `I`: Đánh số bằng chữ số La Mã viết hoa (I, II, III, ...).
   - `i`: Đánh số bằng chữ số La Mã viết thường (i, ii, iii, ...).

   **Ví dụ**:
   ```html
   <ol type="A">
     <li>Apple</li>
     <li>Banana</li>
     <li>Cherry</li>
   </ol>
   ```
   Kết quả hiển thị:
   A. Apple
   B. Banana
   C. Cherry

2. **`start`**: Thuộc tính này xác định số bắt đầu của danh sách. Mặc định, danh sách bắt đầu từ 1, nhưng bạn có thể thay đổi số bắt đầu theo ý muốn.
   
   **Ví dụ**:
   ```html
   <ol start="5">
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ol>
   ```
   Kết quả hiển thị:
   5. Item 1
   6. Item 2
   7. Item 3

3. **`reversed`**: Thuộc tính này làm đảo ngược thứ tự của danh sách, bắt đầu từ số lớn nhất và giảm dần xuống số nhỏ nhất.
   
   **Ví dụ**:
   ```html
   <ol reversed>
     <li>First</li>
     <li>Second</li>
     <li>Third</li>
   </ol>
   ```
   Kết quả hiển thị:
   3. First
   2. Second
   1. Third

4. **`compact`**: Thuộc tính này không còn được sử dụng trong HTML5, nhưng trong các phiên bản HTML cũ, nó dùng để giảm khoảng cách giữa các mục trong danh sách.

### **Ví dụ sử dụng thẻ `<ol>` với các thuộc tính**

```html
<ol type="I" start="3">
  <li>Introduction</li>
  <li>Content</li>
  <li>Conclusion</li>
</ol>
```

Kết quả hiển thị:
III. Introduction  
IV. Content  
V. Conclusion

### **Ứng dụng của thẻ `<ol>`**

1. **Danh sách các bước trong hướng dẫn**:
   Thẻ `<ol>` rất hữu ích khi bạn cần liệt kê các bước trong một hướng dẫn hoặc quy trình, ví dụ như trong hướng dẫn cài đặt phần mềm hoặc các bài tập thực hành.

   **Ví dụ**:
   ```html
   <ol>
     <li>Đăng nhập vào tài khoản</li>
     <li>Chọn sản phẩm bạn muốn mua</li>
     <li>Thanh toán và xác nhận đơn hàng</li>
   </ol>
   ```

2. **Danh sách thứ tự quan trọng**:
   Khi bạn cần liệt kê các mục theo thứ tự ưu tiên hoặc mức độ quan trọng, sử dụng thẻ `<ol>` sẽ giúp người dùng dễ dàng theo dõi.

3. **Danh sách đánh số trong các bài viết**:
   Trong các bài viết, thẻ `<ol>` có thể giúp liệt kê các ý chính hoặc các điểm cần nhấn mạnh theo thứ tự rõ ràng, giúp người đọc dễ dàng theo dõi.

Thẻ `<ol>` là một công cụ hữu ích trong HTML để tạo các danh sách có thứ tự, cho phép bạn tổ chức nội dung theo một cách dễ hiểu và có trật tự. Thẻ này có thể được tùy chỉnh để thay đổi kiểu đánh số, bắt đầu từ số khác, hoặc đảo ngược thứ tự, giúp bạn linh hoạt trong việc trình bày thông tin.

- [0. Menu](#0-menu)

# 15. `<strong>` (element)

Thẻ `<strong>` trong HTML được sử dụng để nhấn mạnh một phần nội dung trong văn bản, thể hiện rằng nội dung này có tầm quan trọng đặc biệt. Theo ngữ nghĩa, thẻ `<strong>` không chỉ làm nổi bật văn bản mà còn giúp người đọc hoặc các công cụ tìm kiếm nhận ra rằng phần văn bản này có ý nghĩa quan trọng.

Mặc định, văn bản trong thẻ `<strong>` thường được hiển thị dưới dạng **in đậm** (bold), mặc dù kiểu hiển thị có thể được thay đổi bằng CSS.

### **Cấu trúc cơ bản của thẻ `<strong>`**

```html
<p>Hãy chú ý đến <strong>quan trọng</strong> trong bài học này.</p>
```

Kết quả hiển thị:
- "Hãy chú ý đến **quan trọng** trong bài học này."

### **Mục đích và ý nghĩa của thẻ `<strong>`**

1. **Nhấn mạnh nội dung quan trọng**:
   - Thẻ `<strong>` giúp nhấn mạnh một phần văn bản có ý nghĩa đặc biệt trong ngữ cảnh của bài viết. Nó không chỉ thay đổi kiểu dáng của văn bản mà còn chỉ ra rằng phần đó có sự quan trọng trong thông điệp hoặc nội dung mà bạn muốn truyền tải.

2. **Tăng khả năng hiểu cho công cụ tìm kiếm và công nghệ hỗ trợ**:
   - Các công cụ tìm kiếm như Google sẽ chú ý đến nội dung trong thẻ `<strong>` vì nó có thể chứa các từ khóa quan trọng. Hơn nữa, các công nghệ hỗ trợ như màn hình đọc cho người khiếm thị cũng có thể nhận ra phần nội dung này và giúp người dùng hiểu rõ hơn về thông điệp.

### **Ví dụ về thẻ `<strong>`**

#### 1. **Nhấn mạnh một từ trong câu**
```html
<p>Chúng tôi <strong>khuyến khích</strong> bạn tham gia khóa học này để nâng cao kỹ năng.</p>
```
Kết quả hiển thị:
- "Chúng tôi **khuyến khích** bạn tham gia khóa học này để nâng cao kỹ năng."

#### 2. **Nhấn mạnh cụm từ trong đoạn văn**
```html
<p>Việc hoàn thành dự án đúng hạn là rất <strong>quan trọng</strong> đối với công ty.</p>
```
Kết quả hiển thị:
- "Việc hoàn thành dự án đúng hạn là rất **quan trọng** đối với công ty."

#### 3. **Sử dụng thẻ `<strong>` trong bài viết dài**
```html
<p><strong>Chú ý:</strong> Hãy đảm bảo rằng tất cả các tài liệu đã được kiểm tra kỹ trước khi nộp.</p>
```
Kết quả hiển thị:
- "**Chú ý:** Hãy đảm bảo rằng tất cả các tài liệu đã được kiểm tra kỹ trước khi nộp."

### **Sự khác biệt giữa thẻ `<strong>` và thẻ `<b>`**

- **`<strong>`**: Được sử dụng để nhấn mạnh ngữ nghĩa của văn bản. Nội dung trong thẻ này thường được hiển thị dưới dạng **in đậm**, nhưng mục đích chính là nhấn mạnh về mặt ngữ nghĩa, không chỉ thay đổi kiểu dáng.
  
- **`<b>`**: Thẻ `<b>` chỉ thay đổi kiểu dáng của văn bản thành **in đậm**, mà không có ý nghĩa nhấn mạnh về mặt ngữ nghĩa. Thẻ này chỉ đơn giản là thay đổi cách thức hiển thị mà không mang tính chất ngữ nghĩa.

**Ví dụ**:
```html
<p><strong>Quan trọng:</strong> Đừng quên gửi báo cáo trước khi kết thúc tuần.</p>
<p><b>In đậm:</b> Đoạn này chỉ để làm nổi bật mà không có ý nghĩa quan trọng.</p>
```
Kết quả hiển thị:
- "**Quan trọng:** Đừng quên gửi báo cáo trước khi kết thúc tuần."
- "**In đậm:** Đoạn này chỉ để làm nổi bật mà không có ý nghĩa quan trọng."

### **Ứng dụng của thẻ `<strong>`**

1. **Nhấn mạnh các từ khóa quan trọng trong bài viết**:
   Thẻ `<strong>` có thể được sử dụng để làm nổi bật các từ khóa hoặc các ý chính trong một bài viết, giúp người đọc dễ dàng nhận ra thông tin quan trọng.

2. **Thông báo quan trọng**:
   Trong các thông báo hoặc cảnh báo, thẻ `<strong>` giúp nhấn mạnh phần nội dung cần sự chú ý đặc biệt của người đọc.

3. **SEO**:
   Việc sử dụng thẻ `<strong>` giúp các công cụ tìm kiếm nhận diện các từ khóa quan trọng trong nội dung, từ đó cải thiện thứ hạng tìm kiếm.

4. **Khả năng truy cập**:
   Các công nghệ hỗ trợ như đọc màn hình sẽ chú ý đến nội dung trong thẻ `<strong>`, giúp người khiếm thị hiểu rõ hơn về thông điệp của phần văn bản.


Thẻ `<strong>` là một công cụ hữu ích trong HTML để nhấn mạnh các phần văn bản quan trọng về mặt ngữ nghĩa, giúp người đọc nhận diện được các ý chính trong bài viết. Thẻ này không chỉ thay đổi kiểu hiển thị mà còn giúp cải thiện SEO và khả năng truy cập cho trang web của bạn.

- [0. Menu](#0-menu)

# 16. `<form>` (semantic element)

Thẻ `<form>` trong HTML được sử dụng để tạo một biểu mẫu (form) trên trang web, cho phép người dùng nhập liệu và gửi thông tin tới một máy chủ để xử lý. Biểu mẫu này có thể bao gồm nhiều loại trường nhập liệu như ô văn bản, ô chọn, nút bấm, v.v.

### **Cấu trúc cơ bản của thẻ `<form>`**

```html
<form action="submit_form.php" method="POST">
  <label for="name">Họ và tên:</label>
  <input type="text" id="name" name="name" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br><br>

  <input type="submit" value="Gửi">
</form>
```

### **Các thuộc tính của thẻ `<form>`**

1. **`action`**:
   - Thuộc tính này xác định URL mà biểu mẫu sẽ gửi dữ liệu đến khi người dùng nhấn nút gửi (submit). Đây là địa chỉ của máy chủ hoặc trang web mà dữ liệu sẽ được xử lý.
   - Ví dụ: `<form action="submit_form.php" method="POST">`.

2. **`method`**:
   - Thuộc tính này xác định phương thức HTTP mà biểu mẫu sẽ sử dụng để gửi dữ liệu. Có hai phương thức chính:
     - `GET`: Dữ liệu được gửi qua URL (thích hợp cho các yêu cầu tìm kiếm hoặc lấy thông tin mà không làm thay đổi trạng thái của máy chủ).
     - `POST`: Dữ liệu được gửi trong thân của yêu cầu HTTP, bảo mật hơn và thích hợp cho các biểu mẫu thay đổi dữ liệu trên máy chủ (ví dụ: đăng nhập, gửi thông tin).
   - Ví dụ: `<form action="submit_form.php" method="POST">`.

3. **`target`**:
   - Thuộc tính này xác định cửa sổ hoặc khung (frame) mà trang trả về sẽ hiển thị. Các giá trị phổ biến của `target` bao gồm:
     - `_self`: Mặc định, dữ liệu sẽ được gửi về trang hiện tại.
     - `_blank`: Mở kết quả trong một cửa sổ hoặc tab mới.
     - `_parent` hoặc `_top`: Các giá trị này liên quan đến khung (frame).
   
   Ví dụ:
   ```html
   <form action="submit_form.php" method="POST" target="_blank">
   ```

4. **`enctype`**:
   - Thuộc tính này xác định cách thức mã hóa dữ liệu khi gửi. Cần thiết khi bạn sử dụng phương thức `POST` và muốn gửi tệp đính kèm (file upload).
     - `application/x-www-form-urlencoded`: Mặc định, dữ liệu sẽ được mã hóa thành chuỗi khóa/giá trị.
     - `multipart/form-data`: Sử dụng khi gửi tệp (file).
     - `text/plain`: Dữ liệu sẽ được mã hóa dưới dạng văn bản thuần túy.
   
   Ví dụ:
   ```html
   <form action="submit_form.php" method="POST" enctype="multipart/form-data">
   ```

5. **`name`**:
   - Thuộc tính này chỉ định tên của biểu mẫu, có thể dùng để tham chiếu biểu mẫu trong JavaScript hoặc khi gửi dữ liệu.
   
   Ví dụ:
   ```html
   <form name="myForm" action="submit_form.php" method="POST">
   ```

### **Các phần tử trong thẻ `<form>`**

- **`<input>`**: Thẻ này dùng để tạo các trường nhập liệu, ví dụ như ô văn bản, ô chọn, checkbox, radio, v.v.
  - Ví dụ:
    ```html
    <input type="text" name="username">
    ```

- **`<label>`**: Dùng để gắn nhãn cho các trường nhập liệu. Thuộc tính `for` của thẻ `<label>` phải trùng với `id` của thẻ `<input>`.
  - Ví dụ:
    ```html
    <label for="username">Tên người dùng:</label>
    <input type="text" id="username" name="username">
    ```

- **`<textarea>`**: Dùng để tạo ô nhập liệu nhiều dòng.
  - Ví dụ:
    ```html
    <textarea name="message" rows="4" cols="50"></textarea>
    ```

- **`<select>` và `<option>`**: Dùng để tạo danh sách thả xuống (dropdown).
  - Ví dụ:
    ```html
    <select name="country">
      <option value="VN">Việt Nam</option>
      <option value="US">Hoa Kỳ</option>
      <option value="JP">Nhật Bản</option>
    </select>
    ```

- **`<button>`**: Tạo nút bấm trong biểu mẫu, có thể dùng để gửi biểu mẫu hoặc thực hiện một hành động khác.
  - Ví dụ:
    ```html
    <button type="submit">Gửi</button>
    ```

### **Ví dụ về biểu mẫu đơn giản**

```html
<form action="submit_form.php" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br><br>

  <label for="gender">Giới tính:</label>
  <input type="radio" id="male" name="gender" value="male"> Nam
  <input type="radio" id="female" name="gender" value="female"> Nữ<br><br>

  <label for="country">Quốc gia:</label>
  <select name="country" id="country">
    <option value="VN">Việt Nam</option>
    <option value="US">Hoa Kỳ</option>
    <option value="JP">Nhật Bản</option>
  </select><br><br>

  <label for="message">Thông điệp:</label><br>
  <textarea name="message" id="message" rows="4" cols="50"></textarea><br><br>

  <input type="submit" value="Gửi">
</form>
```

Thẻ `<form>` là một phần quan trọng trong HTML, giúp người dùng tương tác với trang web thông qua việc nhập liệu và gửi thông tin. Nó có thể chứa nhiều loại phần tử nhập liệu khác nhau, từ ô văn bản, checkbox, radio button đến các nút bấm. Biểu mẫu có thể được tùy chỉnh thông qua các thuộc tính như `action`, `method`, `enctype` và `target` để đáp ứng các yêu cầu cụ thể của ứng dụng web.

- [0. Menu](#0-menu)


# 17. `<input>` (element)

Thẻ `<input>` trong HTML được sử dụng để tạo các trường nhập liệu trong biểu mẫu (form). Nó là một trong những thẻ quan trọng và linh hoạt nhất trong HTML vì có thể sử dụng với nhiều loại trường khác nhau như ô văn bản, checkbox, radio, mật khẩu, tệp, và nhiều loại khác. Tùy thuộc vào giá trị của thuộc tính `type`, thẻ `<input>` có thể có các chức năng khác nhau.

### **Cấu trúc cơ bản của thẻ `<input>`**

```html
<input type="text" name="username" id="username">
```

### **Các thuộc tính phổ biến của thẻ `<input>`**

1. **`type`**:
   - Xác định loại của trường nhập liệu. Các giá trị phổ biến của `type` bao gồm:
     - `text`: Trường nhập liệu dạng văn bản.
     - `password`: Trường nhập mật khẩu (văn bản sẽ bị ẩn).
     - `email`: Trường nhập email (kiểm tra định dạng email).
     - `number`: Trường nhập số (chỉ chấp nhận số).
     - `checkbox`: Trường nhập kiểu checkbox (chọn hoặc không chọn).
     - `radio`: Trường nhập kiểu radio (chỉ chọn một lựa chọn trong nhóm).
     - `file`: Cho phép người dùng chọn tệp.
     - `submit`: Nút gửi biểu mẫu.
     - `reset`: Nút reset biểu mẫu.
     - `date`: Trường nhập ngày tháng.
     - `button`: Nút bấm thông thường (không gửi dữ liệu).
   
   Ví dụ:
   ```html
   <input type="text" name="username">
   <input type="password" name="password">
   <input type="checkbox" name="subscribe">
   <input type="file" name="fileUpload">
   ```

2. **`name`**:
   - Xác định tên của trường nhập liệu, sẽ được sử dụng khi gửi dữ liệu từ biểu mẫu.
   
   Ví dụ:
   ```html
   <input type="text" name="username">
   ```

3. **`id`**:
   - Xác định ID duy nhất cho thẻ `<input>`, thường dùng để liên kết với thẻ `<label>` hoặc trong JavaScript để thao tác với phần tử.
   
   Ví dụ:
   ```html
   <input type="text" id="username">
   ```

4. **`value`**:
   - Xác định giá trị mặc định hoặc giá trị đã chọn của trường nhập liệu. Đối với các loại trường như `checkbox`, `radio`, hoặc `submit`, `value` xác định giá trị sẽ được gửi khi biểu mẫu được gửi đi.
   
   Ví dụ:
   ```html
   <input type="checkbox" name="subscribe" value="yes">
   <input type="radio" name="gender" value="male">
   ```

5. **`placeholder`**:
   - Cung cấp một gợi ý văn bản cho người dùng khi trường nhập liệu chưa có giá trị. Văn bản này sẽ biến mất khi người dùng bắt đầu nhập.
   
   Ví dụ:
   ```html
   <input type="text" name="username" placeholder="Nhập tên người dùng">
   ```

6. **`required`**:
   - Đánh dấu trường nhập liệu là bắt buộc, người dùng phải nhập dữ liệu vào trước khi gửi biểu mẫu.
   
   Ví dụ:
   ```html
   <input type="email" name="email" required>
   ```

7. **`readonly`**:
   - Làm cho trường nhập liệu chỉ đọc, người dùng không thể thay đổi giá trị của nó.
   
   Ví dụ:
   ```html
   <input type="text" name="username" value="admin" readonly>
   ```

8. **`disabled`**:
   - Làm cho trường nhập liệu không thể thao tác được, không thể thay đổi giá trị hoặc gửi dữ liệu.
   
   Ví dụ:
   ```html
   <input type="text" name="username" disabled>
   ```

9. **`size`**:
   - Xác định độ rộng của trường nhập liệu, chỉ áp dụng cho loại `text` và `password`.
   
   Ví dụ:
   ```html
   <input type="text" name="username" size="30">
   ```

10. **`maxlength`**:
    - Xác định số ký tự tối đa mà người dùng có thể nhập vào trường nhập liệu.
    
    Ví dụ:
    ```html
    <input type="text" name="username" maxlength="10">
    ```

### **Các loại trường nhập liệu phổ biến với thẻ `<input>`**

1. **Text Input**:
   - Trường nhập liệu cho văn bản thông thường.
   ```html
   <input type="text" name="username">
   ```

2. **Password Input**:
   - Trường nhập liệu mật khẩu (văn bản sẽ bị ẩn).
   ```html
   <input type="password" name="password">
   ```

3. **Email Input**:
   - Trường nhập liệu cho email (kiểm tra định dạng email).
   ```html
   <input type="email" name="email">
   ```

4. **Number Input**:
   - Trường nhập liệu cho số (chỉ chấp nhận số).
   ```html
   <input type="number" name="age">
   ```

5. **Checkbox Input**:
   - Trường nhập liệu kiểu checkbox (người dùng có thể chọn hoặc không chọn).
   ```html
   <input type="checkbox" name="subscribe" value="yes"> Đăng ký nhận tin
   ```

6. **Radio Input**:
   - Trường nhập liệu kiểu radio (chỉ cho phép chọn một trong các lựa chọn).
   ```html
   <input type="radio" name="gender" value="male"> Nam
   <input type="radio" name="gender" value="female"> Nữ
   ```

7. **File Input**:
   - Trường nhập liệu cho phép người dùng chọn một tệp để tải lên.
   ```html
   <input type="file" name="fileUpload">
   ```

8. **Submit Button**:
   - Nút gửi biểu mẫu.
   ```html
   <input type="submit" value="Gửi">
   ```

9. **Reset Button**:
   - Nút để đặt lại tất cả các trường trong biểu mẫu về giá trị mặc định.
   ```html
   <input type="reset" value="Đặt lại">
   ```

10. **Date Input**:
    - Trường nhập liệu cho phép người dùng chọn một ngày.
    ```html
    <input type="date" name="birthday">
    ```

### **Ví dụ về thẻ `<input>` trong một biểu mẫu**

```html
<form action="/submit" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" required><br><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br><br>

  <label for="gender">Giới tính:</label>
  <input type="radio" id="male" name="gender" value="male"> Nam
  <input type="radio" id="female" name="gender" value="female"> Nữ<br><br>

  <input type="submit" value="Gửi">
</form>
```

Thẻ `<input>` là một phần quan trọng trong HTML, giúp tạo các trường nhập liệu đa dạng trong biểu mẫu. Thẻ này hỗ trợ nhiều loại trường nhập khác nhau, từ ô văn bản, mật khẩu, số, checkbox đến nút gửi, giúp người dùng có thể tương tác với trang web một cách dễ dàng.

### **Nesting `<input>` into `<form>`**

Lồng thẻ `<input>` bên trong thẻ `<form>` là một cách tổ chức hợp lý để tạo các trường nhập liệu trong một biểu mẫu. Thẻ `<form>` sẽ bao gồm tất cả các thẻ `<input>` và các phần tử khác cần thiết để người dùng có thể nhập dữ liệu và gửi đi. Mỗi thẻ `<input>` đại diện cho một trường nhập liệu riêng biệt, có thể là ô văn bản, mật khẩu, checkbox, hoặc các loại khác.

### **Cấu trúc cơ bản của việc lồng thẻ `<input>` trong thẻ `<form>`**

```html
<form action="/submit" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" required><br><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br><br>

  <input type="submit" value="Gửi">
</form>
```

### **Giải thích**

1. **Thẻ `<form>`**:
   - Được sử dụng để bao bọc tất cả các trường nhập liệu và nút gửi. Thẻ này xác định nơi mà dữ liệu sẽ được gửi khi người dùng nhấn nút gửi (`submit`).
   - Thuộc tính `action` xác định URL nơi dữ liệu sẽ được gửi đi khi biểu mẫu được gửi.
   - Thuộc tính `method` xác định phương thức HTTP mà biểu mẫu sẽ sử dụng để gửi dữ liệu (thường là `GET` hoặc `POST`).

2. **Các thẻ `<input>`**:
   - Các thẻ `<input>` đại diện cho các trường nhập liệu mà người dùng có thể tương tác.
   - Mỗi trường có thể có thuộc tính `type` để xác định loại dữ liệu người dùng có thể nhập, ví dụ như `text`, `password`, `email`, v.v.
   - Các thẻ `<input>` này được lồng bên trong thẻ `<form>`, cho phép thu thập và gửi thông tin khi biểu mẫu được gửi đi.

3. **Thẻ `<label>`**:
   - Thẻ `<label>` được sử dụng để gắn nhãn cho các trường nhập liệu. Thuộc tính `for` của thẻ `<label>` phải trùng với `id` của thẻ `<input>` để tạo liên kết giữa chúng, giúp cải thiện khả năng truy cập.

4. **Nút `submit`**:
   - Thẻ `<input type="submit">` tạo một nút gửi để người dùng có thể gửi dữ liệu trong biểu mẫu.

### **Ví dụ đầy đủ về biểu mẫu với nhiều trường nhập liệu**

```html
<form action="submit_form.php" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" required><br><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br><br>

  <label for="gender">Giới tính:</label>
  <input type="radio" id="male" name="gender" value="male"> Nam
  <input type="radio" id="female" name="gender" value="female"> Nữ<br><br>

  <label for="subscribe">Đăng ký nhận tin:</label>
  <input type="checkbox" id="subscribe" name="subscribe" value="yes"><br><br>

  <input type="submit" value="Gửi">
</form>
```
Lồng thẻ `<input>` bên trong thẻ `<form>` là cách cơ bản để xây dựng các biểu mẫu trong HTML. Việc này giúp tổ chức và thu thập thông tin từ người dùng một cách dễ dàng. Biểu mẫu có thể bao gồm nhiều loại trường nhập liệu, và thẻ `<input>` cung cấp khả năng tương tác linh hoạt với người dùng.

- [0. Menu](#0-menu)

# 18. `placeholder` (attribute)

Trong HTML, thuộc tính `placeholder` được sử dụng trong các thẻ nhập liệu (như thẻ `<input>` hoặc `<textarea>`) để hiển thị một gợi ý văn bản trong trường nhập liệu khi trường đó chưa được người dùng điền dữ liệu. Văn bản này sẽ biến mất khi người dùng bắt đầu nhập thông tin vào trường.

### **Cấu trúc cơ bản của thuộc tính `placeholder`**

```html
<input type="text" placeholder="Nhập tên người dùng">
```

### **Các thuộc tính và cách sử dụng của `placeholder`**

1. **Thẻ `<input>`**:
   - `placeholder` thường được sử dụng với các trường nhập liệu dạng văn bản (`text`), mật khẩu (`password`), email (`email`), số (`number`), v.v.
   
   Ví dụ:
   ```html
   <input type="text" placeholder="Nhập tên người dùng">
   <input type="password" placeholder="Nhập mật khẩu">
   <input type="email" placeholder="Nhập email của bạn">
   ```

2. **Thẻ `<textarea>`**:
   - `placeholder` cũng có thể được sử dụng với thẻ `<textarea>`, giúp người dùng hiểu họ cần nhập loại dữ liệu gì trong khu vực nhập liệu.
   
   Ví dụ:
   ```html
   <textarea placeholder="Nhập bình luận của bạn"></textarea>
   ```

### **Ví dụ về sử dụng `placeholder` trong một biểu mẫu**

```html
<form action="/submit" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" placeholder="Nhập tên người dùng" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Nhập email của bạn" required><br><br>

  <label for="message">Tin nhắn:</label>
  <textarea id="message" name="message" placeholder="Nhập tin nhắn của bạn"></textarea><br><br>

  <input type="submit" value="Gửi">
</form>
```

### **Lợi ích của việc sử dụng `placeholder`**

1. **Cải thiện trải nghiệm người dùng**: `placeholder` giúp người dùng hiểu được dữ liệu mà họ cần nhập vào trường nhập liệu mà không cần phải xem xét nhãn hay hướng dẫn bên ngoài.
   
2. **Tiết kiệm không gian**: Thay vì sử dụng văn bản hướng dẫn hoặc nhãn dài, bạn có thể sử dụng `placeholder` để cung cấp thông tin ngắn gọn và dễ hiểu trực tiếp trong trường nhập liệu.

### **Lưu ý khi sử dụng `placeholder`**

- **Không thay thế nhãn (`label`)**: Mặc dù `placeholder` giúp cung cấp hướng dẫn, nhưng nó không thay thế cho nhãn (thẻ `<label>`). `label` vẫn rất quan trọng để cải thiện khả năng truy cập và hỗ trợ người dùng sử dụng màn hình đọc.
- **Văn bản `placeholder` sẽ biến mất khi người dùng nhập**: Khi người dùng bắt đầu nhập vào trường, văn bản `placeholder` sẽ biến mất. Vì vậy, bạn không nên sử dụng `placeholder` để chứa thông tin quan trọng mà người dùng cần tham khảo sau này.


Thuộc tính `placeholder` trong HTML là một công cụ hữu ích để cung cấp hướng dẫn ngắn gọn cho người dùng khi nhập liệu vào các trường. Tuy nhiên, cần lưu ý rằng nó không nên thay thế các thẻ `<label>` để đảm bảo tính khả dụng và trải nghiệm người dùng tốt nhất.

- [0. Menu](#0-menu)

# 19. `required` (attribute)

Trong HTML, thuộc tính `required` được sử dụng để yêu cầu người dùng nhập dữ liệu vào một trường nhập liệu trước khi gửi biểu mẫu. Nếu trường có thuộc tính `required` mà người dùng không điền dữ liệu, trình duyệt sẽ hiển thị thông báo lỗi và không cho phép gửi biểu mẫu cho đến khi người dùng điền đầy đủ thông tin.

### **Cấu trúc cơ bản của thuộc tính `required`**

```html
<input type="text" required>
```

### **Các loại thẻ hỗ trợ `required`**

Thuộc tính `required` có thể được áp dụng cho các thẻ nhập liệu sau:

1. **Thẻ `<input>`**:
   - Được sử dụng cho nhiều loại trường nhập liệu như `text`, `email`, `password`, `number`, `date`, v.v.

   Ví dụ:
   ```html
   <input type="text" required placeholder="Nhập tên người dùng">
   <input type="email" required placeholder="Nhập email của bạn">
   <input type="password" required placeholder="Nhập mật khẩu">
   ```

2. **Thẻ `<textarea>`**:
   - `required` có thể được áp dụng cho trường văn bản.

   Ví dụ:
   ```html
   <textarea required placeholder="Nhập bình luận của bạn"></textarea>
   ```

3. **Thẻ `<select>`**:
   - Thuộc tính `required` có thể được sử dụng cho thẻ `<select>` để yêu cầu người dùng chọn một giá trị từ danh sách.

   Ví dụ:
   ```html
   <select required>
     <option value="">Chọn một quốc gia</option>
     <option value="vietnam">Việt Nam</option>
     <option value="usa">Mỹ</option>
   </select>
   ```

### **Ví dụ về sử dụng `required` trong một biểu mẫu**

```html
<form action="/submit" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username" required placeholder="Nhập tên người dùng"><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required placeholder="Nhập email của bạn"><br><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password" required placeholder="Nhập mật khẩu"><br><br>

  <input type="submit" value="Gửi">
</form>
```

### **Lợi ích của thuộc tính `required`**

1. **Cải thiện khả năng nhập liệu**: `required` giúp đảm bảo rằng người dùng không bỏ sót các trường quan trọng trong biểu mẫu.
2. **Xử lý lỗi phía trình duyệt**: Khi người dùng không điền vào trường có `required`, trình duyệt sẽ tự động thông báo lỗi và yêu cầu người dùng nhập thông tin trước khi gửi biểu mẫu.
3. **Tính khả dụng**: Thuộc tính `required` hỗ trợ việc kiểm tra dữ liệu ngay tại phía client mà không cần phải dựa vào JavaScript.

### **Lưu ý khi sử dụng `required`**

- **Không thay thế kiểm tra phía server**: Mặc dù `required` giúp kiểm tra dữ liệu phía client, nhưng bạn vẫn cần kiểm tra lại dữ liệu trên server để đảm bảo tính bảo mật và tránh các lỗ hổng bảo mật.
- **Không có thông báo lỗi tùy chỉnh**: Trình duyệt sẽ tự động hiển thị thông báo lỗi mặc định khi người dùng bỏ qua trường `required`, nhưng bạn không thể tùy chỉnh thông báo lỗi này mà không sử dụng JavaScript.



Thuộc tính `required` là một công cụ đơn giản nhưng hữu ích trong việc yêu cầu người dùng nhập dữ liệu vào các trường quan trọng trong biểu mẫu. Nó giúp cải thiện tính khả dụng và ngăn ngừa việc gửi biểu mẫu thiếu thông tin quan trọng. Tuy nhiên, bạn vẫn nên kết hợp với các kiểm tra phía server để đảm bảo tính bảo mật.

- [0. Menu](#0-menu)

# 20. `<button>` (element)

Thẻ `<button>` trong HTML được sử dụng để tạo ra một nút bấm, cho phép người dùng tương tác với trang web, ví dụ như gửi biểu mẫu, thực hiện một hành động JavaScript, hoặc điều hướng đến một trang khác. Thẻ này linh hoạt và có thể chứa nội dung văn bản, hình ảnh hoặc cả hai.

### **Cấu trúc cơ bản của thẻ `<button>`**

```html
<button>Click me</button>
```

### **Các thuộc tính phổ biến của thẻ `<button>`**

1. **`type`**:
   - Xác định hành động mà nút sẽ thực hiện khi được nhấn.
   - Có ba giá trị phổ biến:
     - `submit`: Nút này sẽ gửi biểu mẫu (mặc định nếu không chỉ định type).
     - `reset`: Nút này sẽ đặt lại tất cả các trường nhập liệu trong biểu mẫu về giá trị mặc định.
     - `button`: Nút này không có hành động mặc định, thường được sử dụng với JavaScript để thực hiện các hành động tùy chỉnh.

   Ví dụ:
   ```html
   <button type="submit">Gửi</button>
   <button type="reset">Đặt lại</button>
   <button type="button" onclick="alert('Bạn đã nhấn nút!')">Nhấn tôi</button>
   ```

2. **`name`** và **`value`**:
   - Thuộc tính `name` và `value` thường được sử dụng khi thẻ `<button>` nằm trong một biểu mẫu. Chúng xác định tên và giá trị của nút khi biểu mẫu được gửi.

   Ví dụ:
   ```html
   <button type="submit" name="action" value="save">Lưu</button>
   ```

3. **`disabled`**:
   - Thuộc tính này vô hiệu hóa nút, khiến nó không thể nhấn được.

   Ví dụ:
   ```html
   <button type="button" disabled>Không thể nhấn</button>
   ```

4. **`autofocus`**:
   - Khi được sử dụng, thuộc tính này tự động chọn nút khi trang được tải.

   Ví dụ:
   ```html
   <button type="button" autofocus>Nhấn tôi đầu tiên</button>
   ```

### **Ví dụ về sử dụng thẻ `<button>` trong một biểu mẫu**

```html
<form action="/submit" method="POST">
  <label for="name">Tên của bạn:</label>
  <input type="text" id="name" name="name"><br><br>

  <button type="submit">Gửi</button>
</form>
```

### **Thẻ `<button>` với JavaScript**

Bạn có thể kết hợp thẻ `<button>` với JavaScript để thực hiện các hành động khi người dùng nhấn nút, như thay đổi nội dung, hiển thị thông báo, hoặc thực hiện các tác vụ động khác.

Ví dụ:
```html
<button type="button" onclick="alert('Chào bạn!')">Nhấn để chào</button>
```

### **Thẻ `<button>` với nội dung phức tạp**

Thẻ `<button>` không chỉ chứa văn bản mà còn có thể chứa hình ảnh hoặc các thẻ HTML khác như `<span>`, giúp làm phong phú nội dung nút.

Ví dụ:
```html
<button type="button">
  <img src="icon.png" alt="Icon"> Nhấn tôi
</button>
```

### **So sánh với thẻ `<input>`**

Thẻ `<button>` và thẻ `<input>` (với type="button") có thể có chức năng tương tự, nhưng thẻ `<button>` linh hoạt hơn vì có thể chứa nội dung HTML phức tạp như hình ảnh hoặc các thẻ con khác.

Thẻ `<button>` trong HTML là một phần tử rất linh hoạt và dễ sử dụng để tạo các nút bấm trong các trang web hoặc biểu mẫu. Bạn có thể kết hợp nó với các hành động JavaScript hoặc các chức năng mặc định của biểu mẫu, như gửi hoặc đặt lại dữ liệu.

- [0. Menu](#0-menu)

# 21. `radio` (attribute)

Thẻ `<input>` với thuộc tính `type="radio"` trong HTML được sử dụng để tạo các nút chọn (radio buttons). Nút radio cho phép người dùng chọn chỉ một giá trị từ một nhóm các lựa chọn. Các nút radio thường được nhóm lại với nhau bằng cách sử dụng cùng một giá trị cho thuộc tính `name`, để đảm bảo rằng chỉ một nút trong nhóm có thể được chọn cùng lúc.

### **Cấu trúc cơ bản của thẻ `<input>` với `type="radio"`**

```html
<input type="radio" name="option" value="1"> Lựa chọn 1
<input type="radio" name="option" value="2"> Lựa chọn 2
<input type="radio" name="option" value="3"> Lựa chọn 3
```

### **Giải thích về các thuộc tính của thẻ `<input type="radio">`**

1. **`name`**:
   - Thuộc tính này nhóm các nút radio lại với nhau. Các nút radio trong cùng một nhóm (cùng giá trị `name`) chỉ cho phép người dùng chọn một lựa chọn duy nhất.

2. **`value`**:
   - Thuộc tính `value` xác định giá trị mà nút radio sẽ gửi khi biểu mẫu được gửi đi.

3. **`checked`**:
   - Thuộc tính `checked` xác định nút radio nào sẽ được chọn mặc định khi trang được tải.

4. **`disabled`**:
   - Thuộc tính `disabled` làm cho nút radio không thể được chọn.

### **Ví dụ về các nút radio trong một biểu mẫu**

```html
<form action="/submit" method="POST">
  <label>
    <input type="radio" name="color" value="red" checked> Đỏ
  </label><br>
  <label>
    <input type="radio" name="color" value="green"> Xanh lá
  </label><br>
  <label>
    <input type="radio" name="color" value="blue"> Xanh dương
  </label><br>
  <input type="submit" value="Gửi">
</form>
```

### **Các tính năng chính của nút radio**

1. **Chỉ một lựa chọn được phép**:
   - Khi người dùng chọn một nút radio trong nhóm, các nút radio khác trong nhóm đó sẽ tự động không được chọn.

2. **Chọn mặc định**:
   - Nếu bạn muốn một nút radio được chọn mặc định khi trang được tải, bạn chỉ cần thêm thuộc tính `checked` vào nút đó.

   Ví dụ:
   ```html
   <input type="radio" name="color" value="red" checked> Đỏ
   ```

3. **Tạo nhóm lựa chọn**:
   - Các nút radio trong cùng một nhóm phải có cùng giá trị `name`, điều này giúp trình duyệt hiểu rằng người dùng chỉ có thể chọn một lựa chọn trong nhóm.

4. **Thêm nhãn (label)**:
   - Thẻ `<label>` có thể được sử dụng để mô tả nút radio, giúp cải thiện khả năng sử dụng và hỗ trợ người dùng dễ dàng chọn lựa hơn.

   Ví dụ:
   ```html
   <label>
     <input type="radio" name="color" value="red"> Đỏ
   </label>
   ```


Thẻ `<input type="radio">` là một phần quan trọng trong việc tạo các lựa chọn đơn trong các biểu mẫu HTML. Nó cho phép người dùng chọn chỉ một giá trị từ một nhóm các lựa chọn, và có thể dễ dàng kết hợp với JavaScript để xử lý các hành động khi người dùng chọn một trong các nút radio.

- [0. Menu](#0-menu)

# 22. `<label>` (semantic element)

Thẻ `<label>` trong HTML được sử dụng để định nghĩa nhãn cho các phần tử nhập liệu trong biểu mẫu, giúp cải thiện khả năng sử dụng và truy cập của người dùng. Khi bạn sử dụng thẻ `<label>`, nó không chỉ mô tả mục đích của các trường nhập liệu mà còn cải thiện khả năng tương tác, đặc biệt là đối với người dùng sử dụng màn hình cảm ứng hoặc công cụ hỗ trợ.

### **Cấu trúc cơ bản của thẻ `<label>`**

```html
<label for="username">Tên người dùng:</label>
<input type="text" id="username" name="username">
```

### **Giải thích các thuộc tính của thẻ `<label>`**

1. **`for`**:
   - Thuộc tính `for` của thẻ `<label>` liên kết nhãn với một phần tử nhập liệu cụ thể trong biểu mẫu. Giá trị của thuộc tính `for` phải trùng với giá trị của thuộc tính `id` của phần tử nhập liệu.
   - Điều này cho phép người dùng nhấp vào nhãn để kích hoạt trường nhập liệu liên quan, giúp cải thiện trải nghiệm người dùng.

2. **Nội dung**:
   - Nội dung của thẻ `<label>` thường là mô tả cho trường nhập liệu, giúp người dùng hiểu họ cần nhập gì vào đó.

### **Ví dụ về thẻ `<label>`**

```html
<form action="/submit" method="POST">
  <label for="username">Tên người dùng:</label>
  <input type="text" id="username" name="username"><br><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password"><br><br>

  <input type="submit" value="Đăng nhập">
</form>
```

### **Lợi ích của thẻ `<label>`**

1. **Tăng khả năng sử dụng**:
   - Khi bạn nhấp vào nhãn, trường nhập liệu tương ứng sẽ được kích hoạt (focus). Điều này giúp người dùng dễ dàng chọn trường nhập liệu mà không cần phải nhấp vào ô nhập liệu chính.
   
2. **Hỗ trợ truy cập**:
   - Thẻ `<label>` giúp cải thiện khả năng truy cập, đặc biệt đối với người dùng sử dụng công cụ hỗ trợ như màn hình đọc cho người khiếm thị. Mô tả rõ ràng về mục đích của trường nhập liệu giúp họ hiểu rõ hơn về các phần tử trên trang.

3. **Cải thiện trải nghiệm người dùng**:
   - Với thẻ `<label>`, bạn có thể tạo ra các giao diện người dùng dễ dàng sử dụng hơn, đặc biệt là trên các thiết bị di động với màn hình cảm ứng. Việc nhấp vào nhãn sẽ giúp người dùng dễ dàng tương tác với trường nhập liệu.

### **Sử dụng thẻ `<label>` với các loại phần tử nhập liệu khác**

Thẻ `<label>` có thể được sử dụng với nhiều loại phần tử nhập liệu khác nhau, chẳng hạn như các nút radio, checkbox, hoặc thậm chí các phần tử chọn lựa (`<select>`).

Ví dụ với thẻ radio:

```html
<label for="male">Nam</label>
<input type="radio" id="male" name="gender" value="male">

<label for="female">Nữ</label>
<input type="radio" id="female" name="gender" value="female">
```

Ví dụ với thẻ checkbox:

```html
<label for="newsletter">Đăng ký nhận bản tin</label>
<input type="checkbox" id="newsletter" name="newsletter">
```


Thẻ `<label>` là một phần quan trọng trong việc tạo ra các biểu mẫu dễ sử dụng và dễ truy cập. Nó giúp cải thiện khả năng tương tác của người dùng, đặc biệt là với các công cụ hỗ trợ như màn hình đọc. Việc sử dụng thẻ `<label>` một cách hợp lý không chỉ mang lại trải nghiệm người dùng tốt hơn mà còn giúp trang web của bạn dễ dàng tuân thủ các nguyên tắc về truy cập web.

- [0. Menu](#0-menu)

# 23. `id` (attribute)

Thuộc tính `id` trong HTML là một thuộc tính quan trọng dùng để gán một định danh duy nhất cho một phần tử trên trang web. Mỗi giá trị `id` phải là duy nhất trong một trang HTML, điều này có nghĩa là không thể có hai phần tử có cùng giá trị `id` trên cùng một trang. Thuộc tính `id` giúp xác định phần tử một cách dễ dàng, giúp dễ dàng truy cập, thao tác và tương tác với các phần tử trong HTML thông qua CSS và JavaScript.

### **Cấu trúc cơ bản của `id`**

```html
<div id="header">Đây là tiêu đề trang</div>
```

### **Các tính năng và lợi ích của `id`**

1. **Xác định phần tử duy nhất**:
   - `id` giúp bạn xác định một phần tử duy nhất trong trang web. Điều này rất hữu ích khi bạn cần thao tác với phần tử đó thông qua CSS hoặc JavaScript.

2. **Tương tác với CSS**:
   - Bạn có thể sử dụng `id` để áp dụng các kiểu CSS riêng biệt cho phần tử đó.

   Ví dụ:
   ```html
   <div id="header">Tiêu đề</div>
   ```

   ```css
   #header {
     color: blue;
     font-size: 24px;
   }
   ```

3. **Tương tác với JavaScript**:
   - JavaScript có thể dễ dàng truy cập và thay đổi phần tử có `id` nhất định bằng cách sử dụng phương thức `getElementById()`.

   Ví dụ:
   ```html
   <div id="header">Tiêu đề</div>
   <button onclick="changeText()">Thay đổi Tiêu đề</button>

   <script>
     function changeText() {
       document.getElementById("header").innerHTML = "Tiêu đề đã thay đổi!";
     }
   </script>
   ```

4. **Dẫn hướng trong trang (Anchor)**:
   - Bạn có thể sử dụng `id` để tạo các liên kết điều hướng đến các phần khác nhau trong trang. Khi người dùng nhấp vào liên kết, trang sẽ cuộn đến phần tử có `id` tương ứng.

   Ví dụ:
   ```html
   <a href="#section1">Đi đến Phần 1</a>

   <div id="section1">
     <h2>Phần 1</h2>
     <p>Đây là phần 1 của trang.</p>
   </div>
   ```

5. **Dễ dàng tích hợp với các thư viện và công cụ**:
   - Các thư viện JavaScript như jQuery và các công cụ khác thường sử dụng `id` để truy cập và thao tác với các phần tử trong DOM.

### **Quy tắc khi sử dụng `id`**

1. **Đảm bảo tính duy nhất**:
   - Giá trị `id` phải là duy nhất trong trang. Bạn không thể sử dụng cùng một `id` cho nhiều phần tử.

2. **Không bắt đầu bằng số**:
   - Mặc dù các giá trị `id` có thể chứa số, nhưng không nên bắt đầu bằng số. Thay vào đó, giá trị `id` nên bắt đầu bằng một chữ cái.

3. **Không sử dụng khoảng trắng**:
   - Tránh sử dụng khoảng trắng trong giá trị của `id`. Nếu cần, bạn có thể sử dụng dấu gạch ngang (`-`) hoặc dấu gạch dưới (`_`) thay vì khoảng trắng.

   Ví dụ đúng:
   ```html
   <div id="main-header"></div>
   <div id="main_header"></div>
   ```

   Ví dụ sai:
   ```html
   <div id="main header"></div> <!-- Không hợp lệ -->
   ```

4. **Chú ý đến chữ hoa và chữ thường**:
   - `id` trong HTML là phân biệt chữ hoa chữ thường. Điều này có nghĩa là `header` và `Header` sẽ được coi là hai giá trị khác nhau.

### **Ví dụ về sử dụng `id` trong HTML**

```html
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ví dụ về ID</title>
  <style>
    #header {
      color: red;
      font-size: 24px;
    }
  </style>
</head>
<body>

  <div id="header">Đây là tiêu đề trang</div>
  <p id="intro">Giới thiệu về trang này.</p>

  <a href="#header">Đi đến Tiêu đề</a>

  <script>
    document.getElementById("header").innerHTML = "Tiêu đề đã được thay đổi!";
  </script>

</body>
</html>
```


Thuộc tính `id` trong HTML là một công cụ mạnh mẽ để xác định các phần tử trên trang web. Nó cho phép bạn áp dụng CSS, truy cập và thay đổi phần tử bằng JavaScript, cũng như điều hướng người dùng đến các phần cụ thể trong trang. Việc sử dụng `id` đúng cách giúp bạn tối ưu hóa trải nghiệm người dùng và dễ dàng quản lý các phần tử trong trang web.

- [0. Menu](#0-menu)

# 24.  `<fieldset>` and `<legend>` (semantic element)

Thẻ `<fieldset>` trong HTML được sử dụng để nhóm các phần tử trong một biểu mẫu (form) lại với nhau, giúp cải thiện tính tổ chức và dễ đọc cho người dùng. Nó tạo ra một khung viền xung quanh nhóm các phần tử, giúp phân tách các phần khác nhau trong biểu mẫu. Thẻ `<fieldset>` thường được sử dụng kết hợp với thẻ `<legend>` để mô tả nhóm các phần tử trong biểu mẫu.

### **Cấu trúc cơ bản của `<fieldset>`**

```html
<fieldset>
  <legend>Thông tin cá nhân</legend>
  <label for="name">Tên:</label>
  <input type="text" id="name" name="name"><br><br>
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
</fieldset>
```

### **Giải thích các phần tử trong ví dụ**

1. **`<fieldset>`**:
   - Thẻ này dùng để nhóm các phần tử nhập liệu trong một biểu mẫu lại với nhau. Nó tạo ra một khung viền bao quanh các phần tử được nhóm.
   
2. **`<legend>`**:
   - Thẻ `<legend>` được sử dụng để mô tả nhóm các phần tử trong `<fieldset>`. Nội dung của thẻ `<legend>` thường là một tiêu đề ngắn gọn cho nhóm đó. Thẻ `<legend>` là tùy chọn nhưng nó giúp người dùng hiểu rõ hơn về các phần tử trong nhóm.

### **Ví dụ đầy đủ về `<fieldset>` và `<legend>`**

```html
<form action="/submit" method="POST">
  <fieldset>
    <legend>Thông tin cá nhân</legend>
    
    <label for="name">Tên:</label>
    <input type="text" id="name" name="name"><br><br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br><br>
    
    <label for="dob">Ngày sinh:</label>
    <input type="date" id="dob" name="dob"><br><br>
  </fieldset>

  <fieldset>
    <legend>Thông tin địa chỉ</legend>
    
    <label for="address">Địa chỉ:</label>
    <input type="text" id="address" name="address"><br><br>
    
    <label for="city">Thành phố:</label>
    <input type="text" id="city" name="city"><br><br>
    
    <label for="postal">Mã bưu điện:</label>
    <input type="text" id="postal" name="postal"><br><br>
  </fieldset>

  <input type="submit" value="Gửi">
</form>
```

### **Lợi ích của việc sử dụng `<fieldset>` và `<legend>`**

1. **Cải thiện tổ chức biểu mẫu**:
   - Việc nhóm các phần tử trong biểu mẫu lại với nhau giúp tổ chức biểu mẫu một cách rõ ràng hơn. Người dùng sẽ dễ dàng nhận ra các nhóm thông tin liên quan đến nhau, ví dụ như nhóm thông tin cá nhân, nhóm thông tin địa chỉ, v.v.

2. **Tăng khả năng truy cập (accessibility)**:
   - Các nhóm thông tin được mô tả bằng thẻ `<legend>` sẽ giúp người dùng, đặc biệt là những người sử dụng công cụ hỗ trợ như màn hình đọc, dễ dàng hiểu được các phần trong biểu mẫu. Công cụ hỗ trợ có thể đọc nội dung của thẻ `<legend>` để người dùng biết phần đó chứa thông tin gì.

3. **Tạo giao diện rõ ràng hơn**:
   - Khung viền được tạo bởi thẻ `<fieldset>` giúp làm nổi bật các nhóm phần tử, làm cho biểu mẫu trở nên dễ nhìn và dễ hiểu hơn.

### **Sử dụng CSS để tùy chỉnh `<fieldset>`**

Bạn có thể sử dụng CSS để thay đổi giao diện của thẻ `<fieldset>`, chẳng hạn như thay đổi màu sắc, đường viền hoặc padding.

Ví dụ:

```html
<style>
  fieldset {
    border: 2px solid #4CAF50;
    padding: 10px;
  }
  legend {
    font-weight: bold;
    color: #4CAF50;
  }
</style>

<fieldset>
  <legend>Thông tin liên hệ</legend>
  <label for="phone">Số điện thoại:</label>
  <input type="text" id="phone" name="phone"><br><br>
</fieldset>
```



Thẻ `<fieldset>` là một công cụ hữu ích trong việc nhóm các phần tử trong biểu mẫu HTML, giúp tăng tính tổ chức và dễ hiểu cho người dùng. Khi kết hợp với thẻ `<legend>`, bạn có thể mô tả rõ ràng các nhóm thông tin trong biểu mẫu. Việc sử dụng thẻ này giúp biểu mẫu của bạn trở nên dễ sử dụng và dễ truy cập hơn, đặc biệt là đối với những người sử dụng công cụ hỗ trợ.

- [0. Menu](#0-menu)

# 25. `checked` (attribute)

Thuộc tính `checked` trong HTML được sử dụng với các phần tử input có loại là `radio` hoặc `checkbox` để xác định xem chúng có được chọn (checked) hay không. Khi thuộc tính `checked` được thêm vào phần tử, nó sẽ được hiển thị là đã chọn khi trang được tải.

### **Cấu trúc của thuộc tính `checked`**

1. **Đối với checkbox**:
   - Thẻ `<input>` với loại `checkbox` cho phép người dùng chọn hoặc bỏ chọn một ô kiểm tra. Thuộc tính `checked` sẽ xác định ô kiểm tra có được chọn khi trang được tải không.

```html
<input type="checkbox" id="accept" name="accept" checked>
<label for="accept">Tôi đồng ý với các điều khoản và điều kiện</label>
```

- Trong ví dụ trên, ô kiểm tra sẽ được chọn sẵn khi trang được tải vì thuộc tính `checked` đã được thêm vào thẻ `<input>`.

2. **Đối với radio button**:
   - Thẻ `<input>` với loại `radio` cho phép người dùng chọn một trong các tùy chọn trong một nhóm. Chỉ một radio button trong nhóm có thể được chọn tại một thời điểm. Thuộc tính `checked` sẽ xác định radio button nào được chọn khi trang được tải.

```html
<input type="radio" id="male" name="gender" value="male" checked>
<label for="male">Nam</label><br>
<input type="radio" id="female" name="gender" value="female">
<label for="female">Nữ</label>
```

- Trong ví dụ trên, radio button "Nam" sẽ được chọn sẵn khi trang được tải vì thuộc tính `checked` đã được thêm vào thẻ `<input>`.

### **Lưu ý về thuộc tính `checked`**

- **Không cần giá trị**: Thuộc tính `checked` không cần có giá trị cụ thể. Chỉ cần thêm thuộc tính này vào thẻ `<input>`, nó sẽ có tác dụng. Ví dụ: `<input type="checkbox" checked>` là đủ để ô checkbox được chọn.
- **Có thể thay đổi bằng JavaScript**: Bạn có thể thay đổi trạng thái của `checked` bằng cách sử dụng JavaScript, ví dụ như để tự động chọn hoặc bỏ chọn các ô checkbox hoặc radio button.

### **Ví dụ với JavaScript**

```html
<input type="checkbox" id="subscribe" name="subscribe">
<label for="subscribe">Đăng ký nhận bản tin</label><br>

<button onclick="toggleCheckbox()">Thay đổi trạng thái</button>

<script>
  function toggleCheckbox() {
    var checkbox = document.getElementById("subscribe");
    checkbox.checked = !checkbox.checked; // Đảo ngược trạng thái của checkbox
  }
</script>
```

- Trong ví dụ này, khi người dùng nhấp vào nút, trạng thái của checkbox sẽ thay đổi từ được chọn sang không được chọn và ngược lại.


Thuộc tính `checked` là một công cụ quan trọng trong HTML giúp xác định trạng thái ban đầu của các phần tử checkbox và radio button trong biểu mẫu. Nó cho phép bạn dễ dàng xác định các lựa chọn mặc định và có thể được thay đổi động thông qua JavaScript.

- [0. Menu](#0-menu)

# 26. `<header>` (semantic element)

Thẻ `<header>` trong HTML được sử dụng để định nghĩa phần đầu trang của một tài liệu hoặc một phần của tài liệu. Thông thường, thẻ này chứa các yếu tố quan trọng như tiêu đề, logo, menu điều hướng, hoặc các thông tin khác giúp người dùng dễ dàng nhận diện và điều hướng trong trang web. Thẻ `<header>` giúp tổ chức và phân chia nội dung của trang web một cách rõ ràng.

### **Cấu trúc cơ bản của thẻ `<header>`**

```html
<header>
  <h1>Chào mừng đến với trang web của chúng tôi!</h1>
  <nav>
    <ul>
      <li><a href="#home">Trang chủ</a></li>
      <li><a href="#about">Giới thiệu</a></li>
      <li><a href="#services">Dịch vụ</a></li>
      <li><a href="#contact">Liên hệ</a></li>
    </ul>
  </nav>
</header>
```

### **Giải thích các phần trong ví dụ:**

1. **`<header>`**:
   - Thẻ `<header>` định nghĩa phần đầu trang của tài liệu hoặc một phần của tài liệu. Nó có thể chứa nhiều loại nội dung khác nhau, chẳng hạn như tiêu đề, logo, thanh điều hướng, v.v.

2. **Tiêu đề chính (`<h1>`)**:
   - Thẻ `<h1>` chứa tiêu đề chính của trang web, giúp người dùng dễ dàng nhận diện trang web.

3. **Thanh điều hướng (`<nav>`)**:
   - Thẻ `<nav>` được sử dụng để nhóm các liên kết điều hướng của trang web lại với nhau. Đây thường là nơi chứa các menu hoặc liên kết quan trọng, giúp người dùng dễ dàng di chuyển giữa các phần khác nhau của trang web.

4. **Danh sách liên kết (`<ul>`, `<li>`, `<a>`)**:
   - Các liên kết điều hướng thường được nhóm trong một danh sách không có thứ tự (`<ul>`), và mỗi mục trong danh sách được tạo bằng thẻ `<li>`. Các liên kết được tạo bằng thẻ `<a>` với thuộc tính `href` chỉ định đích đến.

### **Các nội dung thường có trong thẻ `<header>`**

Thẻ `<header>` có thể chứa nhiều yếu tố khác nhau, chẳng hạn như:

1. **Logo**:
   - Thường chứa logo của trang web hoặc công ty, giúp người dùng nhận diện thương hiệu.

2. **Tiêu đề trang**:
   - Tiêu đề chính của trang web hoặc phần của trang web, thường được đặt trong thẻ `<h1>` hoặc các thẻ tiêu đề khác.

3. **Thanh điều hướng**:
   - Một thanh điều hướng hoặc menu chứa các liên kết đến các phần quan trọng của trang web.

4. **Thông tin tìm kiếm**:
   - Một ô tìm kiếm hoặc các công cụ tìm kiếm giúp người dùng tìm kiếm nội dung trên trang web.

5. **Các liên kết mạng xã hội**:
   - Các biểu tượng hoặc liên kết đến các trang mạng xã hội của trang web.

### **Ví dụ về cách sử dụng thẻ `<header>`**

```html
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trang web ví dụ</title>
</head>
<body>

  <header>
    <img src="logo.png" alt="Logo Công ty" width="100">
    <h1>Chào mừng đến với công ty ABC</h1>
    <nav>
      <ul>
        <li><a href="#home">Trang chủ</a></li>
        <li><a href="#about">Giới thiệu</a></li>
        <li><a href="#services">Dịch vụ</a></li>
        <li><a href="#contact">Liên hệ</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <p>Đây là nội dung chính của trang web.</p>
  </main>

</body>
</html>
```

### **Sử dụng CSS để tùy chỉnh thẻ `<header>`**

Bạn có thể sử dụng CSS để thay đổi giao diện của phần đầu trang, chẳng hạn như thay đổi màu nền, căn chỉnh các phần tử hoặc tạo các hiệu ứng đặc biệt.

```html
<style>
  header {
    background-color: #4CAF50;
    color: white;
    padding: 20px;
    text-align: center;
  }

  header nav ul {
    list-style-type: none;
    padding: 0;
  }

  header nav ul li {
    display: inline;
    margin-right: 15px;
  }

  header nav ul li a {
    color: white;
    text-decoration: none;
  }

  header nav ul li a:hover {
    text-decoration: underline;
  }
</style>

<header>
  <h1>Chào mừng đến với công ty ABC</h1>
  <nav>
    <ul>
      <li><a href="#home">Trang chủ</a></li>
      <li><a href="#about">Giới thiệu</a></li>
      <li><a href="#services">Dịch vụ</a></li>
      <li><a href="#contact">Liên hệ</a></li>
    </ul>
  </nav>
</header>
```

Thẻ `<header>` là một phần quan trọng trong việc xây dựng cấu trúc trang web, giúp cung cấp thông tin về trang web, điều hướng người dùng và tăng khả năng sử dụng của trang. Thẻ này có thể chứa nhiều loại nội dung khác nhau như tiêu đề, logo, menu điều hướng, và các công cụ tìm kiếm. Sử dụng thẻ `<header>` giúp làm cho trang web của bạn trở nên dễ dàng điều hướng và dễ hiểu hơn đối với người dùng.

- [0. Menu](#0-menu)

# 27. `<footer>` (semantic element)

Thẻ `<footer>` trong HTML được sử dụng để định nghĩa phần chân trang của một tài liệu hoặc một phần trong tài liệu. Thông thường, thẻ `<footer>` chứa thông tin bổ sung về trang web, chẳng hạn như bản quyền, liên kết đến các trang chính sách, thông tin liên hệ, hoặc các liên kết mạng xã hội. Thẻ này có thể xuất hiện một lần trong tài liệu, hoặc có thể xuất hiện nhiều lần trong các phần khác nhau của tài liệu.

### **Cấu trúc cơ bản của thẻ `<footer>`**

```html
<footer>
  <p>© 2025 Công ty ABC. Mọi quyền được bảo lưu.</p>
  <ul>
    <li><a href="#about">Giới thiệu</a></li>
    <li><a href="#contact">Liên hệ</a></li>
    <li><a href="#privacy">Chính sách bảo mật</a></li>
  </ul>
</footer>
```

### **Giải thích các phần trong ví dụ:**

1. **`<footer>`**:
   - Đây là thẻ chứa phần chân trang của tài liệu hoặc phần tử chứa nó. Thông thường, thẻ này sẽ nằm ở cuối trang hoặc phần của trang, nhưng bạn có thể đặt nó ở bất kỳ đâu trong tài liệu.

2. **Thông tin bản quyền**:
   - Thông tin bản quyền như `© 2025 Công ty ABC. Mọi quyền được bảo lưu.` thường được đặt trong thẻ `<footer>` để cho biết quyền sở hữu nội dung trên trang web.

3. **Liên kết điều hướng**:
   - Các liên kết như "Giới thiệu", "Liên hệ", "Chính sách bảo mật" có thể được đặt trong thẻ `<ul>` (danh sách không có thứ tự) và mỗi mục trong danh sách được tạo bằng thẻ `<li>` (mục danh sách) với các thẻ `<a>` chứa liên kết.

### **Thẻ `<footer>` có thể chứa gì?**

Thẻ `<footer>` có thể chứa nhiều loại nội dung khác nhau, chẳng hạn như:

1. **Thông tin bản quyền**:
   - Thông tin về quyền sở hữu trí tuệ hoặc bản quyền của trang web.

2. **Liên kết đến các trang chính sách**:
   - Các liên kết như "Chính sách bảo mật", "Điều khoản sử dụng", hoặc "Chính sách cookie".

3. **Thông tin liên hệ**:
   - Địa chỉ, số điện thoại, hoặc liên kết đến các phương thức liên hệ với chủ sở hữu trang web.

4. **Liên kết mạng xã hội**:
   - Các liên kết đến các mạng xã hội như Facebook, Twitter, LinkedIn, Instagram, v.v.

5. **Các thông tin bổ sung khác**:
   - Ví dụ: thông tin về công ty, bản đồ trang web, hoặc các liên kết đến các tài liệu hoặc dịch vụ khác.

### **Ví dụ về cách sử dụng `<footer>` trong một trang web**

```html
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trang web ví dụ</title>
</head>
<body>

  <header>
    <h1>Chào mừng đến với trang web của chúng tôi!</h1>
  </header>

  <main>
    <p>Đây là nội dung chính của trang web.</p>
  </main>

  <footer>
    <p>© 2025 Công ty ABC. Mọi quyền được bảo lưu.</p>
    <ul>
      <li><a href="#about">Giới thiệu</a></li>
      <li><a href="#contact">Liên hệ</a></li>
      <li><a href="#privacy">Chính sách bảo mật</a></li>
    </ul>
  </footer>

</body>
</html>
```

### **Sử dụng CSS để tùy chỉnh thẻ `<footer>`**

Bạn có thể sử dụng CSS để thay đổi kiểu dáng của phần chân trang. Ví dụ, bạn có thể thay đổi màu nền, căn chỉnh văn bản, hoặc tạo một khoảng cách nhất định giữa phần chân trang và các phần khác trên trang.

```html
<style>
  footer {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
  }

  footer a {
    color: #ffcc00;
    text-decoration: none;
  }

  footer a:hover {
    text-decoration: underline;
  }
</style>
```

Thẻ `<footer>` là một phần quan trọng trong việc xây dựng cấu trúc trang web. Nó giúp cung cấp thông tin bổ sung cho người dùng và cải thiện khả năng điều hướng của trang web. Mặc dù nó thường xuất hiện ở cuối trang, bạn có thể sử dụng thẻ `<footer>` ở bất kỳ đâu trong tài liệu, đặc biệt là khi bạn muốn nhóm các thông tin bổ sung lại với nhau.

- [0. Menu](#0-menu)

# 28. `html:5` (HTML5 template)

`html:5` là một phím tắt được sử dụng trong một số trình soạn thảo mã nguồn (ví dụ như Visual Studio Code) để tạo ra một cấu trúc HTML5 cơ bản một cách nhanh chóng. Khi bạn nhập `html:5` và nhấn **Tab**, trình soạn thảo sẽ tự động tạo ra một mẫu HTML5 chuẩn.

Dưới đây là chi tiết về các phần và thẻ trong template HTML5 được tạo ra từ phím tắt `html:5`.

### Cấu trúc mẫu HTML5

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>

</body>
</html>
```

### Giải thích chi tiết các thẻ trong template HTML5:

1. **`<!DOCTYPE html>`**
   - **Mô tả**: Khai báo loại tài liệu (document type declaration). Dòng này cho trình duyệt biết rằng tài liệu HTML này sử dụng chuẩn HTML5.
   - **Lý do sử dụng**: Việc khai báo `<!DOCTYPE html>` giúp trình duyệt biết rằng đây là một tài liệu HTML5, giúp nó hiển thị chính xác nội dung trang web.
   
2. **`<html lang="en">`**
   - **Mô tả**: Thẻ `<html>` mở đầu tài liệu HTML và đóng lại ở cuối trang. Thuộc tính `lang="en"` chỉ định ngôn ngữ của trang là tiếng Anh.
   - **Lý do sử dụng**: Thuộc tính `lang` giúp công cụ tìm kiếm và trình duyệt nhận diện ngôn ngữ của trang web, từ đó hỗ trợ trong việc hiển thị nội dung và tối ưu hóa công cụ tìm kiếm (SEO).
   - **Lưu ý**: Bạn có thể thay đổi `en` thành mã ngôn ngữ khác nếu cần, ví dụ: `vi` cho tiếng Việt.

3. **`<head>`**
   - **Mô tả**: Phần đầu của tài liệu HTML, chứa các thẻ meta, liên kết đến tệp CSS, và các tài nguyên khác.
   - **Lý do sử dụng**: Thẻ `<head>` không hiển thị trực tiếp trên trang web, nhưng chứa các thông tin quan trọng cho trình duyệt và các công cụ tìm kiếm.
   
4. **`<meta charset="UTF-8">`**
   - **Mô tả**: Đảm bảo rằng tài liệu sử dụng mã hóa ký tự UTF-8, cho phép trang web hiển thị được hầu hết các ký tự quốc tế (bao gồm các ký tự đặc biệt và ngôn ngữ không phải tiếng Anh).
   - **Lý do sử dụng**: Đảm bảo trang web có thể hiển thị đúng các ký tự, bao gồm cả các ngôn ngữ khác như tiếng Việt, tiếng Trung, tiếng Nhật, v.v.

5. **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**
   - **Mô tả**: Thiết lập viewport cho trang web, điều này rất quan trọng để trang web hiển thị đúng trên các thiết bị di động.
   - **Lý do sử dụng**: Khi sử dụng `width=device-width`, bạn yêu cầu trình duyệt điều chỉnh chiều rộng của trang để phù hợp với kích thước màn hình của thiết bị. `initial-scale=1.0` thiết lập tỷ lệ ban đầu của trang.
   - **Lưu ý**: Đây là phần quan trọng khi thiết kế trang web đáp ứng (responsive design).

6. **`<meta http-equiv="X-UA-Compatible" content="ie=edge">`**
   - **Mô tả**: Đảm bảo rằng trang web được hiển thị đúng trên các phiên bản cũ của Internet Explorer.
   - **Lý do sử dụng**: Nếu người dùng đang sử dụng một phiên bản cũ của Internet Explorer (IE), thẻ này sẽ yêu cầu trình duyệt sử dụng chế độ "edge" để đảm bảo tính tương thích.

7. **`<title>`**
   - **Mô tả**: Tiêu đề của trang web, xuất hiện trên tab của trình duyệt.
   - **Lý do sử dụng**: Tiêu đề giúp người dùng nhận diện trang web khi họ mở nhiều tab. Nó cũng là yếu tố quan trọng trong SEO, giúp các công cụ tìm kiếm xác định nội dung của trang.

8. **`<body>`**
   - **Mô tả**: Phần thân của tài liệu HTML, nơi chứa tất cả nội dung hiển thị trên trang web, bao gồm văn bản, hình ảnh, liên kết, và các phần tử khác.
   - **Lý do sử dụng**: Đây là phần quan trọng nhất của trang web, nơi bạn thêm nội dung và các phần tử tương tác cho người dùng.
   - **Lưu ý**: Mọi thứ mà người dùng nhìn thấy trên trang web đều được đặt trong thẻ `<body>`.

### Tóm tắt các thẻ trong template `html:5`:

1. **`<!DOCTYPE html>`**: Khai báo tài liệu HTML5.
2. **`<html lang="en">`**: Mở đầu tài liệu HTML, xác định ngôn ngữ của trang.
3. **`<head>`**: Chứa thông tin không hiển thị trực tiếp trên trang web (metadata, CSS, JS).
4. **`<meta charset="UTF-8">`**: Thiết lập mã hóa ký tự UTF-8.
5. **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**: Thiết lập viewport cho thiết bị di động.
6. **`<meta http-equiv="X-UA-Compatible" content="ie=edge">`**: Đảm bảo tương thích với các phiên bản IE cũ.
7. **`<title>`**: Tiêu đề của trang web, xuất hiện trên tab trình duyệt.
8. **`<body>`**: Chứa nội dung chính của trang web.

### Lợi ích của việc sử dụng `html:5`:

- **Tiết kiệm thời gian**: Bạn không cần phải gõ lại cấu trúc HTML5 cơ bản mỗi khi bắt đầu một dự án.
- **Chuẩn hóa**: Đảm bảo rằng tất cả các trang của bạn đều bắt đầu với cấu trúc HTML5 hợp lệ.
- **Dễ dàng mở rộng**: Sau khi có template cơ bản, bạn có thể nhanh chóng thêm nội dung vào thẻ `<body>` và xây dựng trang web của mình.

Template `html:5` giúp bạn tạo một trang web với cấu trúc chuẩn ngay từ đầu, giảm thiểu lỗi và giúp quá trình phát triển trở nên dễ dàng và nhanh chóng hơn.

- [0. Menu](#0-menu)

# 29. `<meta>` (metadata)

Thẻ `<meta>` trong HTML là một thẻ đặc biệt được sử dụng để cung cấp các thông tin (metadata) về tài liệu HTML. Những thông tin này không hiển thị trực tiếp trên trang web nhưng lại rất quan trọng đối với các công cụ tìm kiếm, trình duyệt và các dịch vụ web khác.

### Cấu trúc cơ bản của thẻ `<meta>`

```html
<meta name="name_of_meta_tag" content="value">
```

- **`name`**: Xác định loại thông tin mà thẻ `<meta>` cung cấp (ví dụ: từ khóa, mô tả trang, tác giả).
- **`content`**: Chứa giá trị của thông tin được cung cấp.

### Các loại thẻ `<meta>` phổ biến

1. **Thẻ `<meta charset>`**
   - **Mô tả**: Định nghĩa mã hóa ký tự của trang web.
   - **Cú pháp**: 
     ```html
     <meta charset="UTF-8">
     ```
   - **Lý do sử dụng**: Giúp trình duyệt hiểu cách giải mã và hiển thị các ký tự trong trang. `UTF-8` là mã hóa ký tự phổ biến nhất và hỗ trợ nhiều ngôn ngữ khác nhau.

2. **Thẻ `<meta name="viewport">`**
   - **Mô tả**: Cung cấp thông tin về cách trang web nên hiển thị trên các thiết bị di động và máy tính bảng.
   - **Cú pháp**: 
     ```html
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     ```
   - **Lý do sử dụng**: Điều chỉnh tỷ lệ và chiều rộng của trang web cho phù hợp với các màn hình có kích thước khác nhau, giúp trang web trở nên đáp ứng (responsive) trên các thiết bị di động.

3. **Thẻ `<meta name="description">`**
   - **Mô tả**: Cung cấp mô tả ngắn gọn về nội dung của trang web.
   - **Cú pháp**:
     ```html
     <meta name="description" content="Đây là một mô tả về trang web của tôi.">
     ```
   - **Lý do sử dụng**: Mô tả này sẽ được hiển thị trong kết quả tìm kiếm của các công cụ tìm kiếm (như Google) và giúp người dùng hiểu về nội dung của trang web. Mô tả ngắn gọn và hấp dẫn có thể giúp cải thiện tỷ lệ nhấp (CTR).

4. **Thẻ `<meta name="keywords">`**
   - **Mô tả**: Cung cấp các từ khóa mô tả nội dung của trang web.
   - **Cú pháp**:
     ```html
     <meta name="keywords" content="HTML, CSS, JavaScript, Web Development">
     ```
   - **Lý do sử dụng**: Trước đây, từ khóa được sử dụng nhiều trong SEO, tuy nhiên, hiện nay vai trò của nó đã giảm do các công cụ tìm kiếm đã thay đổi cách thức xếp hạng trang web.

5. **Thẻ `<meta name="author">`**
   - **Mô tả**: Xác định tác giả của trang web.
   - **Cú pháp**:
     ```html
     <meta name="author" content="Tên tác giả">
     ```
   - **Lý do sử dụng**: Cung cấp thông tin về người tạo ra trang web, hữu ích khi cần ghi nhận quyền sở hữu nội dung.

6. **Thẻ `<meta http-equiv="X-UA-Compatible">`**
   - **Mô tả**: Cung cấp thông tin về cách trang web nên hiển thị trong các trình duyệt cũ, đặc biệt là Internet Explorer.
   - **Cú pháp**:
     ```html
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     ```
   - **Lý do sử dụng**: Đảm bảo rằng trang web được hiển thị đúng trên các phiên bản cũ của Internet Explorer, yêu cầu trình duyệt sử dụng chế độ "edge" (mới nhất).

7. **Thẻ `<meta name="robots">`**
   - **Mô tả**: Điều khiển cách các công cụ tìm kiếm thu thập và lập chỉ mục trang web.
   - **Cú pháp**:
     ```html
     <meta name="robots" content="index, follow">
     ```
   - **Lý do sử dụng**: Thẻ này giúp bạn kiểm soát liệu trang web của bạn có được các công cụ tìm kiếm lập chỉ mục hay không và liệu các liên kết trên trang có được theo dõi hay không.

### Ví dụ về các thẻ `<meta>` trong trang HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Trang web của tôi là nơi chia sẻ kiến thức về lập trình web.">
  <meta name="keywords" content="HTML, CSS, JavaScript, lập trình web">
  <meta name="author" content="Nguyễn Văn A">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <title>Trang Web Lập Trình</title>
</head>
<body>
  <h1>Chào mừng đến với trang web lập trình của tôi!</h1>
</body>
</html>
```

### Tóm tắt các thuộc tính chính của thẻ `<meta>`:

- **`charset`**: Định nghĩa mã hóa ký tự (thường là `UTF-8`).
- **`name="viewport"`**: Thiết lập chế độ hiển thị trên thiết bị di động.
- **`name="description"`**: Cung cấp mô tả ngắn gọn về nội dung của trang.
- **`name="keywords"`**: Cung cấp danh sách các từ khóa mô tả trang web.
- **`name="author"`**: Chỉ định tác giả của trang web.
- **`http-equiv="X-UA-Compatible"`**: Đảm bảo tương thích với trình duyệt cũ (Internet Explorer).
- **`name="robots"`**: Điều khiển cách công cụ tìm kiếm lập chỉ mục trang web.

### Lợi ích của thẻ `<meta>`:

- **SEO (Tối ưu hóa công cụ tìm kiếm)**: Thẻ `<meta>` giúp cải thiện khả năng xuất hiện của trang web trên các công cụ tìm kiếm thông qua các mô tả và từ khóa chính xác.
- **Hiển thị trang trên các thiết bị di động**: Thẻ `<meta name="viewport">` rất quan trọng để trang web hiển thị tốt trên các thiết bị di động.
- **Tương thích với các trình duyệt cũ**: Thẻ `<meta http-equiv="X-UA-Compatible">` giúp đảm bảo trang web hoạt động tốt trên các trình duyệt cũ, đặc biệt là Internet Explorer.

Thẻ `<meta>` là một phần không thể thiếu trong việc tối ưu hóa và cấu hình trang web của bạn, giúp nó hoạt động tốt trên các trình duyệt và công cụ tìm kiếm.

- [0. Menu](#0-menu)

# 30. `<link>` (link document)

Thẻ `<link>` trong HTML là một thẻ không có nội dung và được sử dụng để liên kết tài liệu HTML với các tài nguyên bên ngoài, chẳng hạn như tệp CSS, tệp biểu tượng (favicon), hoặc các tài nguyên khác. Thẻ `<link>` thường được đặt trong phần `<head>` của tài liệu HTML.

### Cấu trúc cơ bản của thẻ `<link>`

```html
<link rel="relationship" href="URL" type="MIME-type" />
```

- **`rel`**: Xác định loại mối quan hệ giữa tài liệu hiện tại và tài nguyên được liên kết. Đây là thuộc tính bắt buộc.
- **`href`**: Chỉ định đường dẫn (URL) đến tài nguyên mà bạn muốn liên kết. Đây cũng là thuộc tính bắt buộc.
- **`type`**: Xác định kiểu MIME của tài nguyên. Đây là thuộc tính tùy chọn, thường được sử dụng khi liên kết đến tệp CSS, chẳng hạn như `text/css`.
- **`media`**: Xác định loại thiết bị hoặc điều kiện hiển thị cho tài nguyên được liên kết, ví dụ như chỉ áp dụng cho màn hình rộng, thiết bị di động, v.v. Thuộc tính này cũng tùy chọn.

### Các ví dụ phổ biến về thẻ `<link>`

1. **Liên kết đến tệp CSS**
   - Thẻ `<link>` thường được sử dụng để liên kết đến tệp CSS ngoài.
   - **Cú pháp**:
     ```html
     <link rel="stylesheet" href="styles.css">
     ```
   - **Giải thích**: Thẻ này liên kết tệp CSS (`styles.css`) vào trang HTML, giúp định kiểu cho trang web.

2. **Liên kết đến favicon (biểu tượng trang web)**
   - **Cú pháp**:
     ```html
     <link rel="icon" href="favicon.ico" type="image/x-icon">
     ```
   - **Giải thích**: Thẻ này liên kết một tệp hình ảnh (ví dụ: `favicon.ico`) với trang web để hiển thị biểu tượng trên tab của trình duyệt.

3. **Liên kết đến một tệp web app manifest**
   - **Cú pháp**:
     ```html
     <link rel="manifest" href="manifest.json">
     ```
   - **Giải thích**: Thẻ này liên kết đến một tệp `manifest.json`, chứa thông tin về ứng dụng web (như tên, biểu tượng, màu sắc) khi người dùng thêm trang web vào màn hình chính trên thiết bị di động.

4. **Liên kết đến tệp font từ Google Fonts**
   - **Cú pháp**:
     ```html
     <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto&display=swap">
     ```
   - **Giải thích**: Thẻ này liên kết đến tệp CSS từ Google Fonts, cho phép sử dụng font chữ "Roboto" trên trang web.

5. **Liên kết đến một tệp RSS feed**
   - **Cú pháp**:
     ```html
     <link rel="alternate" type="application/rss+xml" href="rss_feed.xml">
     ```
   - **Giải thích**: Thẻ này chỉ định một tệp RSS feed (`rss_feed.xml`), cho phép người dùng đăng ký theo dõi trang web qua RSS.

### Thuộc tính của thẻ `<link>`

1. **`rel`** (relationship): Xác định loại mối quan hệ giữa tài liệu HTML và tài nguyên liên kết. Một số giá trị phổ biến:
   - `stylesheet`: Liên kết đến tệp CSS.
   - `icon`: Liên kết đến biểu tượng (favicon).
   - `manifest`: Liên kết đến tệp manifest của ứng dụng web.
   - `alternate`: Liên kết đến một phiên bản thay thế của tài liệu, chẳng hạn như tệp RSS.
   - `preload`: Liên kết đến tài nguyên cần tải trước để tối ưu hóa hiệu suất trang.

2. **`href`** (hyperlink reference): Chỉ định URL của tài nguyên mà bạn muốn liên kết.

3. **`type`** (MIME type): Xác định loại MIME của tài nguyên liên kết. Thường được sử dụng khi liên kết đến các tệp có kiểu dữ liệu cụ thể như CSS, JavaScript, hoặc hình ảnh.
   - Ví dụ: `type="text/css"` cho tệp CSS.

4. **`media`**: Xác định loại thiết bị hoặc điều kiện hiển thị tài nguyên liên kết. Ví dụ, có thể chỉ áp dụng cho màn hình di động hoặc màn hình rộng.
   - Ví dụ: `media="screen"` hoặc `media="print"`.

### Ví dụ về sử dụng thẻ `<link>` trong HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trang Web Của Tôi</title>
  
  <!-- Liên kết đến tệp CSS -->
  <link rel="stylesheet" href="styles.css">
  
  <!-- Liên kết đến favicon -->
  <link rel="icon" href="favicon.ico" type="image/x-icon">
  
  <!-- Liên kết đến tệp font từ Google Fonts -->
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto&display=swap">
  
  <!-- Liên kết đến tệp web app manifest -->
  <link rel="manifest" href="manifest.json">
</head>
<body>
  <h1>Chào mừng đến với trang web của tôi!</h1>
</body>
</html>
```

### Tóm tắt các thuộc tính của thẻ `<link>`:

- **`rel`**: Xác định mối quan hệ giữa tài liệu và tài nguyên liên kết (ví dụ: `stylesheet`, `icon`, `manifest`).
- **`href`**: Đường dẫn đến tài nguyên.
- **`type`**: Xác định loại MIME của tài nguyên.
- **`media`**: Chỉ định điều kiện hiển thị của tài nguyên (ví dụ: `screen`, `print`).

### Lợi ích của thẻ `<link>`:

- **Liên kết tài nguyên bên ngoài**: Thẻ `<link>` giúp liên kết các tài nguyên như tệp CSS, biểu tượng trang web, và tệp manifest một cách dễ dàng, giúp cải thiện trải nghiệm người dùng và tối ưu hóa hiệu suất trang web.
- **Quản lý tài nguyên hiệu quả**: Việc sử dụng thẻ `<link>` cho phép bạn quản lý các tài nguyên bên ngoài một cách linh hoạt và dễ dàng thay đổi mà không cần thay đổi nội dung của tài liệu HTML.
- **Tối ưu hóa SEO và trải nghiệm người dùng**: Các tài nguyên như favicon, font chữ và tệp manifest giúp cải thiện giao diện người dùng và tương tác với trang web.

- [0. Menu](#0-menu)

# 31. `<style>` (CSS element)

Thẻ `<style>` trong HTML được sử dụng để viết các quy tắc CSS trực tiếp trong tài liệu HTML. Các quy tắc này thường được đặt trong phần `<head>` của tài liệu để định dạng và thiết kế các phần tử HTML.

### Cú pháp cơ bản:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thẻ Style</title>
    <style>
        /* CSS viết trong đây */
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
        }

        h1 {
            color: #333;
            text-align: center;
        }

        p {
            color: #555;
            line-height: 1.6;
            margin: 10px 20px;
        }
    </style>
</head>
<body>
    <h1>Đây là thẻ style</h1>
    <p>CSS được định nghĩa trong thẻ <code>&lt;style&gt;</code>.</p>
</body>
</html>
```

### Đặc điểm:
1. **Vị trí**:
   - Thường nằm trong phần `<head>`.
   - Có thể đặt trong `<body>` nhưng không khuyến khích.

2. **Ứng dụng**:
   - Dùng để định nghĩa các quy tắc CSS cho trang HTML.
   - Dễ dàng chỉnh sửa và kiểm tra các quy tắc CSS trong một tệp HTML duy nhất.

3. **Ưu và nhược điểm**:
   - **Ưu điểm**:
     - Dễ triển khai khi chỉ làm việc trên một tệp HTML.
   - **Nhược điểm**:
     - Khó quản lý khi làm việc với nhiều tệp HTML.
     - Không tối ưu khi cần sử dụng chung các quy tắc CSS.

# 32. `<article>` (semantic element)

Thẻ `<article>` trong HTML được sử dụng để đánh dấu một phần nội dung độc lập, có thể tái sử dụng hoặc phân phối lại, như bài viết, tin tức, hoặc nội dung blog. Mục đích của thẻ này là để xác định một khối nội dung có thể tồn tại độc lập và được hiểu như một đơn vị thông tin riêng biệt.

### Thuộc tính của thẻ `<article>`:
- **Không có thuộc tính đặc biệt** trong HTML5.
- Tuy nhiên, thẻ này có thể chứa các phần tử như tiêu đề, đoạn văn, hình ảnh, video, liên kết, v.v.

### Ví dụ sử dụng thẻ `<article>` trong HTML và CSS:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Article Example</title>
    <style>
        article {
            background-color: #f4f4f4;
            padding: 20px;
            margin: 10px 0;
            border: 1px solid #ddd;
        }
        article h2 {
            color: #333;
        }
        article p {
            color: #555;
        }
    </style>
</head>
<body>

    <article>
        <h2>Exploring the World of CSS</h2>
        <p>CSS (Cascading Style Sheets) is a powerful tool for designing and styling web pages. In this article, we explore its core concepts and properties.</p>
    </article>

</body>
</html>
```

### Giải thích:
- Thẻ `<article>` bao gồm một bài viết với tiêu đề `<h2>` và một đoạn văn `<p>`.
- CSS trong phần `<style>` định dạng cho thẻ `<article>`, bao gồm màu nền, đệm, lề, và viền. Các phần tử trong thẻ `<article>` như tiêu đề và đoạn văn cũng được định dạng.

Thẻ `<article>` rất hữu ích khi bạn muốn đánh dấu các phần nội dung có thể được chia sẻ hoặc tái sử dụng, như bài viết trên blog, bài báo tin tức, hay các phần trong diễn đàn.

- [0. Menu](#0-menu)

# 33. `<div>` (semantic element)

Thẻ `<div>` trong HTML là một phần tử khối (block-level element) được sử dụng để nhóm các phần tử khác lại với nhau, nhằm mục đích áp dụng các kiểu dáng (CSS) hoặc xử lý bằng JavaScript. Thẻ `<div>` không có ý nghĩa cụ thể về nội dung, nó chỉ đóng vai trò như một khối chứa, giúp cấu trúc và tổ chức trang web.

### Thuộc tính của thẻ `<div>`:
- **Không có thuộc tính đặc biệt** trong HTML5, nhưng bạn có thể sử dụng các thuộc tính như `id`, `class`, `style` để định danh và áp dụng các kiểu dáng.
  
### Ví dụ sử dụng thẻ `<div>` trong HTML và CSS:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Div Example</title>
    <style>
        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
            background-color: #f0f0f0;
        }
        .box {
            width: 100px;
            height: 100px;
            background-color: #3498db;
            margin: 10px;
            display: inline-block;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome to My Website</h1>
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
    </div>

</body>
</html>
```

### Giải thích:
- Thẻ `<div class="container">` là một thẻ bao bọc chứa toàn bộ nội dung của trang.
- Thẻ `<div class="box">` được sử dụng để tạo ra các khối nhỏ có kích thước và màu sắc cụ thể, chúng được nhóm lại trong phần tử chứa `.container`.
- CSS được áp dụng để tạo kiểu cho thẻ `<div>`, ví dụ như: chiều rộng, chiều cao, màu nền, khoảng cách giữa các phần tử.

### Khi nào sử dụng thẻ `<div>`:
- **Tạo cấu trúc trang web**: Bạn có thể sử dụng thẻ `<div>` để chia nhỏ và sắp xếp các phần khác nhau của trang, như header, footer, sidebar, hoặc nội dung chính.
- **Áp dụng CSS hoặc JavaScript**: Khi bạn cần nhóm các phần tử lại với nhau để áp dụng kiểu dáng chung hoặc xử lý bằng JavaScript.

Thẻ `<div>` không mang bất kỳ ý nghĩa nội dung nào (không như thẻ `<article>`, `<section>`, hoặc `<header>`), vì vậy nó chỉ là công cụ để tổ chức và tạo cấu trúc cho trang web.

- [0. Menu](#0-menu)



### Lưu ý:
- Với các dự án lớn, nên sử dụng tệp CSS riêng (external CSS) để tách biệt mã HTML và CSS.

- [0. Menu](#0-menu)
