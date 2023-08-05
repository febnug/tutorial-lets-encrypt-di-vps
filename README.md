<img src="https://logovectorseek.com/wp-content/uploads/2019/08/lets-encrypt-logo-vector.png"/>

<h2>Tutorial Let's Encrypt di VPS</h2>

<p>Berikut adalah cara pasang SSL di VPS menggunakan <b>certbot</b></p>

<h2>Langkah 1, install certbot</h2>
<ol>
  <li>update VPSnya dulu, ketik <code>apt-get update</code></li>
  <li>install web server, disini saya pake apache2 ketik <code>apt-get install apache2</code></li>
  <li>install <b>certbot</b>, ketik <code>apt-get install python3-certbot-apache</code></li>
  <li>konfigurasi sertifikat SSL, buat sendiri file <code>nama_domain/ip_public_vps.conf</code> di folder <code>/etc/apache2/sites-available</code>, (<a href="https://raw.githubusercontent.com/febnug/tutorial-lets-encrypt-di-vps/main/febnug.cloud.conf">filenya ini</a>)
  </li>
</ol>

<h2>Langkah 2, mendapatkan sertifikat SSL</h2>

<ol>
  <li>ketik perintah <code>certbot --apache -d nama_domain -d www.nama_domain</code></li>
  <li>nanti kurang lebih tampilannya akan seperti pada <a href="https://www.rumahweb.com/journal/wp-content/uploads/2021/09/image-109.png">gambar 1</a> selanjutnya pada <a href="https://www.rumahweb.com/journal/wp-content/uploads/2021/09/image-110-1024x236.png">gambar 2</a></li>
  <li>coba akses domain kamu dan voila! akan muncul icon gembok di samping kiri nama domain kamu</li>
</ol>
