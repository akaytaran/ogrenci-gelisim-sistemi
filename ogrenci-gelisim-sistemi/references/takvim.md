# Takvim kurulumu

Takvim, öğrencinin sistemle tek temas noktasıdır. Her etkinlik bir bildirimdir; başlık "şimdi ne", açıklama "nasıl".

## Genel kurallar

- Her çağrıda saat dilimini açıkça ver (ör. `Europe/Istanbul`). Saatleri yerel saat olarak yaz.
- Etkinlikler öğrencinin bildirim aldığı hesaba yazılır.
- Tekrarlayan seriler dönem sonuna kadar (ör. `RRULE:FREQ=WEEKLY;BYDAY=MO,TU,TH,FR;UNTIL=<dönem sonu>`). Okul tatillerini `EXDATE` ile hariç tut (okul bağlantılı serilerde). EXDATE saatleri serinin başlangıç saatiyle aynı olmalı; seri saati değişirse seriyi silip yeniden kur.
- Tekrar kuralı sonradan değiştirilemiyorsa (araç izin vermiyorsa) seriyi sil ve yeniden oluştur; geçmiş örnekleri bozma.
- Hatırlatma: varsayılan hatırlatmaları kapat, etkinliğe özel ayarla (çoğu iş için başlangıçta 0 dk; yola çıkış 5 dk; antrenman çantası 40–45 dk önce).
- Okul saatlerinde, korunan zamanlarda ve yatıştan sonra bildirim yok.
- Etiketleri açıklamanın son satırına yaz; otomatik görevler bunlarla arar:
  - `#plan` (sistemin her etkinliği) · `#calisma` (çalışma blokları) · `#veli` (veli görevi) · `#dosya` (dosya bildirimi) · `#veliders` (velinin verdiği ders) · `#acik` (açık kapama bloğu) · `#hedef` (başvuru/hedef kilometre taşı)
- Renkler (öneri; Rehber'deki tabloyla aynı olsun): Yemek sarı · Yol/okul gri · Rutinler turkuaz · Çalışma mavi · Spor kırmızı · Hobi/dil mor · Uyku/ekran yeşil · Veli görevleri grafit.

## Kurulacak seriler (gerekli olanlar)

| Seri | Örnek | Not |
|---|---|---|
| Okula çıkış | 07:45 "Okula yola çık" | Çanta/su kontrol listesi |
| Okuldan çıkış / eve varış | "Okuldan çıkış · yolda ara öğün" | Okul saatinde bildirim olmaz; çıkış saatinde tek bildirim |
| Kendi saati | "Eve hoş geldin · bu saat senin" | Görevsiz, "boş" (müsait) olarak işaretle |
| Okul platformu kontrolü | 5 dk | Ödev/duyuru/sınav tarihi |
| Öncelikli ders rutini | "Önce paragraf · 20 soru" | Gün gün içerik açıklamada |
| Çalışma blokları | Haftalık planlayıcı yazar | Açıklamada: önce ödev, konu, kaynak, sayfa/soru sayısı, karma sorular |
| Günlük rapor | "Günü kapat · 2 dk rapor" | Açıklamada: ne yazacağı, örnek cevap, rehber bağlantısı |
| Ekran kapanış | yatıştan 30–45 dk önce | Kitap önerisi |
| Haftaya hazırlık | Pazar akşamı 15–20 dk | Pazartesi çantası, haftanın blokları |
| Spor | antrenman/maç | Çanta listesi, öncesi/sonrası öğün |
| Ev esneme/mobilite | 15 dk | Hareket listesi; ağrı kuralı |
| Hobi | seanslar | Seviyeye uygun içerik, hedef |
| Öğünler (istenirse) | kahvaltı, akşam, antrenman öncesi | Menü önerisi, tabak modeli |
| Veli görevleri | haftalık rapora göz at; aylık kontrol | Veli davetli, öğrenciye bildirim kapalı |

## Veli görevleri

- Öğrencinin takviminde oluşturulur, veli e-postası davetli eklenir (davet e-postası gönderilsin). Öğrenci için hatırlatma kapalı, "müsait" olarak işaretli.
- Açıklama: "Veli görevi (<ad>)." + ne yapılacağı (5–10 dk) + sonucu Claude'a nasıl ileteceği.
- Öğrencinin de görebileceğini unutma: sağlık/kilo gibi hassas ayrıntı yazma; "ayrıntı: Takip Defteri > ..." de.
- Örnekler: haftalık rapora göz at · aylık hedef kontrolü · karne günü · öğretmen görüşmesi · koça sorulacaklar · doktor kontrolü planla · tercih dönemi.

## Açıklama şablonu (çalışma bloğu)

```
(Önce: <öncelikli rutin> bitti mi? Okul ödevi varsa önce ödev.)
1) <Ders>: <konu> · <kaynak, sayfa> · <soru sayısı> (<dk>)
2) <Ders>: <konu> · ... (<dk>)
3) Günün karma soruları (<toplam>): <Ders A> <n> + <Ders B> <n> (kaynak: özet notların mini testleri ya da <kitap>)
Yanlışların nedenini tek kelimeyle yaz (konu / dikkat / süre).

#plan #calisma
```

## Bildirim zamanlaması kontrolü

Kurulumdan sonra 7 günü listele ve tek tek kontrol et: okul saatinde bildirim var mı, korunan saate görev düşmüş mü, iki etkinlik aynı anda bildirim veriyor mu, yatıştan sonra bir şey var mı. Varsa düzelt.
