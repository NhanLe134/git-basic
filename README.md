<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Two Columns with Image</title>
    <link rel="stylesheet" href="styles.css">
<title>NHI.SG</title>
<style>
  /* Style cho menu */
  body, html {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
}

  background-image {
    position: absolute;
    top: 0;
    left: 0;
    object-fit: cover;
    z-index: -1; /* Đặt lớp dưới cùng */
     width: 100%; /* Chiếm 30% chiều rộng của màn hình */
    height: 60%;
}
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: white;
    z-index: 999; 
  }

  li {
    float: left;
    
  }

  li a {
    display: block;
    color: black;
    text-align: center;
    padding: 30px 30px;
    text-decoration: none;
    font-family: 'times new roman', sans-serif;
  }

  li a:hover {
    color: red;
  }
 .container {
    display: grid; 
    grid-template-columns: 45% 55%; /* Chiếm 40% và 60% chiều rộng của màn hình */
    height: 100vh;
    margin-left: 13%;
   margin-right: 13%;
    padding-top: 5%; /* Thêm khoảng trống 10px phía trên */
    padding-bottom: 5%;
}

.left-column {
    background-size: cover; /* Đảm bảo ảnh vừa đủ kích thước với kích thước của phần tử */
    background-position: center; /* Căn giữa ảnh */
    top: 50px;
  
}

.right-column {
    top: 50px;
  padding-top: 3%;
  
}
.column-image {
    width: 90%; /* Chiếm 60% chiều rộng của cột */
    height: auto; /* Đảm bảo tỉ lệ khung hình không bị thay đổi */
    position: center;
}
.vb {
    font-size: 17px;
    color: #555555;
    text-align: justify;
  }
.highlight-text {
      display: inline-block;
      border: 1px solid #DDDDDD; /* Khung xung quanh văn bản, mặc định là đen */
      transition: background-color 0.3s, color 0.3s, border-color 0.3s;
      padding: 5px; /* Khoảng cách giữa văn bản và khung */
 }

.highlight-text:hover {/* Đổi màu nền khi con trỏ chuột hover vào */
      background-color: red;
      color: white;
     border-color: red;
  }
.video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 80%;
        }
.video-container {
            position: relative;
            width: 80%; /* Chiếm 80% tỉ lệ màn hình ngang */
            margin: 0 auto; /* Căn giữa video */
            padding-top: 56.25%; /* Tỉ lệ khung hình 16:9 (9/16 = 56.25%)*/
            border-radius: 50px; /* Bo viền cho video */
        }
.grid-container {
            display: grid;
            grid-template-columns: repeat(5, 1fr); /* Chia màn hình thành 5 cột */
            height: 40vh; /* Chiều cao cả trang */
            margin-left: 11%;
            margin-right: 11%;
            padding-top: 0px; /* Thêm khoảng trống 10px phía trên */
            padding-bottom: 5%;
        }

.grid-item {
            border: 1px solid #DDDDDD; /* Viền khung màu đen */
            box-sizing: border-box; /* Tính cả viền vào kích thước */
        }
.grid-item:first-child {
            border: none;
            margin-right: 40px;
        }
.nd {
            margin-top: 35px; 
            margin-left: 35px;
            font-family: Segoe UI Historic; 
            font-weight: bold;
            font-size: 20px;
    }
.no-line-break p {
            display: inline-block; /* Không cho phép xuống dòng */
            margin: 0; /* Xóa margin để tránh khoảng trắng thừa */
        }
.grid-container2 {
            display: grid; 
            grid-template-columns: 8% 2% 6% 2% 6% 2% 6% 2% 6% 2% 6%;
            justify-content: center; margin-top: -5px;
            margin-top: -40px;
        }

        .grid-item2 {
            border: 1px solid transparent; /* Viền khung màu đen */
            box-sizing: border-box; /* Tính cả viền vào kích thước */
            text-align: center;
            font-family: Segoe UI Historic;
            font-weight: bold;
           padding-top: 7px; /* Thêm khoảng trống 10px phía trên */
            padding-bottom: 7px;
        } 
.grid-item2:hover {/* Đổi màu nền khi con trỏ chuột hover vào */
      background-color: red;
      color: white;
     border-color: red;
  }
  .picturezoom {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px; 
    margin-left: 11%;
    margin-right: 11%;
    padding-top: 40px; /* Thêm khoảng trống 10px phía trên */
    padding-bottom: 5%;
}

.picture {
    border: 1px solid transparent;
    box-sizing: border-box;
    position: relative;
    overflow: hidden;
    
}
.picture img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    transition: transform 0.3s ease;
}
.picture:hover img {
    transform: scale(1.1);
}
  .khung{ background: #F5FFFA;}
  .teacher {
    display: grid;
    grid-template-columns: 34% 25% 30%;
    gap: 30px; /* Chiều cao của màn hình */
/*     background: #F5FFFA; */
    padding-top: 3%;
    padding-left:13%;
    padding-right:11%;
}

.column1,
.column2,
.column3 {
    border: 1px solid transparent;
    box-sizing: border-box;
}
  .column2 img {
    width: 95%;
    height: 90%;
    object-fit: cover;
    padding-left:30px;
}
  .column3 img {
    width: 75%; /* Chiều rộng 100% của khung */
    height: auto; /* Chiều cao tự động thích ứng */
    object-fit: cover; /* Giữ tỷ lệ chiều rộng và chiều cao tự động thích ứng */
    padding-left:30px;
    padding-top:70px;
}
  .demuc {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr; /* Chia mỗi cột thành 1 phần bằng nhau */
    gap: 10px; /* Khoảng cách giữa các cột */
    padding-top:5%;
    padding-left:10%;
    padding-right:10%;
    font-family: arial;
    color: #555555;
}

.cell {
    border: 1px solid transparent;
    box-sizing: border-box;
}
.demuc p {
    transition: transform 0.3s ease;
}

.demuc p:hover:not(.no-effect) {
    transform: translateX(10px);
    color: red;
}
.footer {
/*     position: fixed; */
    bottom: 0;
    left: 0;
    background-color: #C0C0C0;
    padding: 50px;
    height: 50px;
}

.social-icons:not(.nhile) {
    display: flex;
    justify-content: flex-end;
}

.social-icon {
    margin-right: 10px;
}

/* Đảm bảo biểu tượng cuối cùng không có khoảng trắng bên phải */
.social-icon:last-child {
    margin-right: 0;
}
.Logo {
    display: inline-block;
    border-radius: 50%; /* Làm cho hình ảnh trở thành hình tròn */
    overflow: hidden; /* Ẩn phần ngoài của hình ảnh vượt ra khỏi hình tròn */
}

.Logo img {
    width: 30px; /* Đảm bảo hình ảnh lấp đầy phần tròn */
    height: auto; /* Chiều cao tự động thích ứng */
}
.social-icon img {
  width: 50px;
  height: auto;
}
</style>
</head>
<body>
<ul>
  <li><a href="#">HOME</a></li>
  <li><a href="#">PRIVATE COACHING</a></li>
  <li><a href="#">OTHER SERVICES</a></li>
  <li><a href="#">PROJECTS</a></li>
  <li><a href="#">ABOUT US</a></li>
  <li><a href="#">FREE TRAINING</a></li>
  <li><a href="#">CONTACT</a></li>
</ul> 
  
    <img src="https://www.nhi.sg/_next/static/media/home-banner-5.2e1773db.webp" alt="Background" class="background-image">
   
 <div class="container">
        <div class="left-column">  <img src="https://www.nhi.sg/_next/static/media/about-me.2616820d.webp" alt="Image" class="column-image">
         </div>
   
        <div class="right-column">
    <p style="font-size: 15px; font-family: arial; color: red;font-weight: BOLD; line-height: 0.1;">ABOUT ME</p>
   <p style="font-size: 40px; font-family: Arial, sans-serif; font-weight: bold; color: black; line-height: 0.2;">NHILE LIFE COACHING </p>
   <p class="vb" style="line-height: 1.5; font-family: Arial; padding-top: 15px;">
     Welcome to the FREE and VALUABLE knowledge treasure trove of Nhi Le - the first Life Coach in Vietnam. She has Diploma in Psychology from Singapore. Nhi Le helps people become happy, develop themselves, and find the answer to the question "Who am I?" via the lessons and experiences she has accumulated.
<br> <br>
Despite growing up in an imperfect environment in Quang Nam province and becoming a single mother in a foreign land, Nhi Le never gave up. She tirelessly learns and develops herself, standing up against obstacles. With effort and perseverance, Nhi Le has achieved success in her many roles, from investor, entrepreneur, advisor, leader to renowned healing speaker, not only in Singapore but also in many other parts of the world.
<br> <br>
To assist the people of Vietnam in transforming their lives and uncovering their inner potential, Nhi Le, along with the Strengths Quotient Institute (SQI) and the NhiLe Team, is bringing the copyright of many quality courses to her homeland. The positive environment and valuable knowledge of the Ikigai Zone and SQI have also helped Nhi Le continuously "rebirth" herself into a more perfect version.
          </p>
      <p style="font-family: Arial, sans-serif; font-weight: bold; padding: 20px" class="highlight-text">ㅤVIEW MORE →ㅤ</p>
              </div>
  </div>
<div class="video-container">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/LqTQixWPG1c?si=4LFuj6e6Tjcc7tdM&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </div>
<div class="grid-container">
        <div style="font-family: Segoe UI Historic; font-weight: bold;" class="grid-item">
  <p style="color: red;font-size: 48px; margin: 0;">250,000+</p>
  <p style="color: red;font-size: 15px; margin-top: -5px;">YOUTUBE SUBSCRIBERS</p>
  <p style="color: black;font-size: 48px; margin: 0;">423,500+</p>
  <p style="color: black;font-size: 15px; margin-top: -5px;">TIKTOK FOLLOWERS</p>
  <p style="color: #00008B;font-size: 48px; margin: 0;">484,000+</p>
  <p style="color: #00008B;font-size: 15px; margin-top: -5px;">FACEBOOK FOLLOWERS</p>        
  </div>
        <div class="grid-item"> 
  <img style="margin-top: 35px; margin-left: 35px;" src="https://www.nhi.sg/_next/static/media/privacy-life-coach.d83a0e26.png" alt="Image">
  <p style="margin-top: 35px; margin-left: 35px;" class="nd">PRIVACY LIFE <br> COACH</p>
  </div>
        <div class="grid-item">
  <img style="margin-top: 35px; margin-left: 35px;" src="https://www.nhi.sg/_next/static/media/mentor.25606f77.png" alt="Image" width="61px" height="61px">
  <p class="nd">MENTOR</p>
  </div>
        <div class="grid-item">
  <img style="margin-top: 35px; margin-left: 35px;" src="https://www.nhi.sg/_next/static/media/team-building.9c03e8e0.png" alt="Image" width="61px" height="61px">
  <p class="nd">TEAM BUILDING</p>
  </div>
        <div class="grid-item">
  <img style="margin-top: 35px; margin-left: 35px;" src="https://www.nhi.sg/_next/static/media/speaker.010c853e.png" alt="Image" width="61px" height="61px">
  <p class="nd">SPEAKER</p>
  </div>
    </div>
<div>
  <p style="text-align: center; font-weight: bold; font-size: 50px; font-family: Segoe UI Historic;">OTHER SERVICES</p>
  </div>
  <div class="grid-container2">
        <div class="grid-item2" style="background-color: red;color: white;">MARKETING</div>
        <div class="grid-item3" style="text-align: center; font-family: Courier New; font-weight: bolder; color: red;  padding-top: 7px;">-</div>
        <div class="grid-item2">EDITOR</div>
        <div class="grid-item3" style="text-align: center; font-family: Courier New; font-weight: bolder; color: red;  padding-top: 7px;">-</div>
        <div class="grid-item2">DESIGN</div>
        <div class="grid-item3" style="text-align: center; font-family: Courier New; font-weight: bolder; color: red;  padding-top: 7px;">-</div>
        <div class="grid-item2">WEB/APP</div>
        <div class="grid-item3" style="text-align: center; font-family: Courier New; font-weight: bolder; color: red; padding-top: 7px;">-</div>
        <div class="grid-item2">SOCIAL</div>
        <div class="grid-item3" style="text-align: center; font-family: Courier New; font-weight: bolder; color: red; padding-top: 7px;">-</div>
        <div class="grid-item2">BRANING</div>
    </div>
  <div class="picturezoom">
     <div class="picture">
        <img src="https://www.nhi.sg/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fnhi-le.0cda285c.webp&w=384&q=75" alt="Image 1">
    </div>
    <div class="picture">
        <img src="https://www.nhi.sg/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fms-nhi.e08f7339.jpg&w=384&q=75" alt="Image 2">
    </div>
    <div class="picture">
        <img src="https://www.nhi.sg/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fspice-nice.acb4a540.webp&w=384&q=75" alt="Image 3">
    </div>
    <div class="picture">
        <img src="https://www.nhi.sg/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fjovan-medrano.da47350d.jpeg&w=384&q=75" alt="Image 4">
    </div>
</div>
  <div class="no-line-break">
        <p>ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ</p> <p style="justify-content: center;  font-family: Arial, sans-serif; font-weight: bold; padding: 20px; justify-content: center;" class="highlight-text">ㅤVIEW MORE →ㅤ</p>
    </div>
<br> <br> <br> <br>
<div class="khung">
  <p style="font-size: 15px; font-family: arial; color: red;font-weight: BOLD; line-height: 0.1; padding-left:13%; padding-top:2%;">CUSTOMERS TALK ABOUT US</p>
<div class="teacher">
<div>
       <p style="font-size: 40px; font-family: Arial, sans-serif; font-weight: bold; color: black; line-height: 0.2; padding-top:-50px;">MICHAEL LE</p>
<p style="line-height: 1.5; font-family: Arial; padding-top: 15px;font-size: 17px; color: #555555; text-align: justify;">After partnering up with NhiLe team my business has taken a quick positive turn. With a team full of talented individuals that are all, even though already on top of their profession, eager to learn and improve themselves every day. All with their own unique skill set they will, when combined, inevitably create greatness for you.<br>
NhiLe team has helped my business to accelerate and grow really fast on social media platforms by offering and delivering professional management and modern techniques to create content and make sure my business will keep up with this fast growing online marketing industry.<br>
My business and life has changed a lot after teaming up and I feel so grateful that our path has crossed. Outstanding methods on top of excellent teamwork equals extraordinary results.
      </p></div>
    <div class="column2">
        <img src="https://www.nhi.sg/_next/static/media/michael-le-large.42f6ab75.webp" alt="Michael Le">
    </div>
    <div class="column3">
        <img src="https://www.nhi.sg/_next/static/media/michael-le-small.f4bc3c1f.webp" alt="Michael Le Small">
    </div>
</div>
</div>
<div class="demuc">
    <div class="cell" style="padding-left:3%;">
    <p class="no-effect" style="font-size: 25px; font-weight: BOLD; color:black;">SERVICES</p>
    <p>Digital Marketing</p>
    <p>Video Editor</p>
    <p>Graphic Design</p>
    <p>Website & App Development</p>
    <p>Social Media Support</p>
  </div>
    <div class="cell">
    <p class="no-effect" style="font-size: 25px; font-weight: BOLD; color:black;">OUR PAGES</p>
    <p>Free Training</p>
    <p>About Us</p>
    <p>Private Coaching</p>
  </div>
    <div class="cell">
    <p class="no-effect" style="font-size: 25px; font-weight: BOLD; color:black;">SUPPORT</p>
    <p>Contact</p>
    <p>Privacy</p>
    <p>FAQ</p>
    <p>Terms</p>
  </div>
    <div class="cell">
    <p class="no-effect" style="font-size: 25px; font-weight: BOLD; color:black;">REGISTER</p>
    <p>Nhi's House Members</p>
    <p>NhiLe Team Volunteers</p>
    <p>NhiLe Ebook For FREE</p>
    <p>Website Feedback</p>
  </div>
</div>
<footer class="footer">
    <div class="social-icons">
      <img style="margin-left: 0;" src="https://www.nhi.sg/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Flogo.561b301a.png&w=128&q=75" class="nhile">
      <p>ㅤ©2024. All rights reserved</p>
      <p>ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ</p>
         <a href="https://www.youtube.com/c/NHILELifecoach" target="_blank" class="social-icon">
            <img src="https://cdn-icons-png.freepik.com/256/3670/3670147.png" alt="Logo">
        </a>
        <a href="https://www.facebook.com/AnneNhiLe" target="_blank" class="social-icon">
            <img src="https://www.facebook.com/images/fb_icon_325x325.png" alt="Logo">
        </a>
        <a href="https://www.tiktok.com/@nhile_official" target="_blank" class="social-icon">
            <img src="https://i.pinimg.com/originals/53/6b/f6/536bf6ce27c9da001fa7ff45af393693.png" alt="Logo">
        </a>
        <a href="https://www.instagram.com/nhi_sg/" target="_blank" class="social-icon">
            <img src="https://png.pngtree.com/png-clipart/20230401/original/pngtree-three-dimensional-instagram-icon-png-image_9015419.png" alt="Logo">
        </a>
        <a href="https://telegram.me/your_channel" target="_blank" class="social-icon">
            <img src="link_to_telegram_logo_image" alt="Logo">
        </a>
        <a href="https://t.me/nhileofficial" target="_blank" class="social-icon">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Telegram_2019_Logo.svg/1200px-Telegram_2019_Logo.svg.png" alt="Logo">
        </a>
        <a href="https://open.spotify.com/show/075oMTANwNWPZpQgvwh674?si=aa25bcf2f4c848ee&nd=1&dlsi=0ab39312d30f4786" target="_blank" class="social-icon">
            <img src="https://upload.wikimedia.org/wikipedia/commons/9/9b/Spotify_1.png" alt="Logo">
        </a>
        <a href="https://www.linkedin.com/company/nhile/" target="_blank" class="social-icon">
            <img src="https://www.mhe-sme.org/wp-content/uploads/2017/12/linkedin-icon.png" alt="Logo">
        </a>
      </div>
    </div>
</footer>
</body>
</html>
