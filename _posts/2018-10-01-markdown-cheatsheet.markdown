---
layout: post
title: Markdown Cheatsheet
date: 2018-10-01 00:00:00 +0300
description: Learn markdown cheatsheet # Add post description (optional)
img: markdow-cheatsheet.png # Add image post (optional)
tags: [Markdown, Cheatsheet] # add tag
---
#Headers:

# H1
## H2
### H3
#### H4
##### H5
##### H6
Ngoài ra, H1 và H2 còn có kiểu gạch dưới:

Alternatively-H1
======
Alt-H2
------
#Định dạng kiểu chữ:
Đây là *in nghiêng* hoặc _gạch dưới_.
Hoặc là **nhấn mạnh** hoặc __nghiêng và nhấn mạnh__.
Kết hợp *_nghiêng và gạch dưới_*
Gạch ngang là ~~đây~~.

#List:
######(Trong vi du nay, cac dau cach dau va cuoi duoc hien thi voi dau cham .)

1. Danh sách 1
2. Danh sách 2
   * Danh sách 3
1. Thực tế, số không quan trọng, nó không phải là số thứ tự của list?
2. Thứ tự vẫn được sắp xếp theo trật tự.
3. Và thêm nữa, như trên.
   Sử dụng 3 dấu cách để căn chỉnh, thụt lề.
   Để ngắt dòng, xuống dòng sử dụng 2 dấu cách.  
   Dòng này riêng biệt nhưng cùng một đoạn.  
   Điều này trái ngược với ngắt dòng GFM?, nơi không yêu cầu dấu cách.

* Danh sách không có số thứ tự có thể sử dụng hoa thị.
- Hoặc dấu trừ
+ Hoặc dấu cộng

#Links
###Có hai cách tạo liên kết.

1. [Liên kết nội tuyến](https://www.google.com)
2. [Liên kết nội tuyến có tiêu đề](https://www.google.com "Google's Homepage")
3. [Liên kết tham chiếu][Văn bản tham chiếu không phân biệt dạng chữ]
4. [Liên kết tham chiếu tương đối tới một tập tin, kho lưu trữ](../blob/master/LICENSE)
5. [Bạn có thể sử dụng số cho định nghĩa liên kết kiểu tham số][1]
6. Hoặc để trống và sử dụng [liên kết chính nó]
7. URLs và URLs đặt trong dấu ngoặc nhọn sẽ tự động được chuyển thành liên kết. http://www.example.com hoặc <http://www.example.com> và đôi khi là example.com (nhưng không phải trên Github)

Một số văn bản để cho thấy rằng liên kết tham chiếu có thể theo sau.

[Văn bản tham chiếu không phân biệt dạng chữ]: https://www.google.com
[1]: http://slashdot.org
[liên kết chính nó]: http://www.reddit.com

#Images

Đây là logo
Kiểu nộ tuyến- Inline-style:
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo kiểu 1")

Kiểu tham chiếu- Reference-style:
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo kiểu 2"

#Code and Syntax Highlighting
Code block là một phần của đặc tả markdown, nhưng nó không tô sáng cú pháp. Tuy nhiên, nhiều renderers(trình kết xuất) hỗ trợ điều đó như của Github và Markdown Here.
   *Markdown Here hỗ trợ làm nổi bật hàng chục ngôn ngữ(phi ngôn ngữ-như các tiêu đề HTTP).
    Ví dụ: Kiểu nội tuyến `code` has `có dấu tích chéo xung quanh` nó.
    Blocks of code được chặn bằng các dòng với ba dấu chéo ```, hoặc được thụt vào bằng bốn dấu cách
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```

```
Không có ngôn ngữ nào được chỉ định ở đây, do đó không có tô sáng cú pháp trong Markdown Here(thay đổi trên Github). Nhưng hãy đưa nó vào thẻ <b></b>
```

#Tables
Tables không phải là một phần đặc tả của Markdown, nhưng chúng là một phần được GFM và Markdown Here hỗ trợ. Chúng là một cách dễ dàng để thêm bảng vào email.

Dấu hai chấm có thể được thêm vào để căn chỉnh các cột.

| Bảng | Thật | Cool  |
| ---- | :--- | ----: |
| Một  | là   | đô la |
| Hai  | là   | Euror |
| Ba   | là   | VNĐ   |

Phải có ít nhất ba dấu gạch ngang tách riêng mỗi ô tiêu đề.
Các dấu | là tùy ý, không phải xếp thẳng hàng chúng.
Cũng có thể sử dụng markdown nội tuyến:

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| *Still*  | `renders` | **nicely** |
| 1        | 2         | 3          |

#Blockquotes:
> Blockquotes rất tiện dụng trong email để mô phỏng văn bản trả lời.
> Đây là một dòng quote-trích dẫn.

Quote break.

> Đây là một dòng dài vãi cả cức nhưng quote brack vẫn ngắt dòng đúng chỗ khiến nó trông trở nên ngay ngắn xinh đẹp hơn, chúng ta có thể thêm một vài định dạng kiểu chữ để nhấn mạnh như là *in nghiêng*, **in đậm**, _gạch dưới-k thấy có thay đổi gì_, ~~gạch bỏ~~

#Inline HTML

Các cậu có thể sử dụng HTML thô trong Markdown của các cậu, nó vẫn sẽ hoạt động pretty well.
<dl>
	<dt>Danh sách</dt>
	<dd>Đôi khi là thế này.</dd>
	<dt>Markdown in HTML</dt>
	<dd>Nếu *không* hoạt động **tốt**. Hãy sử dụng  <em>thẻ</em></dd>
</dl>


#Horizontal Rule

Ba hoặc nhiều hơn...
---
Dấu gạch ngang

***

Dấu hoa thị

___

Dấu gạch dưới

#Line Breaks

Đây là dòng bắt đầu

Dòng này tách ra khỏi dòng trên bằng hai dòng mới, do đó, nó sẽ là *một đoạn riêng biệt*.

Dòng này cũng là một dòng riêng biệt nhưng
Dòng này chỉ được phân tách bằng một dòng mới, vì vậy nó là một dòng riêng biệt *trong cùng một đoạn*.

Lưu ý: Markdown Here sử dụng ngắt dòng GFM, do đó không cần sử dụng hai dấu cách xuống dòng của MD(markdown.)

#YouTube Videos

Chúng không thể được thêm trực tiếp nhưng có thể thêm hình ảnh có liên kết tới video như sau:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

hoặc trong Markdown thuần túy, nhưng mất kích thước và đường viền:
[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)
