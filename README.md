# 🤖 Öğretmen Atama Robotu

**Tur bazlı, gerekçeli ve şeffaf öğretmen atama sistemi.**
Öğretmen tercihlerini ve okul ihtiyaçlarını toplar, **2026-2027 dönemi MEB atama kurallarına göre** yapılandırılmış robotla adil ve tekrarlanabilir biçimde yerleştirir; her öğretmene ve her okula **neden bu sonucun çıktığını** tek tek gösterir.

> 📌 Bu depo yalnızca **tanıtım** amaçlıdır. Yazılımın **kaynak kodu paylaşılmamaktadır**; ticari bir üründür.
> Ekran görüntüleri **örnek (anonim) verilerle** hazırlanmıştır; gerçek kişi ve kurum bilgisi içermez.

---

## ✨ Öne çıkanlar

### 🔁 Tur bazlı atama modeli
- Atama tek seferde bitmez: **1. tur, 2. tur, 3. tur…** sınırsız sayıda tur yürütülür.
- Her tur **kendi içinde yalıtılmıştır** — 1. tur 2. turu, 1. ve 2. tur 3. turu etkilemez.
- Bir turda **atanan öğretmen** (göreve başlasın ya da başlamasın) sonraki turlara katılamaz.
- **Atanamayan öğretmen** sonraki turda yeniden tercih yapar; eski turun tercihleri geçersiz sayılır.
- Sonuçlar yayımlandığında turun ilan ve başvuruları **arşivlenir**; yalnızca gözlem ve analiz içindir.
- Öğretmen ve okul profil bilgileri sabit kalır; yalnızca atama işlemleri tura göre değişir.

### 🎯 Kademeli (öncelikli) atama robotu
- **Alan Eşleştirme tablosuna** göre (bölüm ↔ atamaya esas alan) üç öncelik derecesi: **1 · Asıl alan**, **2 · Eş değer**, **3 · Son çare**.
- Aynı kademede sıralama: **AGS puanı → diploma notu (4'lük)**; tüm eşitlik kuralları sabit ve tekrarlanabilir.
- Geçen yıl **MEB kurumunda görev yapmış** adaylara 2. ve 3. öncelikte öncelik.
- **İngilizce** ilanlarında bölüm eşleşmesi + **CEFR seviyesine (C2 → A1)** göre değerlendirme.
- **"Her yerde çalışabilirim"** tercihi için son kademe.
- Alan Eşleştirme tablosu yönetici tarafından ekrandan **yönetilir** (ekle / düzenle / sil).

### 🔎 Her sonuç için gerekçe
- Öğretmen, **her tercihinin** neden tuttuğunu ya da tutmadığını görür: kontenjan doldu, yerleşenlerin puanı, branş önceliği, üst tercihe yerleşti…
- Yönetici, öğretmen listesindeki 🟢 / 🔴 rozetine tıklayarak **tur tur tercih formunu ve gerekçeleri** açar.
- Öğretmen profilinde **hangi alanlara hangi öncelikle atanabileceği** açıkça yazar.

### 🔐 KVKK uyumlu görünürlük
- Okul, başvuran adayların ad ve telefonunu **maskeli** görür; yalnızca **kendisine atanan** adayın bilgileri açılır.
- Yönetici ve kritik işlemler denetim kaydına alınır.

### 📱 Her cihazda çalışır
- Yönetici, öğretmen ve okul panelleri masaüstü ve **mobil** ekranlara uyumludur.

---

## 🖼️ Ekran görüntüleri

### Yönetici paneli

**Atama Turları** — kayıt, başvuru ve ilan girişlerini tek yerden aç/kapat; turları yönet.
<img src="screenshots/yonetici-02-atama-turlari.png" alt="Atama Turları" width="100%">

**Alan Eşleştirme** — bölüm ↔ atamaya esas alan eşleşmeleri ve öncelik dereceleri.
<img src="screenshots/yonetici-03-alan-eslestirme.png" alt="Alan Eşleştirme" width="100%">

**Atama Robotu** — çalıştırma kayıtları, yayınlama ve geçersiz kılma.
<img src="screenshots/yonetici-04-atama-robotu.png" alt="Atama Robotu" width="100%">

**Atama raporu** — bölüm bazlı yerleşme oranı, taban ve tavan puanlar.
<img src="screenshots/yonetici-08-robot-raporu.png" alt="Atama raporu" width="100%">

**Öğretmen yönetimi** — 🟢 atandı / 🔴 atanamadı rozetleri tüm turları kapsar.
<img src="screenshots/yonetici-05-ogretmenler.png" alt="Öğretmen yönetimi" width="100%">

**Tur bazlı tercih geçmişi** — her tercih için sonuç ve gerekçe.
<img src="screenshots/yonetici-06-tercih-gecmisi.png" alt="Tur bazlı tercih geçmişi" width="100%">

**Raporlar** — tur seçerek okul, branş ve başvuru istatistikleri.
<img src="screenshots/yonetici-07-raporlar.png" alt="Raporlar" width="100%">

**Panel**
<img src="screenshots/yonetici-01-panel.png" alt="Yönetici paneli" width="100%">

### Öğretmen paneli

**Sonuçlarım** — tur tur sonuç, atanılan okulun iletişim bilgileri ve her tercihin gerekçesi.
<img src="screenshots/ogretmen-01-sonuclar.png" alt="Öğretmen sonuçları" width="100%">

**Atanabileceğiniz alanlar** — Alan Eşleştirme'ye göre öncelikler; Sınıf Öğretmenliği ve İngilizce için özel açıklamalar.

<img src="screenshots/ogretmen-02-atanabilecegi-alanlar.png" alt="Atanabileceğiniz alanlar" width="60%">

**Başvurularım** — gönderilmiş, kilitli tercih listesi; geçmiş turlar ayrı bölümde.
<img src="screenshots/ogretmen-03-basvurularim.png" alt="Başvurularım" width="100%">

**Mobil görünüm**

<img src="screenshots/mobil-01-sonuclar.png" alt="Mobil görünüm" width="320">

### Okul paneli

**Panel** — güncel turun ihtiyaç ve başvuru özeti; atanmayan adayların bilgileri maskeli.
<img src="screenshots/okul-01-panel.png" alt="Okul paneli" width="100%">

---

## ⚙️ Süreç nasıl işler?

1. **Kayıt ve giriş:** Okullar kayıt olup branş ihtiyaçlarını girer; öğretmenler kayıt olup tercihlerini sıralar. Yönetici tek ekrandan hangi girişin açık olacağına karar verir.
2. **Kapanış:** Yönetici başvuru ve ilan girişlerini kapatır.
3. **Robot:** Atama robotu tercihleri kademeli kurallarla değerlendirir ve sonuç raporunu üretir; yönetici raporu inceler.
4. **Yayın:** Sonuçlar yayımlanır; öğretmenlere ve okullara **gerekçeleriyle** iletilir.
5. **Arşiv:** Turun ilan ve başvuruları arşivlenir. Atananlar sonraki turlara katılmaz.
6. **Yeni tur:** Atanamayanlar ve boş kalan kontenjanlar için yeni tur açılır; süreç aynı kurallarla tekrarlanır.

---

## 📞 İletişim

Bilgi ve demo için ulaşabilirsiniz:

- 💬 **WhatsApp:** [0551 184 23 26](https://wa.me/905511842326)
- ✈️ **Telegram:** [@erdem21](https://t.me/erdem21)

---

<sub>© 2026 Erdem Software. Tüm hakları saklıdır. Bu depodaki metin ve görseller izinsiz kopyalanamaz, dağıtılamaz. Yazılımın kaynak kodu bu depoda yer almaz ve paylaşılmaz.</sub>
