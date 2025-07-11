# belajar-git

Belajar git yang menyenangkan!

Saya sedang belajar GitHub
Di MCI Devisi Protik

Kode website devisi programming sederhana:

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>UKM MCI - Divisi Programming</title>
    <base target="_self" />
    <!-- Bootstrap 5 CSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <!-- Font Awesome -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    />
    <style>
      :root {
        --mci-primary: #2c3e50;
        --mci-secondary: #3498db;
        --mci-accent: #e74c3c;
      }

      body {
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        scroll-behavior: smooth;
      }

      .navbar {
        background-color: var(--mci-primary);
      }

      .navbar-brand img {
        height: 40px;
      }

      .hero-section {
        background: linear-gradient(
          135deg,
          var(--mci-primary),
          var(--mci-secondary)
        );
        color: white;
        padding: 100px 0;
      }

      .section-title {
        position: relative;
        margin-bottom: 40px;
        color: var(--mci-primary);
      }

      .section-title:after {
        content: "";
        position: absolute;
        bottom: -10px;
        left: 50%;
        transform: translateX(-50%);
        width: 80px;
        height: 3px;
        background-color: var(--mci-secondary);
      }

      .program-card {
        border: none;
        border-radius: 10px;
        overflow: hidden;
        transition: transform 0.3s, box-shadow 0.3s;
        height: 100%;
      }

      .program-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
      }

      .program-card .card-img-top {
        height: 180px;
        object-fit: cover;
      }

      .program-card .card-body {
        background-color: white;
      }

      .program-card .card-footer {
        background-color: var(--mci-primary);
        color: white;
      }

      .team-member {
        text-align: center;
        margin-bottom: 30px;
      }

      .team-member img {
        width: 150px;
        height: 150px;
        object-fit: cover;
        border-radius: 50%;
        border: 5px solid var(--mci-secondary);
        margin-bottom: 15px;
      }

      .contact-info {
        background-color: #f8f9fa;
        border-radius: 10px;
        padding: 30px;
        height: 100%;
      }

      .contact-info i {
        font-size: 24px;
        color: var(--mci-secondary);
        margin-bottom: 15px;
      }

      footer {
        background-color: var(--mci-primary);
        color: white;
        padding: 30px 0;
      }

      .social-icons a {
        color: white;
        font-size: 20px;
        margin: 0 10px;
        transition: color 0.3s;
      }

      .social-icons a:hover {
        color: var(--mci-secondary);
      }
    </style>
  </head>
  <body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark sticky-top">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img
            src="https://via.placeholder.com/150x50?text=UKM+MCI"
            alt="UKM MCI Logo"
          />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link active" href="#home">Beranda</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#about">Tentang</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#programs">Program</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#team">Tim</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Kontak</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section">
      <div class="container text-center">
        <h1 class="display-4 fw-bold mb-4">Divisi Programming UKM MCI</h1>
        <p class="lead mb-5">
          Mengembangkan skill programming melalui kolaborasi dan inovasi
        </p>
        <a href="#programs" class="btn btn-light btn-lg px-4 me-2"
          >Program Kami</a
        >
        <a href="#contact" class="btn btn-outline-light btn-lg px-4"
          >Gabung Sekarang</a
        >
      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-5">
      <div class="container">
        <h2 class="text-center section-title">Tentang Divisi Programming</h2>
        <div class="row align-items-center">
          <div class="col-lg-6 mb-4 mb-lg-0">
            <img
              src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"
              alt="Programming Team"
              class="img-fluid rounded"
            />
          </div>
          <div class="col-lg-6">
            <h3 class="mb-3">Mengapa Bergabung dengan Divisi Programming?</h3>
            <p>
              Divisi Programming UKM MCI merupakan wadah bagi mahasiswa yang
              tertarik dalam pengembangan perangkat lunak untuk belajar,
              berkolaborasi, dan mengembangkan proyek-proyek inovatif bersama.
            </p>
            <ul class="list-unstyled">
              <li class="mb-2">
                <i class="fas fa-check-circle text-primary me-2"></i> Belajar
                teknologi terbaru dalam dunia programming
              </li>
              <li class="mb-2">
                <i class="fas fa-check-circle text-primary me-2"></i> Kesempatan
                mengerjakan proyek nyata
              </li>
              <li class="mb-2">
                <i class="fas fa-check-circle text-primary me-2"></i> Networking
                dengan sesama programmer
              </li>
              <li class="mb-2">
                <i class="fas fa-check-circle text-primary me-2"></i> Persiapan
                untuk kompetisi dan dunia kerja
              </li>
            </ul>
            <div class="mt-4">
              <a href="#" class="btn btn-primary me-2">Visi & Misi</a>
              <a href="#" class="btn btn-outline-primary"
                >Struktur Organisasi</a
              >
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Programs Section -->
    <section id="programs" class="py-5 bg-light">
      <div class="container">
        <h2 class="text-center section-title">Program Unggulan</h2>
        <div class="row g-4">
          <div class="col-md-4">
            <div class="program-card card">
              <img
                src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"
                class="card-img-top"
                alt="Weekly Workshop"
              />
              <div class="card-body">
                <h5 class="card-title">Weekly Workshop</h5>
                <p class="card-text">
                  Sesi belajar mingguan membahas berbagai topik programming
                  mulai dari dasar hingga advanced dengan pendekatan praktis.
                </p>
              </div>
              <div class="card-footer text-center">
                <small>Setiap Jumat, 16.00 - 18.00 WIB</small>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="program-card card">
              <img
                src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"
                class="card-img-top"
                alt="Project Collaboration"
              />
              <div class="card-body">
                <h5 class="card-title">Project Collaboration</h5>
                <p class="card-text">
                  Kolaborasi dalam pengembangan proyek nyata untuk mengasah
                  kemampuan tim dan portofolio anggota.
                </p>
              </div>
              <div class="card-footer text-center">
                <small>Terbuka untuk semua anggota</small>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="program-card card">
              <img
                src="https://images.unsplash.com/photo-1531482615713-2afd69097998?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"
                class="card-img-top"
                alt="Hackathon & Competition"
              />
              <div class="card-body">
                <h5 class="card-title">Hackathon & Competition</h5>
                <p class="card-text">
                  Persiapan dan partisipasi dalam kompetisi programming baik
                  tingkat regional maupun nasional.
                </p>
              </div>
              <div class="card-footer text-center">
                <small>Event berkala</small>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Team Section -->
    <section id="team" class="py-5">
      <div class="container">
        <h2 class="text-center section-title">Tim Kami</h2>
        <div class="row">
          <div class="col-md-4">
            <div class="team-member">
              <img
                src="https://randomuser.me/api/portraits/men/32.jpg"
                alt="Ketua Divisi"
              />
              <h4>John Doe</h4>
              <p class="text-muted">Ketua Divisi</p>
              <p>
                Full-stack Developer dengan pengalaman 3 tahun di industri
                teknologi.
              </p>
              <div>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-linkedin"></i
                ></a>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-github"></i
                ></a>
                <a href="#" class="text-primary"
                  ><i class="fas fa-envelope"></i
                ></a>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="team-member">
              <img
                src="https://randomuser.me/api/portraits/women/44.jpg"
                alt="Sekretaris"
              />
              <h4>Jane Smith</h4>
              <p class="text-muted">Sekretaris</p>
              <p>
                Mobile Developer spesialisasi Android dengan passion di UI/UX.
              </p>
              <div>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-linkedin"></i
                ></a>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-github"></i
                ></a>
                <a href="#" class="text-primary"
                  ><i class="fas fa-envelope"></i
                ></a>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="team-member">
              <img
                src="https://randomuser.me/api/portraits/men/75.jpg"
                alt="Koordinator Proyek"
              />
              <h4>Robert Johnson</h4>
              <p class="text-muted">Koordinator Proyek</p>
              <p>
                Data Scientist dengan keahlian dalam Python dan machine
                learning.
              </p>
              <div>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-linkedin"></i
                ></a>
                <a href="#" class="text-primary me-2"
                  ><i class="fab fa-github"></i
                ></a>
                <a href="#" class="text-primary"
                  ><i class="fas fa-envelope"></i
                ></a>
              </div>
            </div>
          </div>
        </div>
        <div class="text-center mt-4">
          <a href="#" class="btn btn-outline-primary">Lihat Seluruh Anggota</a>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-5 bg-light">
      <div class="container">
        <h2 class="text-center section-title">Hubungi Kami</h2>
        <div class="row g-4">
          <div class="col-lg-4">
            <div class="contact-info text-center">
              <i class="fas fa-map-marker-alt"></i>
              <h4>Lokasi</h4>
              <p>
                Gedung Student Center Lt. 3<br />Universitas Contoh<br />Jalan
                Pendidikan No. 123
              </p>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="contact-info text-center">
              <i class="fas fa-envelope"></i>
              <h4>Email</h4>
              <p>programming@ukmmci.ac.id<br />ukmmci@example.ac.id</p>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="contact-info text-center">
              <i class="fas fa-phone-alt"></i>
              <h4>Telepon</h4>
              <p>+62 812 3456 7890 (Admin)<br />+62 823 4567 8901 (Ketua)</p>
            </div>
          </div>
        </div>

        <div class="row mt-5">
          <div class="col-lg-6 mx-auto">
            <div class="card shadow-sm">
              <div class="card-body">
                <h4 class="card-title text-center mb-4">
                  Formulir Pendaftaran
                </h4>
                <form>
                  <div class="mb-3">
                    <label for="name" class="form-label">Nama Lengkap</label>
                    <input
                      type="text"
                      class="form-control"
                      id="name"
                      required
                    />
                  </div>
                  <div class="mb-3">
                    <label for="email" class="form-label">Email</label>
                    <input
                      type="email"
                      class="form-control"
                      id="email"
                      required
                    />
                  </div>
                  <div class="mb-3">
                    <label for="npm" class="form-label">NPM</label>
                    <input type="text" class="form-control" id="npm" required />
                  </div>
                  <div class="mb-3">
                    <label for="major" class="form-label">Jurusan</label>
                    <input
                      type="text"
                      class="form-control"
                      id="major"
                      required
                    />
                  </div>
                  <div class="mb-3">
                    <label for="experience" class="form-label"
                      >Pengalaman Programming</label
                    >
                    <textarea
                      class="form-control"
                      id="experience"
                      rows="3"
                    ></textarea>
                  </div>
                  <div class="d-grid">
                    <button type="submit" class="btn btn-primary">
                      Daftar Sekarang
                    </button>
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="text-center">
      <div class="container">
        <div class="social-icons mb-4">
          <a href="#"><i class="fab fa-facebook-f"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
          <a href="#"><i class="fab fa-linkedin-in"></i></a>
          <a href="#"><i class="fab fa-github"></i></a>
        </div>
        <p class="mb-2">
          UKM MCI - Unit Kegiatan Mahasiswa Komputer dan Informatika
        </p>
        <p class="mb-0">
          &copy; 2023 Divisi Programming UKM MCI. All Rights Reserved.
        </p>
      </div>
    </footer>

    <!-- Bootstrap 5 JS Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
      // Smooth scrolling for anchor links
      document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
        anchor.addEventListener("click", function (e) {
          e.preventDefault();

          document.querySelector(this.getAttribute("href")).scrollIntoView({
            behavior: "smooth",
          });
        });
      });

      // Navbar background change on scroll
      window.addEventListener("scroll", function () {
        const navbar = document.querySelector(".navbar");
        if (window.scrollY > 50) {
          navbar.style.boxShadow = "0 2px 10px rgba(0,0,0,0.1)";
          navbar.style.backgroundColor = "var(--mci-primary)";
        } else {
          navbar.style.boxShadow = "none";
          navbar.style.backgroundColor = "var(--mci-primary)";
        }
      });
    </script>
  </body>
</html>
```
