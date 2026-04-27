# Baraj — Privacy Policy

Baraj KPSS hazırlık uygulamasının gizlilik politikası. Static HTML, repo gerektirmeyen ücretsiz hosting sağlayıcısıyla yayına alınır.

---

## Klasör içeriği

```
privacy/
├── index.html      → Ana gizlilik politikası sayfası (TR)
├── 404.html        → Sayfa bulunamadı fallback'i
├── .nojekyll       → Jekyll devre dışı
├── .gitignore
└── README.md       → Bu rehber
```

---

## Yayınlama — 2 ücretsiz seçenek (repo gerekmez)

Her iki seçenek de:
- Tamamen ücretsiz, süresiz
- Public repo, GitHub hesabı, git push gerektirmez
- Dışarıya görünen tek şey gizlilik metninin kendisi (zaten public olması gereken)
- Kalıcı, marketlere uygun URL üretir

### Seçenek 1 — Cloudflare Pages (önerilen)

Profesyonel CDN, hızlı, kararlı.

1. https://dash.cloudflare.com/sign-up → ücretsiz hesap aç (sadece e-posta yeterli)
2. Sol menü: **Workers & Pages → Create application → Pages → Upload assets**
3. Proje adı: `baraj-privacy` (URL'nin parçası olur)
4. Bu klasörün (`privacy/`) tamamını yükle
5. **Deploy site**

**URL hazır:** `https://baraj-privacy.pages.dev`

Politikayı güncellemek istediğinde aynı projeye yeni bir deployment yüklersin, URL aynı kalır.

---

### Seçenek 2 — Netlify Drop (en hızlısı, hesap bile gerekmez)

1. Tarayıcıda aç: https://app.netlify.com/drop
2. Bu klasörün (`privacy/`) tamamını pencereye sürükle-bırak
3. ~30 saniye içinde URL hazır: `https://<rastgele-isim>.netlify.app`

(İstersen ücretsiz hesap açıp site adını `baraj-privacy.netlify.app` olarak değiştirebilirsin.)

---

## URL'yi nereye yapıştıracaksın?

### Google Play Console
**Policy → App content → Privacy policy** → URL'yi yapıştır.
Ayrıca **Data safety** formunda da aynı URL sorulabilir.

### Apple App Store Connect
**App Information → General Information → Privacy Policy URL** → URL'yi yapıştır.
iOS App Privacy bildirimini ayrıca App Store Connect'te doldurman gerekir.

---

## Politikayı güncellemek

1. `index.html` içindeki içeriği değiştir.
2. Sayfa üstündeki **"Son güncelleme"** tarihini bugünle değiştir.
3. Aynı yöntemle tekrar yükle (Cloudflare → yeni deployment / Netlify → yeni drop).
4. URL aynı kalır, marketler otomatik güncel sürümü gösterir.

---

## Notlar

- Politika hem dark hem light mode'a otomatik adapte olur (`prefers-color-scheme`).
- Custom domain (örn. `gizlilik.baraj.app`) ileride istersen Cloudflare Pages içinden ekleyebilirsin (domain ücreti ayrı).
- Bu klasörden hiçbir şey Baraj uygulamasının kaynak koduyla bağlantılı değildir — bağımsız bir static site.
