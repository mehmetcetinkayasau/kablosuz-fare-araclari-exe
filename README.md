# Kablosuz Fare Araçları

Kurulum gerektirmeyen iki Windows programı. İndirip çalıştırmanız yeterli (Windows 10/11, 64 bit).

| Program | Ne işe yarar |
|---|---|
| **AliciBulucu.exe** | Karışmış kablosuz fare USB alıcılarını ayırt eder. Alıcıları bir USB hub'a takın, fareyi sallayın; ekran hangi alıcıdan sinyal geldiğini büyük yazıyla gösterir. |
| **LogitechEslestirici.exe** | Logitech Unifying / Nano / Lightspeed alıcılara Logitech fare eşler, eşli cihazları listeler, Unifying'de siler. |

## Alıcı Bulucu

1. Alıcıları (10–20'lik partiler halinde) harici güç kaynaklı bir USB hub'a takın.
2. `AliciBulucu.exe` dosyasını çalıştırın. Her alıcı bir sıra numarası alır.
3. Bir fare alın, açın, hareket ettirin. Üst bant sarıya döner: **ALICI #7 · Port 3 · Logitech Nano**.
4. Aynı numarayı fareye ve alıcıya yapıştırın, sıradaki fareye geçin.

PC'nin kendi touchpad'i gibi USB olmayan aygıtlar gri satırda otomatik yoksayılır. Satıra çift tık: yoksay / geri al. Başlığa çift tık: sütunu içeriğe sığdır.

## Logitech Eşleştirici

1. Logitech alıcıyı takın, `LogitechEslestirici.exe` dosyasını çalıştırın.
2. Soldan alıcıyı seçin, **Eşleştirme modunu aç (30 sn)** düğmesine basın.
3. Fareyi kapatıp açın. Bant yeşil **EŞLEŞTİ** gösterir.

| Alıcı | Eşlenebilir fareler |
|---|---|
| Unifying (turuncu yıldız logolu) | Unifying logolu ve "Unifying Ready" fareler (M175, M235, M185, M310, M325...) |
| Nano (logosuz, C534 / C52F...) | Yalnız birlikte satıldığı model ailesi |
| Nano C542 (M170/M171 ile gelen) | Yazılımla eşlenemez, sabit eşli → Alıcı Bulucu kullanın |
| Bolt | Bu araçla değil, Logi Options+ ile |

Protokol günlüğü: `%LOCALAPPDATA%\LogitechEslestirici\gunluk.log`

## Notlar

- Windows SmartScreen ilk çalıştırmada uyarabilir: "Ek bilgi" → "Yine de çalıştır".
- Yönetici yetkisi gerekmez. Uzak masaüstü oturumunda Alıcı Bulucu fare sinyallerini alamaz; PC başında çalıştırın.
