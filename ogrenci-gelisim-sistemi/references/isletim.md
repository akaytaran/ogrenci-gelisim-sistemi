# Günlük işletim (kurulumdan sonra)

Kurulum bitince bu skill, öğrencinin ve velinin günlük konuşmalarını yürütür. Her konuşmanın başında:
1. Program Bilgisi > Sistem Kimliği'nden belge ve sayfa kimliklerini al.
2. Konuşan öğrenci ise Durum Panosu > Sistem eğitimi tablosuna bak (`ogretici.md`).

## Günlük rapor ("günlük rapor", "bugün", "bitirdim", "yapamadım")

Amaç: 3 dakikada günü kaydetmek; sorgu değil sohbet.
1. Takvimden bugünün (öğrenci "dün" diyorsa dünün) takip edilecek etkinliklerini çek: `#calisma`, `#acik`, öncelikli rutin, okul platformu kontrolü, hobi, ev egzersizi, antrenman. Yemek ve yol etkinliklerini sorma.
2. Tek mesajda numaralı liste göster: "Şöyle cevaplayabilirsin: 1 tamam, 2 yarım, 3 yapmadım + sebep." Ayrıca: enerji/keyif 1–5 ve (okuma hedefi varsa) kaç sayfa okudun. Serbest yazarsa sen eşleştir.
3. Yapılmayan/yarım için sebebi gruba bağla (Yorgunluk · Süre yetmedi · Konuyu anlamadım · Okul ödevi çoktu · Unuttum · Plan dışı olay · Sağlık · Motivasyon). Sebep yoksa bir kez nazikçe sor; ısrar etme.
4. Günlük Kayıt'a her görev için satır ekle.
5. Telafi:
   - Ana derslerden yarım kalan → tampon bloğa ya da sonraki aynı ders bloğuna 15 dk not (yeni blok açma).
   - Hafif dersler/hobi → bir sonraki doğal bloğa ya da bu hafta bırak.
   - "Anlamadım" → mentor C modunu öner; Açık Haritası'na "Konu eksiği".
   - Yorgunluk ya da enerji ≤ 2 → telafi yok; yarını hafiflet önerisi.
6. Uyarı kontrolü (`ilkeler.md`).
7. Kapanış (4–6 satır): tamamlananları somut kutla, telafiyi tek satırda söyle, yarın için tek küçük hedef, iyi geceler.
8. Haftanın belirlenen gününde: "Bu hafta derslerde hangi konular işlendi?" (müfredat senkronu). "?" ya da uzun süredir "≈" olan ders varsa onu da sor.
9. Sistem eğitimi: rapordan sonra `ogretici.md`'ye göre ipucu/öneri/tekrar sorusu.

Unutulan rapor ertesi gün "dünkü günlük rapor" diye verilebilir (tarihi doğru yaz).

## Veli konuşmaları

- "Nasıl gidiyor?" → kısa durum özeti (Durum Panosu + son 7 gün), sonra ayrıntı isterse dönemsel rapor.
- "Programı değiştir / şu saat değişti" → güncelleme modu (SKILL.md), yalnız değişeni sor.
- "Okulda şu konular işlendi" → müfredat senkronu, ✓.
- Veli dersi yanıtları ("bugün şunu yaptık, şurada zorlandı") → Veli Dersi tablosuna işle; sonraki paketi ona göre ayarla.
- Koç/doktor/öğretmen geri bildirimi → ilgili sekmeye işle, gerekiyorsa rutini güncelle (ör. koç onayıyla kuvvet çalışması eklenir).

## Dosya üretimi ve Dosya Kutusu

Öğrenciye üretilen her dosya (özet not, soru seti, çözüm, çalışma kâğıdı):
1. PDF üret (Türkçe karakter destekli yazı tipi), çalışma dizinine kaydet.
2. Dosya Kutusu sayfasına yükle; "dosyalar" koleksiyonuna satır ekle: `ad, dosyaAdi, ders, aciklama, assetId, boyutKB, eklenme (ISO, saat dilimiyle), indirildi:false, indirilme:null, hatirlatma:0, bildirildi:true`.
3. Takvime uygun saatte 5 dk'lık bildirim (okul saatinde, korunan zamanda ve çalışma bloğu ortasında değil).
4. Sohbette "Dosya Kutusu'na koydum" de.
Dosya Kutusu yoksa: sohbette dosyayı gönder ve bulut klasörüne kaydet (varsa).

## Belge ekleme (karne, sertifika, sınav sonucu)

1. Belgeyi oku; kurum, tarih, puan/not/seviye, geçerlilik bilgisini çıkar. Okunamayanı tahmin etme.
2. Belge Arşivi sayfasına yükle (PDF, PNG, JPEG, WEBP; HEIC ise JPEG'e çevir). "belgeler" koleksiyonu: `ad, kategori (kimlik|akademik|dil|spor|muzik|referans|saglik|odul|diger), tarih, gereksinim (id ya da null), not, assetId, dosyaAdi, tur, boyutKB, eklenme, ekleyen`.
3. Kayıt bir gereksinimi tam karşılamıyorsa `gereksinim`'i boş bırak (sayfa onu "tamam" sayar); gerekirse yeni gereksinim aç.
4. Önemli veriyi (dil puanı, ortalama, sınav sonucu) Durum Panosu ve Yol Haritası'na tek satırla işle.
5. Veliye tek cümleyle onayla; bir sonraki eksik belgeyi söyle.
Belgeler e-postaya eklenmez; öğretmen raporlarına girmez.

## Raporlar ve e-posta biçimi

- HTML e-postada stil bloğu kullanma; satır içi stil ve `<table border=1 cellpadding=5 cellspacing=0>` gibi basit tablolar her istemcide düzgün görünür.
- Konu satırı önekli: "[<öğrenci>] ...".
- Büyük dosyaları e-postaya eklemeye çalışma; içerik gövdede, dosya Dosya Kutusu'nda.

## Aksama ve tekrar

Gece raporu aksama işareti koyarsa (`zamanlanmis-gorevler.md` > 1), öğrencinin bir sonraki sohbetinde `ogretici.md` > Kısa tekrar modu.
