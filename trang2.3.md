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
            font-size: 18px;
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
        <p><b>- Thương hiệu:</b> One A Day (Mỹ)</p>
        <p><b>- Nơi sản xuất:</b> Mỹ</p>
        <p><b>- Giá tham khảo:</b> Khoảng 570.000 VNĐ/lọ 300 viên (Cập nhật tháng 09/2023)</p>
        <p>- One A Day là thương hiệu dược phẩm có tiếng tại Mỹ. Hãng nổi tiếng với các sản phẩm chuyên bổ sung vitamin và khoáng chất phù hợp với mọi lứa tuổi. Đây là thương hiệu quen thuộc với người Mỹ hay người tiêu dùng ở các nước châu Âu và được đánh giá cao về chất lượng sản phẩm.</p>
        <p>- Viên uống vitamin tổng hợp One A Day có thành phần hơn 20 vi khoáng tiêu biểu như vitamin C, vitamin A, vitamin D cùng kẽm, canxi,... bổ sung vitamin, khoáng chất và axit amin cần thiết giúp cơ thể tràn trề năng lượng.</p>
        <p><b>- Đối tượng sử dụng:</b> Phụ nữ từ 18 - 50 tuổi.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>

    </div>
    <img src="ONE A DAY.jpg" alt="Viên uống vitamin tổng hợp One A Day">

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
