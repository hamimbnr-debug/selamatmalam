html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Saya</title>
    <style>
        /* Reset dan Gaya Dasar */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }

        /* Header dan Navigasi */
        header {
            background-color: #2c3e50;
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        .nav-links {
            display: flex;
            list-style: none;
        }

        .nav-links li {
            margin-left: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #3498db;
        }

        /* Bagian Hero */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(135deg, #3498db, #2c3e50);
            color: white;
            margin-top: 60px;
        }

        .hero-content h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background-color: #e74c3c;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #c0392b;
        }

        /* Bagian Tentang */
        .about {
            padding: 5rem 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2rem;
            color: #2c3e50;
        }

        .about-content {
            display: flex;
            align-items: center;
            gap: 2rem;
        }

        .about-text {
            flex: 1;
        }

        .about-image {
            flex: 1;
            text-align: center;
        }

        .about-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        /* Bagian Layanan */
        .services {
            padding: 5rem 0;
            background-color: #f9f9f9;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
            transition: transform 0.3s;
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-icon {
            font-size: 3rem;
            color: #3498db;
            margin-bottom: 1rem;
        }

        /* Bagian Portofolio */
        .portfolio {
            padding: 5rem 0;
            background-color: white;
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .portfolio-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .portfolio-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .portfolio-item:hover img {
            transform: scale(1.1);
        }

        .portfolio-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background-color: rgba(44, 62, 80, 0.8);
            color: white;
            padding: 1rem;
            transform: translateY(100%);
            transition: transform 0.3s;
        }

        .portfolio-item:hover .portfolio-overlay {
            transform: translateY(0);
        }

        /* Bagian Kontak */
        .contact {
            padding: 5rem 0;
            background-color: #2c3e50;
            color: white;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 0.8rem;
            border: none;
            border-radius: 5px;
        }

        .form-group textarea {
            height: 150px;
        }

        /* Footer */
        footer {
            background-color: #1a252f;
            color: white;
            text-align: center;
            padding: 2rem 0;
        }

        /* Responsif */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero-content h1 {
                font-size: 2rem;
            }

            .about-content {
                flex-direction: column;
            }

            .about-image {
                order: -1;
            }
        }
    </style>
</head>
<body>
    <!-- Header dan Navigasi -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">Portofolio</div>
                <ul class="nav-links">
                    <li><a href="#home">Beranda</a></li>
                    <li><a href="#about">Tentang</a></li>
                    <li><a href="#services">Layanan</a></li>
                    <li><a href="#portfolio">Portofolio</a></li>
                    <li><a href="#contact">Kontak</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Bagian Hero -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Halo, Saya John Doe</h1>
                <p>Seorang Web Developer & Desainer Grafis</p>
                <a href="#portfolio" class="btn">Lihat Portofolio</a>
            </div>
        </div>
    </section>

    <!-- Bagian Tentang -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">Tentang Saya</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Saya adalah seorang web developer dengan pengalaman lebih dari 5 tahun dalam mengembangkan website dan aplikasi web. Saya memiliki keahlian dalam HTML, CSS, JavaScript, dan berbagai framework modern.</p>
                    <p>Saya sangat antusias dalam menciptakan pengalaman digital yang menarik dan fungsional untuk pengguna. Saya selalu berusaha untuk tetap update dengan teknologi terbaru dan tren desain.</p>
                </div>
                <div class="about-image">
                    <img src="https://via.placeholder.com/400x300" alt="Foto Profil">
                </div>
            </div>
        </div>
    </section>

    <!-- Bagian Layanan -->
    <section id="services" class="services">
        <div class="container">
            <h2 class="section-title">Layanan Saya</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">💻</div>
                    <h3>Web Development</h3>
                    <p>Membangun website responsif dan aplikasi web dengan teknologi terbaru.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🎨</div>
                    <h3>UI/UX Design</h3>
                    <p>Mendesain antarmuka yang menarik dan pengalaman pengguna yang optimal.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📱</div>
                    <h3>Mobile Apps</h3>
                    <p>Mengembangkan aplikasi mobile untuk platform iOS dan Android.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Bagian Portofolio -->
    <section id="portfolio" class="portfolio">
        <div class="container">
            <h2 class="section-title">Portofolio Saya</h2>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <img src="https://via.placeholder.com/400x300" alt="Proyek 1">
                    <div class="portfolio-overlay">
                        <h3>Website E-commerce</h3>
                        <p>Toko online dengan sistem pembayaran terintegrasi</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://via.placeholder.com/400x300" alt="Proyek 2">
                    <div class="portfolio-overlay">
                        <h3>Aplikasi Manajemen</h3>
                        <p>Sistem manajemen inventaris untuk bisnis kecil</p>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://via.placeholder.com/400x300" alt="Proyek 3">
                    <div class="portfolio-overlay">
                        <h3>Website Perusahaan</h3>
                        <p>Situs web perusahaan dengan desain modern</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Bagian Kontak -->
    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title">Hubungi Saya</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Nama</label>
                        <input type="text" id="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Pesan</label>
                        <textarea id="message" required></textarea>
                    </div>
                    <button type="submit" class="btn">Kirim Pesan</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2023 Portofolio Saya. Semua Hak Dilindungi.</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling untuk navigasi
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Efek transparan header saat scroll
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.backgroundColor = 'rgba(44, 62, 80, 0.9)';
            } else {
                header.style.backgroundColor = '#2c3e50';
            }
        });
    </script>
</body>
</html>
