<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      phone: "",
      message: "",
      submitted: false,
      entries: [],
    };
  },
  methods: {
    submitForm(event) {
      event.preventDefault();

      // Menyimpan hasil input dalam tabel
      const formData = {
        name: this.name,
        email: this.email,
        phone: this.phone,
        message: this.message,
      };
      this.entries.push(formData);

      // Cetak di console.log
      console.log(formData);

      // Reset form setelah mengirim
      this.resetForm();
    },
    resetForm() {
      // Reset nilai form setelah mengirim
      this.name = "";
      this.email = "";
      this.phone = "";
      this.message = "";
      this.submitted = true;
    },
  },
};
</script>

<template>
  <i class="bi bi-list mobile-nav-toggle d-lg-none"></i>
  <!-- Codingan Navbar -->
  <header id="header" class="d-flex flex-column justify-content-center">
    <nav id="navbar" class="navbar nav-menu">
      <ul>
        <li>
          <a href="#hero" class="nav-link scrollto active"
            ><i class="bx bx-home"></i> <span>Home</span></a
          >
        </li>
        <li>
          <a href="#about" class="nav-link scrollto"
            ><i class="bx bx-user"></i> <span>About</span></a
          >
        </li>
        <li>
          <a href="#resume" class="nav-link scrollto"
            ><i class="bx bx-file-blank"></i> <span>Resume</span></a
          >
        </li>
        <li>
          <a href="#portfolio" class="nav-link scrollto"
            ><i class="bx bx-book-content"></i> <span>Portfolio</span></a
          >
        </li>
        <li>
          <a href="#task" class="nav-link scrollto"
            ><i class="bx bx-task"></i> <span>Task/Tugas</span></a
          >
        </li>
        <li>
          <a href="#contact" class="nav-link scrollto"
            ><i class="bx bx-envelope"></i> <span>Contact</span></a
          >
        </li>
      </ul>
    </nav>
    <!-- .nav-menu -->
  </header>
  <!-- End Header -->
  <!-- Akhir Codingan Navbar -->

  <!-- Codingan Data diri -->
  <!-- ======= Hero Section ======= -->
  <section id="hero" class="d-flex flex-column justify-content-center">
    <div class="container" data-aos="zoom-in" data-aos-delay="100">
      <h1>Raihan Muhammad Saprudin</h1>
      <p>
        I'm
        <span
          class="typed"
          data-typed-items="Undergraduate at STMIK Mardira Indonesia, Junior Electrical Engineering, Hardware Engineering, IoT Engineering"
        ></span>
      </p>
      <div class="social-links">
        <a
          href="https://web.facebook.com/profile.php?id=100016967735048"
          target="_blank"
          class="facebook"
          ><i class="bx bxl-facebook"></i
        ></a>
        <a
          href="https://www.instagram.com/raihanm0607"
          target="_blank"
          class="instagram"
          ><i class="bx bxl-instagram"></i
        ></a>
        <a href="https://github.com/fsociety781" target="_blank" class="github"
          ><i class="bx bxl-github"></i
        ></a>
        <a
          href="https://www.linkedin.com/in/raihanms07/"
          target="_blank"
          class="linkedin"
          ><i class="bx bxl-linkedin"></i
        ></a>
      </div>
    </div>
  </section>
  <!-- End Hero -->
  <!-- Akhir Codingan Data diri -->

  <main id="main">
    <!-- ======= About Section ======= -->
    <section id="about" class="about">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>About</h2>
          <p>
            Saya Raihan Muhammad Saprudin seorang Undergraduate dari STMIK
            Mardira Indonesia jurusan Teknik Informatika dengan passion besar
            untuk bisa berkarier di bidang Internet Of Things, Hardware dan Web
            Development.Saya tertarik terhadap Internet of Things, telah
            memiliki pengalaman pembuatan project IoT baik tim maupun individu,
            menekuni bidang IoT Hardware dan Elektronika, serta Pemrograman Web
            untuk mengintegrasikan Alat IoT yang dibuat. Saat ini sedang
            mempelajari Software Engineering agar dapat mengembangkan project
            IoT yang mengikuti perkembangan teknologi terkini.
          </p>
        </div>
        <div class="row">
          <div class="col-lg-4">
            <img src="../assets/img/Raihan.png" class="img-fluid" alt="" />
          </div>
          <div class="col-lg-8 pt-4 pt-lg-0 content">
            <h3>Electrical, Hardware &amp; IoT Engineering.</h3>
            <!-- <p class="fst-italic">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
              magna aliqua.
            </p> -->
            <div class="row">
              <div class="col-lg-6">
                <ul>
                  <li>
                    <i class="bi bi-chevron-right"></i>
                    <strong>Birthday:</strong> <span>6 Juli 2002</span>
                  </li>
                  <li>
                    <i class="bi bi-chevron-right"></i> <strong>Phone:</strong>
                    <span>089516011186</span>
                  </li>
                  <li>
                    <i class="bi bi-chevron-right"></i> <strong>City:</strong>
                    <span>Bandung, Jawa Brat</span>
                  </li>
                </ul>
              </div>
              <div class="col-lg-6">
                <ul>
                  <li>
                    <i class="bi bi-chevron-right"></i> <strong>Age:</strong>
                    <span>20</span>
                  </li>
                  <li>
                    <i class="bi bi-chevron-right"></i> <strong>Email:</strong>
                    <span>raihanmuhammadsaprudin898@gmail.com.</span>
                  </li>
                  <li>
                    <i class="bi bi-chevron-right"></i>
                    <strong>Freelance:</strong> <span>Available</span>
                  </li>
                </ul>
              </div>
            </div>
            <!-- <p>
              Officiis eligendi itaque labore et dolorum mollitia officiis optio vero. Quisquam sunt adipisci omnis et ut. Nulla accusantium dolor incidunt officia tempore. Et eius omnis.
              Cupiditate ut dicta maxime officiis quidem quia. Sed et consectetur qui quia repellendus itaque neque. Aliquid amet quidem ut quaerat cupiditate. Ab et eum qui repellendus omnis culpa magni laudantium dolores.
            </p> -->
          </div>
        </div>
      </div>
    </section>
    <!-- End About Section -->

    <!-- ======= Skills Section ======= -->
    <section id="skills" class="skills section-bg">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Skills</h2>
          <p>
            Keahlian: Program Arduino, PHP, Web Development,Electrical dan
            Hardware Engineering,IoT Technician, Leadership, Planning, Teamwork.
          </p>
        </div>

        <div class="row skills-content">
          <div class="col-lg-6">
            <div class="progress">
              <span class="skill">HTML <i class="val">80%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="100"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">CSS <i class="val">30%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="90"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">JavaScript <i class="val">20%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="75"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">Arduino Code <i class="val">70%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="75"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">PHP <i class="val">70%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="75"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>
          </div>

          <div class="col-lg-6">
            <div class="progress">
              <span class="skill">IoT Developed<i class="val">90%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="80"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill"
                >Hardware dan Robotik<i class="val">70%</i></span
              >
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="80"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">Electrical <i class="val">70%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="90"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">Eagel <i class="val">70%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="55"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>

            <div class="progress">
              <span class="skill">kicad <i class="val">70%</i></span>
              <div class="progress-bar-wrap">
                <div
                  class="progress-bar"
                  role="progressbar"
                  aria-valuenow="55"
                  aria-valuemin="0"
                  aria-valuemax="100"
                ></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- End Skills Section -->

    <!-- ======= Resume Section ======= -->
    <section id="resume" class="resume">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Resume</h2>
          <p>
            Di bawah ini merupakan ringkasan tentang saya, riwayat pendidikan
            saya dan pengalaman saya pada saat magang di perusahaan.
          </p>
        </div>

        <div class="row">
          <div class="col-lg-6">
            <h3 class="resume-title">Sumary</h3>
            <div class="resume-item pb-0">
              <h4>Raihan Muhammad Saprudin</h4>
              <p>
                <em
                  >Seorang Mahasiswa Rekayasa Perangkat Lunak memiliki
                  pengalaman magang sebagai Staff Officer dan Electrical
                  Engineering. Memiliki jiwa kepemimpinan dan dapat bekerja
                  secara mandiri maupun dalam tim.</em
                >
              </p>
              <ul>
                <li>Kp.Babkan Nanjung, Kab.Bandung, Jawa Barat</li>
                <li>089516011186</li>
                <li>raihanmuhammadsaprudin898@gmailcom</li>
              </ul>
            </div>

            <h3 class="resume-title">Education</h3>
            <div class="resume-item">
              <h4>Teknik Informatika</h4>
              <h5>September 2020 - Expected 2024</h5>
              <p><em>STMIK Mardira Indonesia</em></p>
              <p>
                Menjadi bagian dari tim Pelopor IoT sebagai Asisten Dosen.
                <br />
                Course Summary : Arsitektur dan Organisai Komputer, Struktur
                Data,Algoritma Pemrograman, Web IoT, Sistem Basis Data, Analisis
                SistemInformasi, Matematika Diskrit.
              </p>
            </div>
            <div class="resume-item">
              <h4>Rekayasa Perangkat Lunak</h4>
              <h5>Juli 2017 - Mei 2020</h5>
              <p><em>SMK Lugina Rancaekek</em></p>
              <p>
                Menjadi Siswa di sekolah tersebut dan mengambil jurusa Rekayasa
                Perangkat Lunak, Menjadi bagian dari Tim program Teaching
                Factory sebagai Hardware and Electrical Technician.
              </p>
            </div>
          </div>
          <div class="col-lg-6">
            <h3 class="resume-title">Experience</h3>
            <div class="resume-item">
              <h4>Electrical Engineering SIB</h4>
              <h5>Agustus - Desember 2022</h5>
              <p><em>PT STECHOQ ROBOTIKA INDONESIA</em></p>
              <ul>
                <li>Merancang Desain Skematik dan Desain Board PCB.</li>
                <li>
                  Mengimplementasikan Mikrokontroller, Sensor dan Akuator dan
                  cara programnya.
                </li>
                <li>Memanfaatkan Website Simulasi Rangkaian IoT.</li>
                <li>Memanfaatkan Software Simulai rangakain Eltronika.</li>
                <li>Merancangan Power supplya pada rangkaian Elektronik.</li>
                <li>
                  Menerapkan Sistem IoT pada bidang pekerjaan di dunia nyata.
                </li>
              </ul>
            </div>
            <div class="resume-item">
              <h4>Staff Officer</h4>
              <h5>Desember 2018 – Februari 2019</h5>
              <p><em>PT.Kewalram Indonesia</em></p>
              <ul>
                <li>Melakukan cek up data absensi karyawan.</li>
                <li>Membuat backup data absensi menjadi digital.</li>
                <li>Melakukan pengarsipan surat masuk dan surat keluar PT</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- End Resume Section -->

    <!-- ======= Portfolio Section ======= -->
    <section id="portfolio" class="portfolio section-bg">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Portfolio</h2>
          <p>
            Berikut dibawah merupakan beberapa Portfolio, dari beberapa projek
            sudah saya selesaikan.
          </p>
        </div>

        <div class="row">
          <div
            class="col-lg-12 d-flex justify-content-center"
            data-aos="fade-up"
            data-aos-delay="100"
          >
            <ul id="portfolio-flters">
              <li data-filter="*" class="filter-active">All</li>
              <li data-filter=".filter-iot">IoT</li>
              <li data-filter=".filter-web">Web</li>
            </ul>
          </div>
        </div>

        <div
          class="row portfolio-container"
          data-aos="fade-up"
          data-aos-delay="200"
        >
          <div class="col-lg-4 col-md-6 portfolio-item filter-iot">
            <div class="portfolio-wrap">
              <img
                src="../assets/img/portfolio/rfidlogin.jpg"
                class="img-fluid"
                alt=""
              />
              <div class="portfolio-info">
                <h4>Smart Presence DoorLock</h4>
                <p>IoT Projek</p>
                <div class="portfolio-links">
                  <a
                    href="../assets/img/portfolio/rfidlogin-1.jpg"
                    data-gallery="portfolioGallery"
                    class="portfolio-lightbox"
                    title="App 1"
                    ><i class="bx bx-plus"></i
                  ></a>
                  <a
                    href="/src/components/SPD.html"
                    class="portfolio-details-lightbox"
                    data-glightbox="type: external"
                    title="Portfolio Details"
                    ><i class="bx bx-link"></i
                  ></a>
                </div>
              </div>
            </div>
          </div>

          <div class="col-lg-4 col-md-6 portfolio-item filter-web">
            <div class="portfolio-wrap">
              <img
                src="../assets/img/portfolio/loginsiswa.png"
                class="img-fluid"
                alt=""
              />
              <div class="portfolio-info">
                <h4>Sistem Informasi Sekolah</h4>
                <p>Projek Web</p>
                <div class="portfolio-links">
                  <a
                    href="../assets/img/portfolio/loginsiswa.png"
                    data-gallery="portfolioGallery"
                    class="portfolio-lightbox"
                    title="Web 3"
                    ><i class="bx bx-plus"></i
                  ></a>
                  <a
                    href="/src/components/Datasiswa.html"
                    class="portfolio-details-lightbox"
                    data-glightbox="type: external"
                    title="Portfolio Details"
                    ><i class="bx bx-link"></i
                  ></a>
                </div>
              </div>
            </div>
          </div>

          <div class="col-lg-4 col-md-6 portfolio-item filter-iot">
            <div class="portfolio-wrap">
              <img
                src="../assets/img/portfolio/Smarthome.png"
                class="img-fluid"
                alt=""
              />
              <div class="portfolio-info">
                <h4>SmartHome</h4>
                <p>Projek IoT</p>
                <div class="portfolio-links">
                  <a
                    href="../assets/img/portfolio/Smarthome.png"
                    data-gallery="portfolioGallery"
                    class="portfolio-lightbox"
                    title="App 2"
                    ><i class="bx bx-plus"></i
                  ></a>
                  <a
                    href="/src/components/SmartHome.html"
                    class="portfolio-details-lightbox"
                    data-glightbox="type: external"
                    title="Portfolio Details"
                    ><i class="bx bx-link"></i
                  ></a>
                </div>
              </div>
            </div>
          </div>

          <div class="col-lg-4 col-md-6 portfolio-item filter-web">
            <div class="portfolio-wrap">
              <img
                src="../assets/img/portfolio/loginpengaduan.png"
                class="img-fluid"
                alt=""
              />
              <div class="portfolio-info">
                <h4>Wesite Pengaduan Masyarakat</h4>
                <p>Projek Web</p>
                <div class="portfolio-links">
                  <a
                    href="../assets/img/portfolio/loginpengaduan.png"
                    data-gallery="portfolioGallery"
                    class="portfolio-lightbox"
                    title="Web 2"
                    ><i class="bx bx-plus"></i
                  ></a>
                  <a
                    href="/src/components/PengaduanView.vue"
                    class="portfolio-details-lightbox"
                    data-glightbox="type: external"
                    title="Portfolio Details"
                    ><i class="bx bx-link"></i
                  ></a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- End Portfolio Section -->

    <!-- ======= Services Section ======= -->
    <section id="task" class="task">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Pengumpulan Tugas</h2>
          <p>Halaman Untuk Pengumpulan Tugas Matkul Basic Web Programming</p>
        </div>

        <div class="row">
          <div
            class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4 mt-md-0"
            data-aos="zoom-in"
            data-aos-delay="200"
          >
            <div class="icon-box iconbox-orange">
              <div class="icon">
                <svg
                  width="100"
                  height="100"
                  viewBox="0 0 600 600"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke="none"
                    stroke-width="0"
                    fill="#f5f5f5"
                    d="M300,582.0697525312426C382.5290701553225,586.8405444964366,449.9789794690241,525.3245884688669,502.5850820975895,461.55621195738473C556.606425686781,396.0723002908107,615.8543463187945,314.28637112970534,586.6730223649479,234.56875336149918C558.9533121215079,158.8439757836574,454.9685369536778,164.00468322053177,381.49747125262974,130.76875717737553C312.15926192815925,99.40240125094834,248.97055460311594,18.661163978235184,179.8680185752513,50.54337015887873C110.5421016452524,82.52863877960104,119.82277516462835,180.83849132639028,109.12597500060166,256.43424936330496C100.08760227029461,320.3096726198365,92.17705696193138,384.0621239912766,124.79988738764834,439.7174275375508C164.83382741302287,508.01625554203684,220.96474134820875,577.5009287672846,300,582.0697525312426"
                  ></path>
                </svg>
                <a href="../assets/Tugas Analisis 1.pdf" target="_blank"
                  ><i class="bx bx-file"></i
                ></a>
              </div>
              <h4>
                <a href="../assets/Tugas Analisis 1.pdf" target="_blank"
                  >Tugas Analisis 1</a
                >
              </h4>
              <p>Mata Kuliah Basic Web Programming</p>
            </div>
          </div>

          <div
            class="col-lg-4 col-md-6 d-flex align-items-stretch mt-4 mt-md-0"
            data-aos="zoom-in"
            data-aos-delay="200"
          >
            <div class="icon-box iconbox-teal">
              <div class="icon">
                <svg
                  width="100"
                  height="100"
                  viewBox="0 0 600 600"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke="none"
                    stroke-width="0"
                    fill="#f5f5f5"
                    d="M300,582.0697525312426C382.5290701553225,586.8405444964366,449.9789794690241,525.3245884688669,502.5850820975895,461.55621195738473C556.606425686781,396.0723002908107,615.8543463187945,314.28637112970534,586.6730223649479,234.56875336149918C558.9533121215079,158.8439757836574,454.9685369536778,164.00468322053177,381.49747125262974,130.76875717737553C312.15926192815925,99.40240125094834,248.97055460311594,18.661163978235184,179.8680185752513,50.54337015887873C110.5421016452524,82.52863877960104,119.82277516462835,180.83849132639028,109.12597500060166,256.43424936330496C100.08760227029461,320.3096726198365,92.17705696193138,384.0621239912766,124.79988738764834,439.7174275375508C164.83382741302287,508.01625554203684,220.96474134820875,577.5009287672846,300,582.0697525312426"
                  ></path>
                </svg>
                <a href="../assets/Tugas Analisis 2.pdf" target="_blank"
                  ><i class="bx bx-file"></i
                ></a>
              </div>
              <h4>
                <a href="../assets/Tugas Analisis 2.pdf" target="_blank"
                  >Tugas Analisis 2</a
                >
              </h4>
              <p>Mata Kuliah Basic Web Programming</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- End Services Section -->
    <!-- ======= Contact Section ======= -->
    <section id="contact" class="contact">
      <div class="container" data-aos="fade-up">
        <div class="section-title">
          <h2>Contact</h2>
        </div>

        <div class="row mt-1">
          <div class="col-lg-4">
            <div class="info">
              <div class="address">
                <i class="bi bi-geo-alt"></i>
                <h4>Location:</h4>
                <p>Kp.Babakan Nanjung, Kab.Bandung, Jawa Barat</p>
              </div>

              <div class="email">
                <i class="bi bi-envelope"></i>
                <h4>Email:</h4>
                <p>raihanmuhammadsaprudin898@gmail.com</p>
              </div>

              <div class="phone">
                <i class="bi bi-phone"></i>
                <h4>Call:</h4>
                <p>+62 89516011186</p>
              </div>
            </div>
          </div>

          <div class="col-lg-8 mt-5 mt-lg-0">
            <form
              action="forms/contact.php"
              method="post"
              role="form"
              class="form"
              @submit="submitForm"
            >
              <div class="row">
                <div class="col-md-6 form-group">
                  <input
                    type="text"
                    name="name"
                    class="form-control"
                    id="name"
                    placeholder="Your Name"
                    v-model="name"
                    required
                  />
                </div>
                <div class="col-md-6 form-group mt-3 mt-md-0">
                  <input
                    type="email"
                    class="form-control"
                    name="email"
                    id="email"
                    v-model="email"
                    placeholder="Your Email"
                    required
                  />
                </div>
                <div class="col-md-6 form-group mt-3">
                  <input
                    type="phone"
                    class="form-control"
                    name="phone"
                    id="phone"
                    v-model="phone"
                    placeholder="Your phone"
                    required
                  />
                </div>
              </div>
              <div class="form-group mt-3">
                <textarea
                  class="form-control"
                  name="message"
                  rows="5"
                  placeholder="Message"
                  v-model="message"
                  required
                ></textarea>
              </div>
              <div class="text-center">
                <button type="submit">Send Message</button>
              </div>
            </form>
            <table class="table table-dark table-striped table-fixed">
              <colgroup>
                <col style="width: 50px" />
                <col style="width: 150px" />
                <col style="width: 125px" />
                <col style="width: 125px" />
                <col style="width: 300px" />
              </colgroup>
              <thead>
                <tr>
                  <th class="table-mainn">No</th>
                  <th class="table-mainn">Nama</th>
                  <th class="table-mainn">Email</th>
                  <th class="table-mainn">Telepon</th>
                  <th class="table-mainn">Pesan</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="(entry, index) in entries" :key="index">
                  <td class="td-cen">{{ index + 1 }}</td>
                  <td class="td-cen">{{ entry.name }}</td>
                  <td class="td-cen">{{ entry.email }}</td>
                  <td class="td-cen">{{ entry.phone }}</td>
                  <td class="td-just">{{ entry.message }}</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </section>
    <!-- End Contact Section -->
  </main>
  <!-- End #main -->

  <!-- ======= Footer ======= -->
  <footer id="footer">
    <div class="container">
      <h3>Raihan Muhammad Saprudin</h3>
      <p>If you don’t take risks, you can’t create a future!</p>
      <div class="social-links">
        <a
          href="https://web.facebook.com/profile.php?id=100016967735048"
          class="facebook"
          target="_blank"
          ><i class="bx bxl-facebook"></i
        ></a>
        <a
          href="https://www.instagram.com/raihanm0607"
          class="instagram"
          target="_blank"
          ><i class="bx bxl-instagram"></i
        ></a>
        <a href="https://github.com/fsociety781" class="github" target="_blank"
          ><i class="bx bxl-github"></i
        ></a>
        <a
          href="https://www.linkedin.com/in/raihanms07/"
          class="linkedin"
          target="_blank"
          ><i class="bx bxl-linkedin"></i
        ></a>
      </div>
      <div class="copyright">
        &copy; Copyright <strong><span>Raihan Muhammad Saprudin</span></strong
        >. All Rights Reserved
      </div>
    </div>
  </footer>
  <!-- End Footer -->

  <div id="preloader"></div>
  <a
    href="#"
    class="back-to-top d-flex align-items-center justify-content-center"
    ><i class="bi bi-arrow-up-short"></i
  ></a>
</template>
