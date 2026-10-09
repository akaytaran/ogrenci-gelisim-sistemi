# Belgeler ve tablo şemaları

Sistemin ortak hafızası üç belgedir. Sekmeli bir belge aracı (Claude Docs) varsa Takip Defteri tek belge, çok sekmeli kurulur; yoksa ayrı belgeler/dosyalar. Tablolar düz ve tutarlı olsun ki otomatik görevler okuyup yazabilsin. Sütun adlarını değiştirme; otomatik görev talimatları bu adlara dayanır.

## 1 · Takip Defteri (aile + sistem)

### Sekme: Durum Panosu
- Başlık, tarih, kısa açıklama.
- **Ders durumu** tablosu: `Ders | Okulda şu anki konu | Son net/not | Durum | Odak`
  - "Okulda şu anki konu" işaretleri: `✓ <kim>, <tarih>` (doğrulanmış) · `≈ tahmini, <tarih>` (sistem tahmini) · `?` (bilgi yok). Ayrıntı: `mentorlar.md` > Müfredat senkronu.
- **Akademik geçmiş** satırı (yıllara göre ortalamalar, belgeler).
- **Sistem eğitimi** tablosu: `Alan | Değer` → İlk eğitim (yapılmadı / yapıldı, tarih) · Eğitimden sonraki kullanım (sayı) · Tekrar önerisi (yok / evet (sebep, tarih)) · Son aksama işareti.
- **Uyarılar** (madde listesi; tarihli).
- **Kurallar** (korunan zamanlar, yatış, bildirim saygısı; 4–6 madde).
- **E-posta alıcıları** tablosu: `Kişi | Adres | Aldığı raporlar`.

### Sekme: Günlük Kayıt
Tablo (en yeni üstte): `Tarih | Görev | Durum | Sebep | Enerji/keyif | Okunan sayfa | Not`
- Durum: Tamam / Yarım / Yapılmadı.
- Sebep grupları: Yorgunluk · Süre yetmedi · Konuyu anlamadım · Okul ödevi çoktu · Unuttum · Plan dışı olay · Sağlık · Motivasyon.

### Sekme: Açık Haritası
Tablo: `Ders | Konu | Açık türü | Kaynak (test/tarih) | Kapama planı | Durum`
- Açık türü: Konu eksiği · İşlem hatası · Dikkat · Süre · Soru kökünü okuma.
- Durum: Açık · Çalışılıyor · Kapandı (tarih).

### Sekme: Test ve Denemeler
Tablo: `Tarih | Tür (test/deneme/yazılı) | Ders | Doğru | Yanlış | Boş | Net/Not | Yanlış konular | Not`
Altında deneme trendi (deneme başına toplam net, ders netleri).

### Sekme: Spor ve Sağlık (spor ya da sağlık takibi varsa)
- Kulüp/antrenman bilgisi, koç görüşü (soru + cevap), mevcut ev rutini (tablo: Seans | Zaman | İçerik).
- Ölçümler (okul fiziksel uygunluk vb.) yalnız aile için; sakin ve olgusal dil.
- Beslenme planı özeti (istenmişse).
- Kayıt tablosu: `Tarih | Konu | Not`.

### Sekme: Program Bilgisi
- Okul saatleri, yol, ders programı (tablo), antrenman/kurs saatleri, korunan zamanlar.
- Günlük rutinler (öncelikli ders rutini, karma soru dağılımı tablosu).
- **Müfredat ilerleyişi:** her dersin ünite sırası, okulun resmi plana göre ofseti, ilerleme kuralları.
- Kaynaklar (kitaplar, soru bankaları, platformlar).
- **Sistem Kimliği:** belge id'leri/bağlantıları, sayfa adresleri, takvim hesabı ve seriler, otomatik görevler (ad, id, saat) ve **her birinin tam talimat metni**.
- **Değişiklik günlüğü:** `Tarih | Değişiklik | Kim istedi`.

### Sekme: Raporlar
Her gece/haftanın kısa raporu en üste: `## <tarih> · Günlük` (5–8 satır), `## <tarih> · Haftalık`.

### İsteğe bağlı sekmeler
- **Veli Dersi** (veli bir dersi kendisi çalıştırıyorsa): `Tarih | Konu | Paket | Kaynak ödevi | Sonuç / velinin notu`; satır `PLAN:` ile başlıyorsa planlanmış ders.
- **Özet Notlar Kitaplığı** (haftalık konu özetleri ayrı belgede de tutulabilir).

## 2 · Yol Haritası (aile)
Bkz. `hedefler.md` > Yol Haritası belgesi bölümleri.

## 3 · Öğrenci Rehberi (öğrenci)
Öğrenciye "sen" diliyle; kısa.
1. **Başlarken** (bkz. `ogretici.md`): ailenin mesajı + "senin işin üç şey" + bir akşamın akışı + aksarsa ne olur + kafan karışırsa ne yazarsın.
2. Günlük rapor nasıl verilir (örnek tek mesaj).
3. Test/deneme nasıl gönderilir (fotoğraf + "analiz et").
4. Anlamadığın bir şey olunca (fotoğraf + "anlamadım").
5. Spor ve esneme (varsa): ağrı varsa yapma kuralı.
6. Takvim renkleri tablosu.
7. Dosya Kutusu (bağlantı; "İndir"e bas).
8. Kurallarımız (4–5 madde, olumlu dille).

## Belge erişimi notu
Belgeler öğrencinin hesabındaysa öğrenci de görebilir. Aile içi hassas notları (sağlık, aile görüşmeleri) yazarken bunu hesaba kat ya da aile isterse bu notları velinin kendi belgesinde tut.
