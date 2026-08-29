ali
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقعي الشخصي</title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Cairo', sans-serif;
            scroll-behavior: smooth;
        }
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        /* القائمة العلوية */
        header {
            background: #ffffff;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
        }
        .nav-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }
        .logo {
            font-weight: 700;
            font-size: 20px;
            color: #007BFF;
        }
        .nav-links {
            list-style: none;
            display: flex;
            gap: 20px;
        }
        .nav-links a {
            text-decoration: none;
            color: #555;
            font-weight: 600;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: #007BFF;
        }

        /* تنسيق الأقسام العامة */
        section {
            padding: 100px 20px 60px 20px;
            max-width: 900px;
            margin: 0 auto;
            text-align: center;
        }
        h2 {
            font-size: 28px;
            margin-bottom: 20px;
            color: #222;
            position: relative;
        }
        h2::after {
            content: '';
            width: 50px;
            height: 3px;
            background-color: #007BFF;
            display: block;
            margin: 8px auto 0 auto;
            border-radius: 2px;
        }

        /* قسم الهيرو (البداية) */
        .hero {
            background: linear-gradient(135deg, #007BFF, #0056b3);
            color: white;
            padding: 140px 20px 80px 20px;
            text-align: center;
        }
        .profile-img {
            width: 140px;
            height: 140px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid #fff;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        .hero h1 {
            font-size: 32px;
            margin-bottom: 10px;
        }
        .hero p {
            font-size: 18px;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto 25px auto;
        }
        .btn-main {
            display: inline-block;
            background: #fff;
            color: #007BFF;
            padding: 10px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            transition: transform 0.3s, background 0.3s;
        }
        .btn-main:hover {
            transform: translateY(-3px);
            background: #f1f1f1;
        }

        /* المهارات */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        .skill-card {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            font-weight: 600;
            color: #444;
        }

        /* معرض الأعمال */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        .project-card {
            background: #fff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            text-align: right;
        }
        .project-content {
            padding: 20px;
        }
        .project-content h3 {
            font-size: 18px;
            margin-bottom: 10px;
            color: #222;
        }
        .project-content p {
            font-size: 14px;
            color: #666;
            margin-bottom: 15px;
        }
        .project-link {
            color: #007BFF;
            text-decoration: none;
            font-weight: 700;
            font-size: 14px;
        }

        /* قسم التواصل */
        .contact-box {
            background: #fff;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            margin-top: 20px;
        }
        .social-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }
        .social-btn {
            background: #007BFF;
            color: #fff;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-size: 14px;
            transition: background 0.3s;
        }
        .social-btn:hover {
            background: #0056b3;
        }

        /* الفوتر */
        footer {
            text-align: center;
            padding: 20px;
            background: #222;
            color: #aaa;
            font-size: 14px;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">موقعي</div>
            <ul class="nav-links">
                <li><a href="#about">عني</a></li>
                <li><a href="#skills">مهاراتي</a></li>
                <li><a href="#projects">أعمالي</a></li>
                <li><a href="#contact">تواصل معي</a></li>
            </ul>
        </div>
    </header>

    <div class="hero">
        <img src="https://via.placeholder.com/140" alt="صورتك الشخصية" class="profile-img">
        <h1>علي بن عبدالعزيز الزايدي</h1>
        <p>مرحباً بك في موقعي الشخصي. أنا شخص شغوف بالتكنولوجيا والتطوير المستمر.</p>
        <a href="#contact" class="btn-main">تواصل معي</a>
    </div>

    <section id="about">
        <h2>نبذة عني</h2>
        <p>أنا علي بن عبدالعزيز الزايدي، مهندس برمجيات مختص في تطوير الويب وتصميم واجهات المستخدم. لدي خبرة في استخدام أحدث التقنيات لخلق تجارب مستخدم excepcional.</p>
    </section>

    <section id="skills">
        <h2>مهاراتي</h2>
        <div class="skills-grid">
            <div class="skill-card">تصميم واجهات المستخدم</div>
            <div class="skill-card">تطوير الويب (HTML/CSS)</div>
            <div class="skill-card">حل المشكلات</div>
            <div class="skill-card">إدارة المشاريع</div>
        </div>
    </section>

    <section id="projects">
        <h2>معرض أعمالي</h2>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-content">
                    <h3>انشاء موقع اكتروني</h3>
                    <pالموقع عبارة عن كلام عني ووش ممكن افعل بالمستقبل القريب ان شاءالله و</p>
                    <a href="#" class="project-link">عرض المشروع &larr;</a>
                </div>
            </div>
            <div class="project-card">
                <div class="project-content">
                    <h3>لعبة</h3>
                    <p>لم ابدا بعد</p>
                    <a href="#" class="project-link">عرض المشروع &larr;</a>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>تواصل معي</h2>
        <div class="contact-box">
            <p>يسعدني تواصلك معي عبر منصات التواصل الاجتماعي أو البريد الإلكتروني:</p>
            <div class="social-buttons">
                <a href="https://twitter.com" target="_blank" class="social-btn">تويتر (X)</a>
                <a href="https://linkedin.com" target="_blank" class="social-btn">لينكد إن</a>
                <a href="mailto:example@email.com" class="social-btn">البريد الإلكتروني</a>
            </div>
        </div>
    </section>

    <footer>
        <p>جميع الحقوق محفوظة &copy; 2026 - علي بن عبدالعزيز الزايدي</p>
    </footer>

</body>
</html>
