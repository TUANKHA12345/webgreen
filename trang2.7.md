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
            margin: 25px 0;
        }

        img {
            width: 600px; 
            margin-left: 50px;
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
        <p><b>- Thương hiệu:</b> Centrum (Mỹ)</p>
        <p><b>- Nơi sản xuất:</b> Mỹ</p>
        <p><b>- Giá tham khảo:</b> Khoảng 120.000 VNĐ/lọ 60 viên (Cập nhật tháng 09/2023)</p>
        <p>- Centrum là thương hiệu có nguồn gốc từ Mỹ và được nghiên cứu bởi hãng Pfizer. Centrum đã có hơn 30 năm kinh nghiệm trong lĩnh vực sản xuất thực phẩm chức năng. Các sản phẩm của Centrum đều được nghiên cứu bởi các chuyên gia đầu ngành cùng quy trình sản xuất và kiểm tra nghiêm ngặt, vì vậy bạn hoàn toàn có thể yên tâm khi sử dụng.</p>
        <p>- Viên uống vitamin tổng hợp Centrum Adults Multivitamin bổ sung 31 loại vi khoáng thiết yếu cho cơ thể. Sản phẩm giúp nâng cao khả năng miễn dịch, cải thiện các vấn đề về tim mạch, tăng cường chuyển hóa chất và tạo năng lượng, cùng với đó là nhiều công dụng khác tốt cho sức khỏe.</p>
        <p><b>- Đối tượng sử dụng:</b> Nam nữ từ 18 – 50 tuổi thiếu dinh dưỡng, thường xuyên mệt mỏi.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>
    </div>
    <img src="CENTRUM.jpg" alt="Viên uống Centrum Adults Multivitamin">

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
