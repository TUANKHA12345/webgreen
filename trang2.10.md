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
            background-color: #8BC34A; 
            padding: 10px 15px; 
            border-radius: 5px; 
            position: absolute; 
            right: 20px; 
            top: 20px;
        }
    </style>
</head>
<body>  <a href="trang2.html" class="home-button">← Quay lại trang 2</a>
    <div class="content">
        <p><b>- Thương hiệu:</b> Herbland (Việt Nam)</p>
        <p><b>- Nơi sản xuất:</b> Việt Nam</p>
        <p><b>- Giá tham khảo:</b> 130.000 VNĐ/lọ 60 viên (Cập nhật tháng 09/2023)</p>
        <p>- Herbland là thương hiệu dược phẩm thuộc Công ty TNHH Dược Phẩm Thành Tâm, ra đời năm 2011. Hãng chuyên phân phối và tiếp thị các sản phẩm dược phẩm, thuốc và thực phẩm chức năng có chất lượng cao, dành cho mọi lứa tuổi.</p>
        <p>- Viên uống giúp bổ sung vitamin D3 hỗ trợ tăng cường hấp thu canxi vào xương, làm giảm nguy cơ còi xương ở trẻ em và loãng xương ở người lớn do thiếu vitamin D. Sản phẩm phù hợp sử dụng cho trẻ em từ 6 tuổi trở lên và người lớn cần bổ sung vitamin D, người lớn bị loãng xương, trẻ em bị còi xương,...</p>
        <p><b>-Đối tượng sử dụng:</b> Sử dụng cho trẻ từ 6 tuổi trở lên.</p>
        <p><b>- Cách sử dụng:</b> Uống 1 – 2 viên/ngày.</p>
    </div>
    <img src="HEALTHZA.jpg" alt="Viên uống Healthza Vitamin D3 1000IU">

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
