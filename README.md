<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Minamoto no Tora - 12.9</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Segoe UI', Arial, sans-serif;
}

html{
  scroll-behavior:smooth;
}

body{
  background:#f1f5f9;
  color:#0f172a;
  line-height:1.6;
}

/* ===== BANNER ===== */
header{
  position: relative;
  text-align: center;
  padding: 100px 20px;
  color: white;
  overflow: hidden;
  background: #333; /* Màu nền dự phòng */
}

/* Lớp nền ảnh có thêm Overlay để nổi bật chữ */
header::before{
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), 
              url("https://i.ibb.co/TMtFcdHv/image.png") center/cover no-repeat;
  filter: blur(1px);
  z-index: 1;
}

/* Đưa nội dung lên trên lớp nền */
header .container {
  position: relative;
  z-index: 2;
}

header h1{
  font-size: 40px;
  margin-bottom: 10px;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}

header p{
  font-size: 20px;
  font-weight: 500;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
}

nav{
  margin-top:30px;
}

nav a{
  display:inline-block;
  color:white;
  text-decoration:none;
  padding:12px 25px;
  margin:5px;
  border-radius:30px;
  transition:0.3s;
  background:rgba(255,255,255,0.2);
  backdrop-filter: blur(5px);
  border: 1px solid rgba(255,255,255,0.3);
}

nav a:hover{
  background:white;
  color:#7c3aed;
}

/* ===== SECTION ===== */
section{
  padding:40px 20px;
  max-width:1100px;
  margin:auto;
}

.card{
  background:white;
  padding:30px;
  border-radius:18px;
  margin-bottom:30px;
  box-shadow:0 10px 25px rgba(0,0,0,0.05);
  transition:0.3s;
}

.card:hover{
  transform:translateY(-5px);
}

h2{
  color:#7c3aed;
  margin-bottom:20px;
  border-left: 5px solid #7c3aed;
  padding-left: 15px;
}

/* ===== ACTIVITIES ===== */
.activities-menu{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:15px;
  margin-bottom:25px;
}

.activity-btn{
  background:linear-gradient(135deg,#6366f1,#a855f7);
  border:none;
  padding:18px;
  border-radius:15px;
  color:white;
  font-size:17px;
  font-weight: bold;
  cursor:pointer;
  transition:0.3s;
}

.activity-btn:hover, .activity-btn.active{
  transform:scale(1.05);
  box-shadow: 0 5px 15px rgba(124, 58, 237, 0.4);
  filter: brightness(1.1);
}

.activity-content{
  display:none;
  animation:fade 0.6s ease-out;
}

@keyframes fade{
  from{opacity:0; transform:translateY(15px);}
  to{opacity:1; transform:translateY(0);}
}

/* ===== GALLERY ===== */
.gallery{
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(240px,1fr));
  gap:15px;
  margin-top:20px;
}

.gallery img{
  width:100%;
  height:220px;
  object-fit:cover;
  border-radius:12px;
  transition:0.4s;
cursor: pointer;
}

.gallery img:hover{
  transform:scale(1.03);
}

/* ===== FOOTER ===== */
footer{
  text-align:center;
  padding:50px 20px;
  background:#e2e8f0;
  margin-top:60px;
  border-top: 1px solid #cbd5e1;
}

.contact-info {
  margin-bottom: 20px;
}

footer p {
  color: #475569;
  font-size: 15px;
}
</style>
</head>

<body>

<header id="home">
  <div class="container">
    <h1>CLB Minamoto no Tora 源の虎</h1>
    <p>12.9 – Trường THPT Huỳnh Văn Nghệ</p>
    <p>"Thanh xuân là hành trình, không phải đích đến."</p>

    <nav>
      <a href="#home">Trang Chủ</a>
      <a href="#activities">Hoạt Động</a>
      <a href="#contact">Liên Hệ</a>
    </nav>
  </div>
</header>

<section>
  <div class="card">
    <h2>📌 Thông Tin Chuyến Đi</h2>
    <p><b>Lớp:</b> 12.9</p> 
    <p><b>Câu lạc bộ:</b> Minamoto no Tora</p>
    <p><b>Trường:</b> THPT Huỳnh Văn Nghệ</p>
    <p><b>Thời gian:</b> 23 – 25 / 01 / 2026</p>
  </div>
</section>

<section id="activities">
  <h2>🔥 Hoạt Động Nổi Bật</h2>
  <div class="activities-menu">
    <button class="activity-btn" onclick="showContent('dalat', this)">Đà Lạt</button>
    <button class="activity-btn" onclick="showContent('vannghe', this)">Văn Nghệ</button>
    <button class="activity-btn" onclick="showContent('team', this)">Tri Ân</button>
  </div>

  <div id="dalat" class="activity-content card">
    <h3>🌲 Tham Quan Đà Lạt</h3>
    <p>>Đà Lạt không chỉ là chuyến đi, mà là một phần ký ức thanh xuân.
Giữa cái se lạnh của cao nguyên, chúng mình đã cùng nhau cười thật to, chụp thật nhiều ảnh và lưu lại những khoảnh khắc chẳng thể quay lại lần thứ hai.
Thành phố mộng mơ ấy đã chứng kiến tuổi 17 của 12.9 – vô tư, rực rỡ và đầy yêu thương.</p>
    <div class="gallery">
      <img src="https://i.ibb.co/4R8Bddpw/image.png" alt="Đà Lạt 1">
      <img src="https://i.ibb.co/rRZmXmx2/image.png" alt="Đà Lạt 2">
      <img src="https://i.ibb.co/Zp6F7nr1/image.png" alt="Đà Lạt 3">
      <img src="https://i.ibb.co/pB7pCz1J/image.png" alt="Đà Lạt 4">
    </div>
  </div>

  <div id="vannghe" class="activity-content card">
    <h3>🎤 Văn Nghệ</h3>
    <p>Những tiết mục văn nghệ không chỉ là ánh đèn sân khấu, mà là nơi chúng mình cháy hết mình vì tập thể.
Từng bước nhảy, từng lời ca là cả những ngày tập luyện mồ hôi và tiếng cười.
Dưới ánh đèn ấy, 12.9 đã tỏa sáng theo cách rực rỡ nhất của tuổi trẻ</p>
    <div class="gallery">
      <img src="https://i.ibb.co/5WZC2Dh5/image.png" alt="Văn nghệ 1">
      <img src="https://i.ibb.co/607tq6xL/image.png" alt="Văn nghệ 2">
      <img src="https://i.ibb.co/NQbGFjc/image.png" alt="Văn nghệ 3">
      <img src="https://i.ibb.co/vvRqr5vH/image.png" alt="Văn nghệ 4">
    </div>
  </div>

  <div id="team" class="activity-content card">
    <h3>🌸 Lễ Tri Ân</h3>
    <p>Chúng em xin gửi lời tri ân chân thành nhất đến thầy cô – những người đã âm thầm gieo mầm tri thức và thắp sáng ước mơ cho chúng em suốt ba năm qua.
Mỗi lời dạy, mỗi sự nghiêm khắc và yêu thương đều trở thành hành trang quý giá để chúng em bước vào tương lai.
Thanh xuân có thể khép lại, nhưng lòng biết ơn thì sẽ còn mãi.</p>
    <div class="gallery">
      <img src="https://i.ibb.co/HL1HFVf9/image.png" alt="Team 1">
      <img src="https://i.ibb.co/Cp9N2rGP/image.png" alt="Team 2">
    </div>
  </div>
</section>

<section id="contact">
  <div class="card">
    <h2>📞 Liên Hệ</h2>
    <div class="contact-info">
        <p><b>Họ tên:</b> Lại Thị Thuý Hà – <b>STT:</b> 10 – <b>Lớp:</b> 12.9</p>
<p><b>Họ tên:</b> Nguyễn Duy Mạnh – <b>STT:</b> 20 – <b>Lớp:</b> 12.9</p>
     <p><b>Họ tên:</b> Lê Thị Phương Nhi – <b>STT:</b> 27 – <b>Lớp:</b> 12.9</p>   
     <p><b>Họ tên:</b> Đỗ Thành Nhân – <b>STT:</b> 26 – <b>Lớp:</b> 12.9</p>
        <p><b>Email:</b> thpthuynhvannghe@gmail.com</p>
    </div>
  </div>
</section>

<footer>
  <h3>CLB Minamoto no Tora 源の虎 12.9</h3>
  <p>Trường THPT Huỳnh Văn Nghệ</p>
  <p>© 2026 - Kỷ yếu Đà Lạt</p>
</footer>

<script>
// Hàm hiển thị nội dung hoạt động
function showContent(id, btn){
  // Ẩn tất cả nội dung
  document.querySelectorAll('.activity-content').forEach(el=>{
    el.style.display='none';
  });
  
  // Bỏ class active ở tất cả các nút
  document.querySelectorAll('.activity-btn').forEach(b => {
    b.classList.remove('active');
  });

  // Hiển thị nội dung được chọn
  const box = document.getElementById(id);
  box.style.display='block';
  
  // Thêm class active cho nút vừa nhấn
  if(btn) btn.classList.add('active');
}

// Tự động hiển thị mục Đà Lạt khi vừa vào trang
window.onload = function() {
    const firstBtn = document.querySelector('.activity-btn');
    showContent('dalat', firstBtn);
};
</script>

</body>
