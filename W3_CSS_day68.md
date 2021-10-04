## CSS Image Gallery

CSS를 사용하여 이미지 갤러리를 만들 수 있습니다.

---

### 이미지 갤러리

다음 이미지 갤러리는 CSS로 생성됩니다.

    예시

    <html>
    <head>
    <style>
    div.gallery {
    margin: 5px;
    border: 1px solid #ccc;
    float: left;
    width: 180px;
    }

    div.gallery:hover {
    border: 1px solid #777;
    }

    div.gallery img {
    width: 100%;
    height: auto;
    }

    div.desc {
    padding: 15px;
    text-align: center;
    }
    </style>

    </head>
    <body>

    <div class="gallery">
    <a target="_blank" href="img_5terre.jpg">
        <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
    </div>

    <div class="gallery">
    <a target="_blank" href="img_forest.jpg">
        <img src="img_forest.jpg" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
    </div>

    <div class="gallery">
    <a target="_blank" href="img_lights.jpg">
        <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
    </div>

    <div class="gallery">
    <a target="_blank" href="img_mountains.jpg">
        <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
    </div>

    </body>
    </html>
