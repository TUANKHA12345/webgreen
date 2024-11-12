<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="refresh" content="5">
    <title>Document</title>
    <style>
        body {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px;
            font-size: 16px; 
        }

        .content {
            max-width: 60%;
        }

        p {
            margin: 20px 0; 
        }

        img {
            width: 600px; 
            margin-left: 20px;
        } .home-button {
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
        <p><b>- Thương hiệu:</b> Puritan’s Pride (Mỹ)</p>
        <p><b>- Nơi sản xuất:</b> Mỹ</p>
        <p><b>- Giá tham khảo:</b> Khoảng 349.000 VNĐ/ 100 viên (Cập nhật tháng 09/2023)</p>
        <p>- Viên uống bổ sung vitamin tổng hợp và khoáng chất của Puritan’s Pride là sản phẩm đến từ Mỹ. Thương hiệu Puritan’s Pride nổi tiếng với sản phẩm thực phẩm chức năng có chiết xuất từ thiên nhiên. Với hơn 40 năm hình thành và phát triển, các sản phẩm được nhiều người trên thế giới tin dùng.</p>
        <p>- Sản phẩm cung cấp hơn 30 loại vitamin như vitamin A, vitamin B1, vitamin B12, vitamin C, vitamin D, vitamin E,... cùng các khoáng chất như sắt, kẽm,... giúp tăng cường sức đề kháng, cải thiện thị lực, hoạt động tim mạch tốt, huyết áp ổn định.</p>
        <p><b>- Đối tượng sử dụng:</b> Nam nữ trên 18 tuổi.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>
    </div>
    <img src="PRIDE.jpg" alt="Viên uống Puritan’s Pride">

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
