# Fafi 27 — Dokunmatik + Telefon Gamepad

Fafi 27'in iki kişilik futbol sürümü.

## Kontrol seçenekleri

- **Akıllı Tahta · 2 Oyuncu:** Aynı dokunmatik ekranda sol yarı Takım 1, sağ yarı Takım 2 gamepad olur. İki oyuncu aynı anda ayrı parmaklarla oynayabilir.
- **Telefonla Oyna:** Node.js sunucusu çalışırken QR kod ile telefonları gamepad olarak bağlar.
- **Penaltı Atışları:** Mevcut penaltı serisi korunmuştur.

## Maç süreleri

- 3 dakika
- 5 dakika
- 8 dakika

Bu süre seçenekleri hem telefon gamepad modunda hem de akıllı tahta dokunmatik modunda kullanılabilir.

## GitHub Pages ile doğrudan oynama

Bu repo statik oynanabilir sürümü kökte içerir. GitHub'a yükledikten sonra:

1. Repository'yi aç.
2. **Settings → Pages** bölümüne gir.
3. **Deploy from a branch** seç.
4. Branch olarak `main`, klasör olarak `/ (root)` seç.
5. Kaydet.
6. Oluşan Pages adresini akıllı tahtada aç.

GitHub Pages sürümünde telefon/QR için Node.js sunucusu gerekmez; **Akıllı Tahta · 2 Oyuncu** doğrudan çalışır.

## Telefon gamepad + QR için

Node.js 18+:

```bash
npm install
npm start
```

Ardından bilgisayardaki/akıllı tahtadaki `http://localhost:3000` adresini aç. QR ile telefonları bağlamak için bu sunucu sürümü gerekir.

## Geliştirici testleri

```bash
npm test
```

23 mevcut oyun testi geçmelidir.
