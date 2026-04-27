# Privacy URL — Ücretsiz Hosting Rehberi

`index.html` dosyasını aşağıdaki **3 ücretsiz seçenekten** birine yükleyince Play Store / App Store için hazır URL elde edersin. Hepsi tamamen bedava ve süresiz.

---

## Seçenek 1: Netlify Drop — Hesap bile gerekmez (en hızlısı, ~30 saniye)

1. Tarayıcıda aç: **https://app.netlify.com/drop**
2. `Baraj/privacy` klasörünü tarayıcı penceresine sürükle bırak.
3. Anında bir URL verir, örn: `https://baraj-privacy-xyz123.netlify.app`
4. (Opsiyonel) Ücretsiz hesap açıp site adını `baraj-privacy.netlify.app` yapabilirsin.

**Sonuç URL'si:** `https://<isim>.netlify.app`

---

## Seçenek 2: GitHub Pages — Public repo'lar için %100 ücretsiz

> **Not:** GitHub Pages'in ücretli olduğu yanlış bilgi. Public repo'larda sınırsız ve ücretsizdir. Sadece custom domain (kendi alan adın) almak istersen domain ücreti çıkar.

1. https://github.com adresinden hesap aç (zaten varsa giriş yap).
2. **New repository** → İsim: `baraj-privacy` → **Public** seç → Create.
3. `index.html` dosyasını upload et (drag-drop yeterli).
4. Repo'da: **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save**.
5. 1-2 dakika sonra URL hazır: `https://<kullanıcıadın>.github.io/baraj-privacy/`

**Sonuç URL'si:** `https://ismailtaspinar.github.io/baraj-privacy/`

---

## Seçenek 3: Cloudflare Pages — Profesyonel + hızlı CDN

1. https://pages.cloudflare.com → ücretsiz hesap aç.
2. **Create a project → Direct Upload** seç.
3. `Baraj/privacy` klasörünü yükle.
4. Anında URL: `https://baraj-privacy.pages.dev`

**Sonuç URL'si:** `https://<proje>.pages.dev`

---

## Hangisini seçmeliyim?

| Kriter | Netlify Drop | GitHub Pages | Cloudflare Pages |
|---|---|---|---|
| Hesap gerekir mi? | Hayır | Evet | Evet |
| Kurulum süresi | 30 saniye | 5 dakika | 3 dakika |
| URL kalıcı mı? | Evet | Evet | Evet |
| Güncelleme kolaylığı | Tekrar drag-drop | Git push | Tekrar drag-drop |
| Önerilen kim için? | Hızlı çözüm isteyen | GitHub kullananlar | En profesyonel |

**Öneri:** Hemen URL lazımsa **Netlify Drop**. Uzun vadede repo'da tutmak istersen **GitHub Pages**.

---

## Google Play / App Store'a nereye yapıştırılır?

### Google Play Console
- **Policy → App content → Privacy policy** alanına URL'yi yapıştır.
- **Data safety** formunda yine bu URL'yi sorabilir.

### Apple App Store Connect
- **App Information → General Information → Privacy Policy URL** alanına yapıştır.
- iOS 14+ App Privacy bildirimi ayrıca App Store Connect'te doldurulmalı.

---

## Politikayı güncellemek istersen

1. `index.html` içindeki içeriği değiştir.
2. Üstteki **"Son güncelleme"** tarihini güncelle.
3. Aynı yöntemle tekrar yükle (Netlify drop / git push / Cloudflare upload).
4. URL aynı kaldığı için marketler otomatik en son sürümü gösterir.
