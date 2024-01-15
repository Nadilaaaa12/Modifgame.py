SS Code python 
![code3](https://github.com/Nadilaaaa12/Modifgame.py/assets/127285166/9c15e533-cfd4-45ae-8887-ae22a5d2afec)
SS run game
![image](https://github.com/Nadilaaaa12/Modifgame.py/assets/127285166/0f780ca1-11a1-42a1-809c-f800c48b28eb)

Ini saya mengubah icon lives,colours,Background warna,Mengubah font dan menebalkan font dan mengubah jumlah score.

import tkinter as tk : untuk mengimpor modul tkinter dan memberikannya alias tk agar lebih mudah digunakan.

GameObject class:
Ini adalah kelas dasar untuk objek dalam permainan. Ini mempunyai metode untuk dapatkan posisi objek, mindahin objek, dan menghapus objek dari kanvas.

Ball class (subclass of GameObject):
Kelas ini mewakili bola dalam permainan. Ini memiliki properti seperti radius, arah pergerakan, kecepatan. Metode update ini digunakan untuk memperbarui posisi bola, dan metode collide untuk menangani tumbukan bola dengan objek lain.

Paddle class (subclass of GameObject):
Kelas ini mewakili papan dalam permainan. Ini memiliki metode tambahan set_ball untuk menghubungkan bola dengan papan dan metode move yang disesuaikan untuk memastikan bahwa papan tidak keluar dari batas kanvas.

Brick class (subclass of GameObject):
Kelas ini mewakili bata dalam permainan. Bata memiliki properti jumlah pukulan (hits) dan dapat mengurangi jumlahnya setiap kali terkena bola. Metode hit mengurangi hitpoints dan menghapus bata jika hitpoints mencapai nol.

Game class (subclass of tk.Frame):
Kelas ini adalah inti dari permainan. Ini mengelola elemen-elemen seperti bola, papan, batu bata, dan HUD (Heads-Up Display). Metode setup_game, add_ball, add_brick, draw_text, update_lives_text, dan lainnya digunakan untuk mengatur dan memperbarui elemen-elemen permainan.

Main Program:
Bagian akhir adalah bagian utama program yang membuat instance dari kelas Game dan menjalankan mainloop untuk memulai permainan.
