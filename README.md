<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Portfolio Cá Nhân</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- MENU -->
  <header>
    <nav class="navbar">
      <h1 class="logo">My Portfolio</h1>
      <ul>
        <li><a href="#home">Trang chủ</a></li>
        <li><a href="#about">Giới thiệu</a></li>
        <li><a href="#skills">Kỹ năng</a></li>
        <li><a href="#projects">Dự án</a></li>
        <li><a href="#contact">Liên hệ</a></li>
      </ul>
    </nav>
  </header>

  <!-- HOME -->
  <section id="home" class="section home">
    <h2>Xin chào, mình là</h2>
    <h1>[Tên của bạn]</h1>
    <p>Sinh viên | Ứng viên ngành Du lịch | Sale Tour</p>
  </section>

  <!-- ABOUT -->
  <section id="about" class="section">
    <h2>Giới thiệu bản thân</h2>
    <p>
      Tôi là sinh viên ngành Du lịch, có định hướng phát triển trong lĩnh vực
      kinh doanh tour và chăm sóc khách hàng. Tôi yêu thích ứng dụng công nghệ
      và AI trong học tập và công việc.
    </p>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="section gray">
    <h2>Kỹ năng</h2>
    <ul class="skills-list">
      <li>Thiết kế chương trình tour</li>
      <li>Tư vấn và bán tour du lịch</li>
      <li>Word, Excel, PowerPoint</li>
      <li>Canva, AI (ChatGPT)</li>
    </ul>
  </section>

  <!-- PROJECTS -->
  <section id="projects" class="section">
    <h2>Dự án & Portfolio</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Tour Cần Thơ – Phú Quốc</h3>
        <p>Xây dựng chương trình tour 4N3Đ và tính giá tour.</p>
      </div>
      <div class="project-card">
        <h3>Bài nghiên cứu du lịch bền vững</h3>
        <p>Phân tích phát triển du lịch tại Kỳ Co.</p>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section gray">
    <h2>Liên hệ</h2>
    <p>Email: yourname@gmail.com</p>
    <p>Điện thoại: 0xxx xxx xxx</p>
  </section>

  <footer>
    <p>© 2026 - Website cá nhân</p>
  </footer>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

header {
  background: #0a58ca;
  padding: 15px 0;
}

.navbar {
  width: 90%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  color: #fff;
}

.navbar ul {
  list-style: none;
  display: flex;
}

.navbar ul li {
  margin-left: 20px;
}

.navbar ul li a {
  color: #fff;
  text-decoration: none;
}

.section {
  padding: 60px 10%;
}

.gray {
  background: #f4f4f4;
}

.home {
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.skills-list {
  margin-top: 20px;
}

.skills-list li {
  margin-bottom: 10px;
}

.projects {
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

.project-card {
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  width: 50%;
}

footer {
  text-align: center;
  padding: 15px;
  background: #0a58ca;
  color: #fff;
}

/* RESPONSIVE */
@media (max-width: 768px) {
  .navbar ul {
    flex-direction: column;
  }

  .projects {
    flex-direction: column;
  }

  .project-card {
    width: 100%;
  }
}document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();
    document.querySelector(this.getAttribute('href'))
      .scrollIntoView({
        behavior: 'smooth'
      });
  });
});
  <script src="script.js"></script>
</body>
</html>
