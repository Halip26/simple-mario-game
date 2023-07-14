## Simple Mario Game with Pygame

### Penjelasan kode untuk baris 213 - 230

-```for event in pygame.event.get():```

- Baris ini memulai loop yang mengiterasi semua event dalam antrian event Pygame.
```if event.type == pygame.QUIT:```
- Baris ini memeriksa apakah event adalah event "QUIT", yang dipicu ketika pengguna mengklik tombol close pada jendela Pygame.
pygame.quit()
- Baris ini keluar dari modul Pygame.
sys.exit()
- Baris ini keluar dari interpreter Python.
if event.type == pygame.KEYDOWN:
- Baris ini memeriksa apakah event adalah event "KEYDOWN", yang dipicu ketika tombol pada keyboard ditekan.
if event.key == pygame.K_UP:
- Baris ini memeriksa apakah tombol yang ditekan adalah tombol panah "ATAS".
mario.up = True
- Baris ini mengatur atribut "up" dari objek "mario" menjadi True, menunjukkan bahwa tombol panah "ATAS" sedang ditekan.
mario.down = False
- Baris ini mengatur atribut "down" dari objek "mario" menjadi False, menunjukkan bahwa tombol panah "BAWAH" tidak sedang ditekan.
elif event.key == pygame.K_DOWN:
- Baris ini memeriksa apakah tombol yang ditekan adalah tombol panah "BAWAH".
mario.down = True
- Baris ini mengatur atribut "down" dari objek "mario" menjadi True, menunjukkan bahwa tombol panah "BAWAH" sedang ditekan.
mario.up = False
- Baris ini mengatur atribut "up" dari objek "mario" menjadi False, menunjukkan bahwa tombol panah "ATAS" tidak sedang ditekan.
if event.type == pygame.KEYUP:
- Baris ini memeriksa apakah event adalah event "KEYUP", yang dipicu ketika tombol pada keyboard dilepas.
if event.key == pygame.K_UP:
- Baris ini memeriksa apakah tombol yang dilepas adalah tombol panah "ATAS".
mario.up = False
- Baris ini mengatur atribut "up" dari objek "mario" menjadi False, menunjukkan bahwa tombol panah "ATAS" tidak lagi ditekan.
mario.down = True
- Baris ini mengatur atribut "down" dari objek "mario" menjadi True, menunjukkan bahwa tombol panah "BAWAH" sedang ditekan.
elif event.key == pygame.K_DOWN:
- Baris ini memeriksa apakah tombol yang dilepas adalah tombol panah "BAWAH".
mario.down = False
- Baris ini mengatur atribut "down" dari objek "mario" menjadi False, menunjukkan bahwa tombol panah "BAWAH" tidak lagi ditekan.
mario.up = True
- Baris ini mengatur atribut "up" dari objek "mario" menjadi True, menunjukkan bahwa tombol panah "ATAS" sedang ditekan.
