# Kontrol Listesi — Doğrula · Onayla · Uygula · Test Et

Her değişiklik, boyutu ne olursa olsun, bu dört adımdan geçer. Adım
atlanmaz; küçük bir CSS düzeltmesi de büyük bir veri aktarımı da aynı
döngüyü izler.

---

## 01 — Doğrula

Değişikliğe başlamadan önce mevcut durumun tam olarak anlaşılması.

- [ ] İlgili dosya/sayfa `grep` veya `ls` ile gerçekten var mı, doğrulandı mı?
      (Var olduğu varsayılmadı, kontrol edildi.)
- [ ] Değiştirilecek şey başka hangi sayfaları/bileşenleri etkiliyor?
      (Bir sorunu çözerken başka bir şeye dokunulmadığından emin olundu.)
- [ ] Değişiklikten önce dosyanın yedeği alındı mı?
      (`.backup-YYYYMMDD-HHMM` formatında)
- [ ] Türkçe karakter içeren bir dosyaysa, doğru kodlama (UTF-8) planlandı mı?

## 02 — Onayla

Yapay zekânın önerdiği değişiklik, uygulanmadan önce kütüphaneci tarafından
gözden geçirilir.

- [ ] Önerilen değişiklik, üretim ortamına değil, önce bir mockup/önizleme
      olarak sunuldu mu?
- [ ] Değişiklik, istenen sonucu karşılıyor mu — yoksa gereğinden fazlasını
      mı yapıyor? (Kapsam taşması kontrol edildi.)
- [ ] Değişiklik, kurumun stil ve içerik standartlarına (renk, tipografi,
      dil) uygun mu?
- [ ] Metadata şeması (Dublin Core) ve mevcut alan adları korunuyor mu?
- [ ] Telif durumu belirsiz bir içerik varsa, insan tarafından ayrıca
      doğrulandı mı?

## 03 — Uygula

Onaylanan değişiklik, tek seferde ve izlenebilir şekilde uygulanır.

- [ ] Tek seferde yalnızca **tek bir değişiklik** yapıldı mı? (Birden fazla
      değişikliği aynı anda uygulamak, bir sorun çıktığında kaynağını
      bulmayı zorlaştırır.)
- [ ] Değişiklik öncesi yedek, geri dönüş için erişilebilir bir yerde mi?
- [ ] Değişiklik, versiyon kontrolüne (örn. günlük git commit) kaydedildi mi?
- [ ] Sunucu/dosya sistemi düzeyinde bir değişiklikse, kritik servisler
      (örn. dış yönlendirmenin bağlı olduğu port) yanlışlıkla kapatılmadı mı?

## 04 — Test Et

Değişiklik canlıya alındıktan hemen sonra doğrulanır; onay burada bitmez.

- [ ] İlgili sayfa gerçekten yüklendi mi, JS hatası var mı? (Tarayıcı
      konsolu kontrol edildi.)
- [ ] Değişiklik, hedeflenen sorunu çözdü mü — gerçek veriyle test edildi mi
      (mock/placeholder veri değil)?
- [ ] Standart test listesi çalıştırıldı mı: dil seçici, kullanıcı menüsü,
      arama, galeri/görsel yükleme, mobil görünüm?
- [ ] Bir şey beklenenden farklı davranıyorsa, döngü 01'e (Doğrula) geri
      dönüldü mü — üstüne yeni bir değişiklik eklenmedi mi?

---

## Genel ilkeler (her adımda geçerli)

- **Karar her zaman insanda kalır.** Yapay zekâ değişikliği üretir,
  kütüphaneci onaylar ve uygulama kararını verir.
- **Geri alınabilirlik ön koşuldur.** Yedeksiz değişiklik yapılmaz.
- **Kapsam disiplini.** Bir sorunu çözerken başka bir şeye dokunulmaz;
  "madem buradayım" mantığıyla ek değişiklik yapılmaz.
- **Şeffaflık.** Yapay zekânın hata yaptığı durumlar saklanmaz, öğrenme
  girdisi olarak değerlendirilir.
