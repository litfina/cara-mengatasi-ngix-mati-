<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?color=%2336BCF7&center=true&vCenter=true&lines=CARA+MENGATASI+NGIX+MATI" />
</p>
<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?color=%2336BCF7&center=true&vCenter=true&lines=L+I+T+F+I+N+A" />
</p>
<p align='center'>
  <a href="https://api.daily.dev/get?r=fisabiliyusri">
    <img src="https://github.com/litfina/scrip/raw/main/WhatsApp%20Image%202024-07-27%20at%2017.40.05.jpeg" width="300" alt="Hayuk"/>
  </a>
</p>

# `pertama cek apakah ngix mati di auto scrip`
## dengan perintah  ##
```
 sudo systemctl status nginx
```
# jika iya maka kerjakan seperti yang di bawah ini # 
 
# BAHAN BAHAN YANG DI BUTUHKAN #
`1 siapkan domain/subdomain`

`2 masukan perintah ini` 
```
sudo systemctl status nginx
```

#Job for nginx.service failed because the control process exited with error code.
See "systemctl status nginx.service" and "journalctl -xe" for details.
root@njay:~# sudo tail -f /var/log/nginx/error.log
2024/07/28 09:39:34 [emerg] 2592#2592: invalid number of arguments in "server_na                                                                                                             me" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:40:16 [emerg] 5359#5359: invalid number of arguments in "server_na                                                                                                             me" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:40:49 [emerg] 8397#8397: invalid number of arguments in "server_na                                                                                                             me" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:41:46 [emerg] 11439#11439: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:42:21 [emerg] 14174#14174: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:56:31 [emerg] 16712#16712: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:56:45 [emerg] 16844#16844: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 09:57:24 [emerg] 16882#16882: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:5
2024/07/28 10:03:51 [emerg] 18103#18103: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:120
2024/07/28 10:09:04 [emerg] 18762#18762: invalid number of arguments in "server_                                                                                                             name" directive in /etc/nginx/conf.d/xray.conf:120
#
contoh isi nya kek gitu 

nah di situ kita bisa membaca ada angka di terahir perintah di situ menerangkan permasalahan ngix kita kita harus memperbaikinya sendiri di configurasi ngix nya cara memperbaikinya adalah 

```
sudo nano /etc/nginx/conf.d/xray.conf
```
setelah kita masuk ke dalam file nya maka kita sekarang harus mencari yang namanya `` server_name `` cara pengisian nya adalah mengganti name server ke domain kalian 
kalian pasti bingun cari yang mana akan di ubah yang di ubah itu seperti yang di gambar gunakan domain kalian sendiri 
<p align='center'>
  <a href="https://api.daily.dev/get?r=fisabiliyusri">
    <img src=https://github.com/litfina/litfina/blob/main/1%20root.png width="1000" alt="1000"/>
  </a>
</p>

`` ini adalah yang pertama ``

`` yang kedua adalah ``

<p align='center'>
  <a href="https://api.daily.dev/get?r=fisabiliyusri">
    <img src=https://github.com/litfina/litfina/blob/main/2%20root.png width="1000" alt="1000"/>
  </a>
</p>

`` yang ketiga adalah ``

<p align='center'>
  <a href="https://api.daily.dev/get?r=fisabiliyusri">
    <img src=https://github.com/litfina/litfina/blob/main/3%20root.png width="1000" alt="1000"/>
  </a>
</p>

`` setelah itu jika sudah simpan ``


