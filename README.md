# Proje Masası

Arazi, imar ve ihtiyaç programından kütle yerleşimi: 2D plan, 3D ve kesit bir arada. Tablet için tasarlandı; kalemle çalışır. Chrome'da "Ana ekrana ekle" ile uygulama gibi kurulur, internetsiz de açılır.

İlk açılışta yarışma arsası (79,2 × 144,8 m), ihtiyaç programı ve kütleler hazır gelir.

Adres (Pages açıldıktan sonra): **https://mfbarsiv.github.io/proje-masasi/**

## GitHub'a yükleme

1. GitHub'da **New repository** ile `proje-masasi` adında, **Public** bir depo aç.
2. **Add file → Upload files** de. Zip'in içindeki her şeyi sürükle:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `README.md`
   - `icons` klasörü
   - `vendor` klasörü
   Klasör yapısı aynen kalmalı. **Commit changes**'e bas.
3. **Settings → Pages**: Source **Deploy from a branch**, Branch **main**, klasör **/ (root)**, **Save**.
4. 1–2 dakika içinde adres çalışır.

## Tablete kurma

1. Tablette **Chrome** ile adresi aç.
2. **⋮** menüsünden **Ana ekrana ekle** (ya da **Uygulamayı yükle**) de.
3. Ana ekrandaki **Proje Masası** simgesinden aç. Tam ekran açılır.

## Dosya menüsü (üstte, sağdaki belge simgesi)

- **DXF aç**: arazi çizimini içeri alır.
- **OBJ · 3D model**: kütleler hacim olarak çıkar (metre, Z yukarı). Her program ayrı katman/grup.
- **DXF · 3D hacim** ve **DXF · 2D plan**: CAD programları için.
- **Projeyi dosyaya kaydet / dosyadan aç**: tam yedek. Drive'a atabilirsin.

Çalışma tablette kendiliğinden saklanır. Tarayıcı verisini silersen ya da tablet değişirse yedek dosyadan geri yüklersin.

## Güncelleme

Yeni `index.html` gelince eski dosyanın üstüne yükle. Tablet hâlâ eskisini gösteriyorsa `sw.js` içindeki `proje-masasi-v1` adını `v2` yap ve onu da yükle.

## Notlar

- Kütleler çok kenarlı olabilir (U, L, T, X hazır şekiller ya da elle çizim). Avlulu (içi boş) çokgen yok.
- Aynı programa birden çok parça verilirse alanlar toplanır.
