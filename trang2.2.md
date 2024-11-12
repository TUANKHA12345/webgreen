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
        <p><b>- Thương hiệu:</b> DHC (Nhật Bản)</p>
        <p><b>- Nơi sản xuất:</b> Nhật Bản</p>
        <p><b>- Giá tham khảo:</b> Khoảng 275.000 VNĐ/90 viên (Cập nhật tháng 09/2023).</p>
        <p>- Viên uống DHC vitamin tổng hợp là sản phẩm thuộc thương hiệu DHC, chuyên sản xuất và kinh doanh mỹ phẩm cũng như các sản phẩm chăm sóc sức khỏe bao gồm thực phẩm chức năng nổi tiếng tại Nhật Bản, được nhiều người yêu thích và tin dùng nhất.</p>
        <p>- Sản phẩm có chứa 12 loại dưỡng chất thiết yếu cho cơ thể với hàm lượng phù hợp. Khi sử dụng, bạn sẽ được bổ sung đầy đủ vitamin và khoáng chất, giúp tăng cường sức đề kháng chống lại bệnh tật.</p>
        <p><b>Đối tượng sử dụng:</b> Người trưởng thành bị thiếu chất, có nhu cầu bổ sung vitamin.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>
    </div>
    <img src="LỢI ÍCH.jpg" alt="Viên uống DHC vitamin tổng hợp">

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
