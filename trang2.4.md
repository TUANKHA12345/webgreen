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
        }
        h1 {
            font-size: 100px; 
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
        <p><b>- Thương hiệu:</b> Kirkland (Mỹ)</p>
        <p><b>- Nơi sản xuất:</b> Mỹ</p>
        <p><b>- Giá tham khảo:</b> Khoảng 535.000 VNĐ/lọ 500 viên (Cập nhật tháng 09/2023)</p>
        <p>- Viên uống bổ sung vitamin tổng hợp Daily Multi Kirkland Signature là sản phẩm của thương hiệu Kirkland đình đám tại Mỹ. Các sản phẩm của Kirkland đều được chứng nhận bởi Hội đồng Dược điển Hoa Kỳ (USP) nên người dùng hoàn toàn có thể yên tâm khi sử dụng.</p>
        <p>- Sản phẩm cung cấp đầy đủ các loại vitamin thiết yếu giúp nâng cao sức đề kháng cho cơ thể, hỗ trợ ngăn ngừa các bệnh liên quan đến tim mạch như cao huyết áp, đột quỵ. Ngoài ra, sản phẩm còn có nhiều công dụng của các loại vitamin khác nhau.</p>
        <p><b>- Đối tượng sử dụng:</b> Người trên 18 tuổi có nhu cầu bổ sung vitamin và khoáng chất. Không sử dụng cho phụ nữ mang thai và cho con bú.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 viên/ngày.</p>

    </div>
    <img src="DAILY MULTI.jpg" alt="Viên uống Daily Multi Kirkland Signature">

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
