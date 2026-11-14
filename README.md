# 🃏 Kıraathane VIP — Çok Oyunculu Kart Oyunları (GitHub Pages)

Sunucusuz (Backend gerektirmeyen), **Host-Otoriter (Anti-Cheat)** WebRTC mimarisiyle çalışan, 7 farklı kart oyununu barındıran statik web uygulaması.

## 🚀 GitHub Pages'e Yükleme (Adım Adım)
1. **GitHub.com** hesabınıza giriş yapın ve sağ üstten **New Repository** oluşturun (Örn: `kart-oyunlari`, **Public** seçin).
2. Bu ZIP paketinden çıkan tüm dosya ve klasörleri (`index.html`, `css/`, `js/`, `README.md`) reponuzun ana dizinine yükleyin.
3. Reponuzda **Settings > Pages** menüsüne girin.
4. **Build and deployment > Branch** kısmından **`main`** ve **`/ (root)`** seçip **Save** butonuna tıklayın.
5. 1-2 dakika sonra siteniz `https://kullaniciadi.github.io/kart-oyunlari/` adresinde yayında olacaktır!

## 🌐 Arkadaşlarla Uzaktan Nasıl Oynanır?
1. Bir oyuncu sitede **"👑 Arkadaşlarınla Oda Kur (Host)"** butonuna basar.
2. Ekranda oluşan 5 haneli oda kodunu veya **"🔗 Davet Linki Gönder"** butonuna basarak kopyaladığı linki WhatsApp/Discord üzerinden arkadaşlarına gönderir.
3. Arkadaşlarınız linke tıkladığında doğrudan odaya bağlanır.
4. Kurucu **"▶ Masayı Başlat"** butonuna bastığında herkes aynı masaya geçer.

## 🧪 Otomatik Doğrulama Motoru (`?test=1`)
Sitenizin sonuna `?test=1` ekleyerek açtığınızda (`https://.../index.html?test=1`), 7 oyunun tamamı için 200'er tam oyun (toplam 1.400 oyun) botlarla simüle edilir ve kart korunumu doğrulanır.

## ⚠️ Bilinen Sınırlamalar
- WebRTC (PeerJS) doğrudan tarayıcılar arası bağlantı kurar. Çok sıkı kurumsal güvenlik duvarları veya bazı simetrik NAT (CGNAT) mobil şebekelerde STUN/TURN bağlantısı engellenirse bağlantı zaman aşımına uğrayabilir.
- Oda kurucusu (Host) sekmesini tamamen kapatırsa oda sonlanır; diğer oyuncular koparsa 15 saniye beklenir ve dönmezlerse yerlerine otomatik Akıllı Bot geçer.
