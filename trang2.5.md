
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
            font-size: 100%; 
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
    <a href="trang2.html" class="home-button">Home</a>
    <div class="content">
        <p><b>- Thương hiệu:</b> Blackmores (Úc)</p>
        <p><b>- Nơi sản xuất:</b> Úc</p>
        <p><b>- Giá tham khảo:</b> Khoảng 450.000 VNĐ/lọ 50 viên (Cập nhật tháng 09/2023)</p>
        <p>- Blackmores là thương hiệu thực phẩm chức năng hàng đầu đến từ Úc được thành lập từ năm 1930. Với hơn 85 năm phát triển, thương hiệu đã sở hữu 1500 điểm phân phối tại 17 quốc gia. Các sản phẩm thực phẩm chức năng của Blackmores đều đạt tiêu chuẩn TGA nghiêm ngặt tại Úc.</p>
        <p>- Viên uống đa vitamin và tăng cường năng lượng Blackmores Multivitamin + Energy tổng hợp toàn diện các loại vitamin nhóm B cùng các loại vitamin khác. Cung cấp các dưỡng chất quan trọng giúp cơ thể phục hồi và khỏe mạnh hơn đồng thời sản xuất năng lượng để hoạt động mỗi ngày.</p>
        <p><b>- Đối tượng sử dụng:</b> Người trưởng thành trên 18 tuổi.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>
    
    </div>
    <img src="MULTIVITAMIN+ENERGY.jpg" alt="Viên uống Blackmores Multivitamin + Energy">

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