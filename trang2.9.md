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
        <p><b>- Thương hiệu:</b> Pediakid (Pháp)</p>
        <p><b>- Nơi sản xuất:</b> Pháp</p>
        <p><b>- Giá tham khảo:</b> 270.000 VNĐ/lọ 125 ml (Cập nhật tháng 09/2023)</p>
        <p>- Pediakid là một thương hiệu thực phẩm chức năng nổi tiếng có xuất xứ từ Pháp, thuộc sở hữu của Công ty Ineldea Laboratoires de France, thành lập vào năm 2003. Đây là một công ty có tuổi đời lâu năm trong ngành chăm sóc sức khỏe con người với đa dạng sản phẩm, phổ biến nhất là những loại siro cung cấp vitamin cho trẻ nhỏ.</p>
        <p>- Bảng thành phần của siro dinh dưỡng có đến 22 loại vitamin và khoáng chất đa dạng khác nhau, giúp đẩy mạnh sự phát triển của trẻ nhỏ. Thêm vào đó, hoạt chất hỗ trợ hệ tiêu hóa của bé khỏe hơn gọi là prebiotic cũng được nhà sản xuất nghiên cứu và bổ sung trong sản phẩm.</p>
        <p><b>-Đối tượng sử dụng:</b> Sử dụng cho trẻ từ 1 tuổi trở lên.</p>
        <p><b>- Cách sử dụng:</b> Uống 2 lần/ngày vào sáng và chiều.</p>
    </div>
    <img src="SIRO.jpg" alt="Siro Pediakid 22 Vitamines">

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
