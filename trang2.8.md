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
        <p><b>- Thương hiệu:</b> Orihiro (Nhật Bản)</p>
        <p><b>- Nơi sản xuất:</b> Nhật Bản</p>
        <p><b>- Giá tham khảo:</b> 389.000 VNĐ/lọ 180 viên (Cập nhật tháng 09/2023)</p>
        <p>- Thương hiệu Orihiro thành lập năm 1972 tại Nhật Bản. Các sản phẩm của Orihiro luôn được các chuyên gia hàng đầu Nhật Bản nghiên cứu và phát triển để mang đến sản phẩm chăm sóc sức khỏe chất lượng tốt cho người dùng. Hiện nay thương hiệu Orihiro luôn nằm trong top đầu lựa chọn ở các nước Nhật, Nga, Trung Quốc, Singapore,...</p>
        <p>- Sản phẩm với các thành phần chính như vitamin B5, vitamin B12, biotin và axit folic có tác dụng bổ sung vitamin cho cơ thể, hỗ trợ nâng cao sức khỏe cho những người ăn uống thiếu chất. Đồng thời còn giúp cải thiện sức khỏe xương khớp, làm móng, tóc mọc nhanh và chắc khỏe.</p>
        <p><b>-Đối tượng sử dụng:</b> Sử dụng cho trẻ từ 3 tuổi trở lên.</p>
        <p><b>- Cách sử dụng:</b> Uống 2 viên/ngày vào sáng và chiều.</p>
    </div>
    <img src="ORHIRO.jpg" alt="Viên nhai Orihiro Most Chewable">

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
