<img src="https://logovectorseek.com/wp-content/uploads/2019/08/lets-encrypt-logo-vector.png"/>

<h1>Tutorial Let's Encrypt di VPS</h1>

<p>Berikut adalah cara pasang SSL di VPS menggunakan <b>certbot</b></p>

<ol>
  <li>update VPSnya dulu, ketik <code>apt-get update</code></li>
  <li>install web server, disini saya pake apache2 ketik <code>apt-get install apache2</code></li>
  <li>install <b>certbot</b>, ketik <code>apt-get install python3-certbot-apache</code></li>
  <li>konfigurasi sertifikat SSL, buat sendiri file <code>nama_domain/ip_public_vps.conf</code> di folder <code>/etc/apache2/sites-available</code>, (<a href="">filenya ini</a>)
  </li>
</ol>
