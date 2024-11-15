<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bài Tập Thể Thao</title>
    <style>
        body {
            font-family: Arial, sans-serif; 
            font-size: 18px; 
            background-color: #d9f7d9; 
            color: #333; 
            line-height: 1.6; 
            padding: 20px;
        }
        h1 {
            font-size: 36px;
            color: #007BFF;
            text-align: center; 
        }
        h2 {
            font-size: 28px;
            color: #FF5722; 
            margin-top: 30px; 
        }
        p {
            font-weight: bold;
        }
        ul {
            margin: 20px 0; 
            padding-left: 20px; 
            list-style-type: disc;
        }
        video {
            display: block;
            margin: 20px auto; 
            width: 600px; 
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
    <a href="trang chủ.html" class="home-button">Home</a>
    <h1>MỘT SỐ BÀI TẬP NÂNG CAO SỨC KHOẺ</h1>

    <h2>SQUAT BẬT NHẢY</h2>
    <p>Nằm trong top các bài tập tăng sức bền được nhiều người ưa chuộng lựa chọn luyện tập, Squat bật nhảy chắc hẳn là cái tên không còn quá xa lạ đối với dân tập gym chuyên nghiệp. Bài tập này giúp rèn luyện sức bền cho cơ thể rất tốt.</p>
    <ul>
        <li>Bước 1: Đứng thẳng lưng, hai bàn tay nắm chặt và đặt hai bên cạnh sườn, hai chân tách rộng ngang vai.</li>
        <li>Bước 2: Nhún nhẹ chân để tạo được thế bật nhảy lên cao.</li>
        <li>Bước 3: Tiếp tục bật nhảy thật cao rồi tiếp đất ở tư thế tương tự như bước 2.</li>
        <li>Bước 4: Lưu ý khi bật nhảy thì hít vào. Lúc tiếp đất thì thở ra.</li>
    </ul>
    <video controls class="video">
        <source src="squat.mp4" type="video/mp4">
    </video>

    <h2>NHẢY DÂY</h2>
    <p>Nếu bạn đang tìm kiếm bài tập tăng sức bền, nhảy dây chính là gợi ý phù hợp.</p>
    <ul>
        <li>Bước 1: Chuẩn bị dây nhảy có chiều dài phù hợp.</li>
        <li>Bước 2: Hai bàn chân chụm lại, cầm hai đầu dây đặt sau gót chân.</li>
        <li>Bước 3: Tiến hành nhảy dây liên tục trong 40 giây rồi nghỉ 10 giây.</li>
    </ul>
    <video controls class="video">
        <source src="nhảy dây.mp4" type="video/mp4">
    </video>

    <h2>CHẠY BƯỚC NHỎ TẠI CHỖ</h2>
    <p>Chạy bước nhỏ tại chỗ là động tác cơ bản mà hầu như bất kỳ ai cũng từng luyện tập qua.</p>
    <ul>
        <li>Bước 1: Đứng thẳng người, hai chân dang rộng bằng hông.</li>
        <li>Bước 2: Tiến hành chạy bước nhỏ, tiếp đất bằng mũi chân.</li>
        <li>Bước 3: Giữ nhịp thở đều đặn và nhịp nhàng trong khi thực hiện.</li>
    </ul>
    <video controls class="video">
        <source src="chạy bước nhỏ.mp4" type="video/mp4">
    </video>

    <h2>MOUNTAIN CLIMBERS</h2>
    <p>Mountain climbers không đòi hỏi quá nhiều kỹ thuật nhưng vẫn mang đến hiệu quả cao.</p>
    <ul>
        <li>Bước 1: Bắt đầu với tư thế Plank cao.</li>
        <li>Bước 2: Co đầu gối chân phải về phía trước.</li>
        <li>Bước 3: Duỗi thẳng chân phải và co đầu gối chân trái.</li>
        <li>Bước 4: Hạ phần hông xuống và thực hiện động tác co duỗi với tốc độ nhanh nhất có thể.</li>
    </ul>
    <video controls class="video">
        <source src="mountain climbers.mp4" type="video/mp4">
    </video>

    <h2>NHẢY LÒ CO MỘT CHÂN</h2>
    <p>Nhảy lò cò một chân cũng là bài tập tăng sức bền cho tác dụng tốt được nhiều người yêu thích.</p>
    <ul>
        <li>Bước 1: Đứng thẳng lưng, hai chân mở rộng.</li>
        <li>Bước 2: Tiến hành bật nhảy, một chân co, chân còn lại duỗi thẳng tiếp đất.</li>
        <li>Bước 3: Nhảy liên tục trong vòng 40 giây.</li>
    </ul>
    <video controls class="video">
        <source src="nhảy lò cò.mp4" type="video/mp4">
    </video>

    <script>
        const videos = document.querySelectorAll('.video');

        const options = {
            root: null, //*viewport
            threshold: 0 //*ra khỏi vùng nhìn
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (!entry.isIntersecting) {
                    entry.target.pause(); //* dừng video lhi không nhìn thaays 
                }
            });
        }, options);

        videos.forEach(video => {
            observer.observe(video);
        });
    </script>
</body>
</html>
