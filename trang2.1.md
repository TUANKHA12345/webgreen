<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="refresh" content="5">
    <title>Document</title>
    <style>
        body {
            font-size: 18; 
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px; 
        }
        .content {
            max-width: 60%; 
        }
        img {
            width: 600px; 
            height: auto; 
            margin-left: 20px; 
        }
        h1 {
            font-size: 200px; 
        }
        p {
            margin: 20px 0; 
        }
        .home-button {
            font-size: 24px; 
            text-decoration: none; 
            color: white; 
            background-color: #8BC34A; 
            padding: 10px 15px;
            border-radius: 5px;
            position: absolute;
            right: 20px; 
            top: 20px;
        }
    </style>
</head>
<body>
    <a href="trang2.html" class="home-button">← Quay lại trang 2</a>
    <div class="content">
        <p><b>- Thương hiệu:</b> Herbland (Việt Nam)</p>
        <p><b>- Nơi sản xuất:</b> Việt Nam</p>
        <p><b>- Giá tham khảo:</b> Khoảng 550.000 VNĐ/2 lọ 30 viên (Cập nhật tháng 09/2023)</p>
        <p>- Viên uống Herbland IQKARE là sản phẩm thuộc thương hiệu Herbland nổi tiếng của Việt Nam. Đây là thương hiệu dược phẩm nổi tiếng được nhiều người Việt tin dùng bởi chất lượng sản phẩm tốt. Sản phẩm chứa hơn 20 loại vitamin và khoáng chất thiết yếu cho mẹ bầu như dầu cá, vitamin A, vitamin E,... Đồng thời, sản phẩm có chứa biotin giúp làn da của mẹ bầu khỏe mạnh và đẹp hơn.</p>
        <p><b>- Đối tượng sử dụng:</b> Phụ nữ mang thai và cho con bú cần bổ sung vitamin và khoáng chất.</p>
        <p><b>- Cách sử dụng:</b> Uống 2 viên mỗi ngày.</p>
    </div>
    <img src="HERBLAND IQKARE.jpg" alt="Viên uống Herbland IQKARE">

    <audio id="background-music" loop autoplay>
        <source src="nhac1234.mp3" type="audio/mpeg">
    </audio>
    <script>
        const music = document.getElementById('background-music');
        music.volume = 0.12;
    
        window.onload = () => {
            if (localStorage.getItem('musicPaused') === 'true') {
                music.pause();
            } else {
                music.play();
            }
        };
    
        window.onbeforeunload = () => {
            localStorage.setItem('musicPaused', music.paused);
        };
    </script>

</body>
</html>
