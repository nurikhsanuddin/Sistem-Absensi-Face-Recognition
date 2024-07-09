   <h1>Sistem Absensi Berbasis Face Recognition</h1>
   <p>Dalam dunia pendidikan, sistem absensi yang akurat dan efisien sangat penting untuk memastikan tercatatnya kehadiran siswa secara tepat waktu. Kehadiran yang teratur tidak hanya mendukung proses belajar mengajar, tetapi juga diperlukan untuk penilaian, pelaporan, dan analisis data. Namun, metode absensi tradisional seperti penggunaan sidik jari sering kali menghadapi berbagai kendala. Tidak semua individu memiliki sidik jari yang memadai untuk proses identifikasi, yang dapat disebabkan oleh sejumlah faktor. Beberapa di antaranya adalah cedera fisik yang mengubah pola sidik jari, aktivitas berlebihan yang mengikis sidik jari seperti mengetik atau bermain alat musik, serta kondisi medis atau penyakit tertentu yang mempengaruhi kondisi kulit dan pola sidik jari. Masalah lain yang dapat muncul termasuk reaksi alergi atau iritasi yang menyebabkan kerusakan pada sidik jari.</p>
    <p>Proyek ini adalah sistem absensi berbasis pengenalan wajah yang menggunakan OpenCV untuk deteksi wajah, Flask sebagai framework web, dan MySQL sebagai penyimpanan database. Sistem ini dirancang untuk mempermudah dan meningkatkan akurasi dalam proses absensi.</p>
    <h2>Fitur</h2>
    <ul>
        <li><strong>Pengenalan Wajah</strong>: Menggunakan OpenCV untuk mendeteksi dan mengenali wajah.</li>
        <li><strong>Web Interface</strong>: Dibangun menggunakan Flask untuk memungkinkan akses melalui browser.</li>
        <li><strong>Database</strong>: MySQL digunakan untuk menyimpan data absensi dan informasi pengguna.</li>
        <li><strong>Registrasi Wajah</strong>: Fitur untuk menambahkan wajah baru ke database.</li>
        <li><strong>Riwayat Absensi</strong>: Menampilkan riwayat absensi setiap pengguna.</li>
    </ul>
    <h2>Instalasi</h2>
    <ol>
        <li><strong>Clone repository ini</strong>
            <pre><code>git clone https://github.com/nurikhsanuddin/Sistem-Absensi-Face-Recognition</code></pre>
        </li>
        <li><strong>Navigasi ke direktori proyek</strong>
            <pre><code>cd Sistem-Absensi-Face-Recognition</code></pre>
        </li>
        <li><strong>Buat VENV</strong>
            <pre><code>py -3 -m venv .venv</code></pre>
        </li>
        <li><strong>Aktifkan VENV</strong>
            <pre><code>.venv\Scripts\activate</code></pre>
        </li>
        <li><strong>Install dependencies</strong>
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
        <li><strong>Konfigurasi Database</strong>
            <ul>
                <li>Buat database MySQL dengan nama "flask_db" dan sesuaikan pengaturan koneksi di file <code>app.py</code>.</li>
                <li>Import file <code>flask_db.sql</code> untuk membuat tabel yang diperlukan.</li>
                <li>pastikan seluruh lokasi folder/direktori pada <code>app.py</code> sudah benar, contoh : <code>D:/laragon/www/citra digital/dataset</code> disesuaikan dengan lokasi folder anda.</li>
                <li>Lakukan hal yang sama untuk setiap konfigurasi direktori yang ada pada <code>app.py</code></li>
            </ul>
        </li>
        <li><strong>Jalankan Aplikasi</strong>
            <pre><code>flask run</code></pre>
        </li>
    </ol>
    <h2>Konfigurasi</h2>
    <p>Konfigurasi aplikasi dapat diubah melalui file <code>app.py</code>, termasuk pengaturan database dan parameter lainnya.</p>
    <h2>Penggunaan</h2>
    <ol>
        <li><strong>Registrasi Wajah</strong>:
            <ul>
                <li>Akses endpoint <code>/tambah</code> melalui browser.</li>
                <li>Masukkan seluruh inputan dan lakukan perekaman wajah/training data maka data akan tersimpan di folder dataset.</li>
            </ul>
        </li>
        <li><strong>Absensi</strong>:
            <ul>
                <li>Akses endpoint <code>/</code> melalui browser.</li>
                <li>Sistem akan melakukan pengenalan wajah dan mencatat waktu absensi, nama, jabatan, serta lokasi</li>
            </ul>
        </li>
        <li><strong>Lihat Riwayat Absensi</strong>:
            <ul>
                <li>Akses endpoint <code>/admin</code> melalui browser.</li>
                <li>Gunakan username: admin, dan password: admin123 untuk login</li>
            </ul>
        </li>
    </ol>
    <h1>collaborator</h1>
    Ridwan Dwi Irawan : ridwan_dwiirawan@udb.ac.id
    
    
