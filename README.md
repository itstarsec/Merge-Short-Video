![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
<a href = "https://cothach.vn">![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)</a>

# Ứng dụng tạo video dựa trên trích dẫn cho Shorts/Reels/TikTok
<h3>Kịch bản này tạo video trích dẫn chất lượng cao dọc (1920x1080) trong khoảng 15 giây mỗi video!</h3>

## 📝 Table of Contents

1. [Giới thiệu](#about)
2. [Demo](#demo)
3. [Cách hoạt động](#working)
4. [Cách chạy ứng dụng](#how_to)
5. [Triển khai](#built_using)
6. [Kết quả đạt được](#results)
7. [Lưu ý](#note)

<h2 id="demo">🎥 Demo</h2>

https://github.com/SamuraiPolix/ShortsMaker/assets/52662032/fb67c274-8701-482a-a557-466ce4b9a9ef


<h2 id="about">🧐 About</h2>

Đây là dự án Python lớn đầu tiên của tôi, mà tôi đã bỏ rất nhiều công sức vào đó, hy vọng bạn sẽ tận dụng tối đa nó :)

Tôi đã sử dụng nó để bán các video trích dẫn Kinh Thánh trên Fiverr trong một thời gian.


<h2 id="working">💭 How it works</h2>

<h4>#1 Content</h4>
Tôi có 50+ video nền (chủ yếu là thiên nhiên), 40 tệp âm thanh và 10 phông chữ.

<h4>#2 Editing</h4>

Kịch bản hoạt động bằng cách lấy một video nền từ thư mục '/videos', một tệp âm thanh từ thư mục '/audios', một phông chữ ngẫu nhiên, và một trích dẫn (một đoạn Kinh Thánh) từ tệp JSON, và kết hợp chúng thành một video duy nhất.


Tôi đang sử dụng **PILLOW** để tạo ra văn bản bằng các phông chữ khác nhau và **FFMPEG** để kết hợp chúng một cách nhanh chóng nhất có thể (ban đầu tôi đã sử dụng **MoviePy** nhưng nó quá chậm).

Tất cả các tệp video và tệp âm thanh đều là miễn phí bản quyền từ các trang web cung cấp video và hình ảnh như Pexels, Pixabay, v.v., và các phông chữ cũng là miễn phí bản quyền.

<h2 id="how_to">🏁 How to run</h2>

Follow the instructions given below to get this script up and running on your device.

1. Download this repository as zip file / using git.
2. Open the folder.
3. Make sure all the required modules are installed. (`pip install -r requirements.txt`)
4. Open main.py
5. set the number of videos you want, your logo, and choose a quote file from '/sources/verses_data' (you can also use the <a href="https://github.com/SamuraiPolix/openbible-verse-scraper">topical bible verses scraper</a> I developed)
```python
number_of_videos = 99
customer_name = "your_name"
image_file = f"{project_dir}/sources/logo.png"
json_file = f"{project_dir}/sources/verses_data/love_data.json"
```
6. RUN!
7. And that's it! Everything else will be handled automatically!
8. You can find your video in the `customers/your-name/` directory.

<h2 id="built_using">⛏️ Built Using</h2>

1. [PILLOW](https://pypi.org/project/Pillow/) - For generating text images.
2. [FFMPEG](https://ffmpeg.org/) - For video editing.


<h2 id="results">🎥 Final Results</h2>

After running the script you will get these 3 files:
1. The edited video file.

   https://github.com/SamuraiPolix/ShortsMaker/assets/52662032/1640ba4f-13c5-4698-9f2f-bcbfacb9b908
3. A spreadsheet containing all the File names, verses, and references, to make it easier to find the video you want.

   ![image](https://github.com/SamuraiPolix/ShortsMaker/assets/52662032/6b597a1a-d7e0-495b-8f65-b6852eeb04a1)
4. The generated text image (for the quote in the video).

   <img src="https://github.com/SamuraiPolix/ShortsMaker/assets/52662032/340d9401-5aac-49f9-bf44-66e982b61abc" width="45%">

<h2 id="note">🗒️ Note</h2>

Lưu ý rằng kịch bản này hiện tại rất cơ bản. Tôi đã thêm Text-to-Speech vào phiên bản sau và hy vọng sẽ sớm đăng lên. Nếu bạn muốn đóng góp, bạn hoàn toàn có thể làm và bạn cũng có thể fork và cải thiện kho lưu trữ này..
"# Merge-Short-Video" 
