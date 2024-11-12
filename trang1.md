<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="refresh" content="5">
    <title>Document</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            font-size: 18px; /* Thay đổi kích thước chữ tại đây */
            background-color: #D9EAD3; /* Màu nền xanh lá cây nhạt */
            padding: 20px; /* Thêm khoảng cách bên ngoài */
            text-align: left; /* Căn trái nội dung */
        }
        h1 {
            font-size: 32px; /* Kích thước chữ cho tiêu đề */
        }
        .home-button {
            font-size: 24px; /* Kích thước nút */
            text-decoration: none; /* Không có gạch chân */
            color: white; /* Màu chữ */
            background-color: #8BC34A; /* Màu xanh lá cây nhạt */
            padding: 10px 15px; /* Khoảng cách bên trong nút */
            border-radius: 5px; /* Bo tròn góc nút */
            position: absolute; /* Để định vị nút */
            right: 20px; /* Đẩy nút sang bên phải */
            top: 20px; /* Đẩy nút lên trên cùng */
        }
    </style>
</head>
<body>
    <a href="trang chủ.html" class="home-button">Home</a>
    <h1><b>Một chế độ ăn uống lành mạnh là gì?</b></h1><br>
    <p>Chế độ ăn uống lành mạnh là một loại chế độ ăn cung cấp cho cơ thể lượng calo đầy đủ cùng với các chất dinh dưỡng cần thiết từ đồ ăn và thức uống, đảm bảo mục tiêu duy trì và cải thiện sức khỏe tổng thể.<br>
        Một chế độ ăn uống lành mạnh có thể bao gồm trái cây, rau, ngũ cốc, cây họ đậu, thịt nạc,… và hạn chế các thực phẩm chế biến sẵn hoặc đồ uống có đường. <br>
        Một lối sống lành mạnh bao gồm tập thể dục mỗi ngày cùng với việc ăn uống lành mạnh, lối sống lành mạnh có thể làm giảm nguy cơ mắc các bệnh như béo phì, bệnh tim, tiểu đường loại 2, tăng huyết áp và ung thư.</p><br>
    
    <p>Để có một chế độ ăn uống lành mạnh, bạn cần:</p>
    <ul>
        <li>Uống đủ nước mỗi ngày để duy trì sự cân bằng nước cho cơ thể.</li>
        <li>Chọn các loại thực phẩm tươi sống, hạn chế thực phẩm đông lạnh hoặc chế biến sẵn.</li>
        <li>Ăn đủ các loại thực phẩm từ các nhóm khác nhau để đảm bảo đầy đủ chất dinh dưỡng.</li>
        <li>Theo dõi khẩu phần ăn của bạn để không tiêu thụ quá nhiều calo.</li>
    </ul>
    
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