# Ders 4: Hareket

Dosyalar:
- `baslangic.html`  -> BURADAN BASLA. Sahne hazir, hareketi sen ekleyeceksin.
- `index.html`      -> Tam kod. Takilirsan buna bak (once kendin dene!).
- `three.min.js`    -> Three.js kutuphanesi. Dokunma. Hepsi AYNI klasorde kalmali.

Calistirmak: html dosyasina cift tikla, tarayicida acilir.
Degisiklikten sonra: Ctrl+S (kaydet), F5 (yenile).

## Yeni fikir: zaman ve sinus
- `t` = sayfa acildigindan beri gecen saniye (surekli buyur: 0, 1, 2, 3...)
- `Math.sin(t)` = -1 ile 1 arasinda yumusakca gidip gelen bir sayi

Hareket kalibi:

    taban + Math.sin(t * hiz) * mesafe

- `taban`: nesnenin durdugu yer
- `hiz`: buyudukce hareket hizlanir
- `mesafe`: buyudukce nesne daha uzaga gider

Zipla = `Math.abs(...)` ekle (eksi sayilari artiya cevirir, nesne yere batmaz).

## Konsol deneyi
F12 -> Console, sirayla yaz:
- `Math.sin(0)`
- `Math.sin(1.57)`
- `Math.sin(3.14)`
- `Math.sin(4.71)`
Sayilar nasil degisiyor?

## Gorevler (baslangic.html icinde)
1. Zaman olcer ekle (`saat` ve `t`)
2. Kup saga sola sallansin
3. Kure ziplasin
4. Silindir havada suzulsun
5. Bonus: Halka nefes alsin

## Bozma Oyunu
- `Math.sin(t * 3)` -> `Math.sin(t * 10)`
- `* 2` -> `* 5` (kurenin ziplama yuksekligi)
- `Math.abs(Math.sin(t * 3))` -> `Math.sin(t * 3)` (abs'i sil)
- `const t = saat.getElapsedTime();` -> `const t = 0;`

## Odev (birini sec)
- Kolay: 3 top, farkli hizlarda ziplasin
- Orta: Kardan adamin kafasi saga sola sallansin (`rotation.z`)
- Zor: Bir gezegen gunesin etrafinda donsun (ipucu: `Math.cos` ve `Math.sin` birlikte)

## Sayfa bos kalirsa
F12 -> Console -> kirmizi yaziyi oku.
