# Prompt Örnekleri

Aşağıdaki kalıplar, süreç boyunca yapay zekâya verilen isteklerin
genelleştirilmiş hâlleridir. Kurum adı, sunucu bilgisi ve kişisel veri
içermez; doğrudan kopyalanıp kendi bağlamınıza uyarlanabilir.

Her kalıp, [kontrol listesindeki](kontrol-listesi.md) döngüye karşılık
gelir: önce **mevcut durumu okut**, sonra **öneri iste**, sonra
**tek bir değişikliği uygulat**, sonra **test ettir**.

---

## 1. Mevcut durumu anlama (Doğrula adımı)

```
[Dosya/klasör yolu]'ndaki [sayfa adı] sayfasını incele.
Şu an nasıl görünüyor, hangi bileşenlerden oluşuyor, açıkla.
Değişiklik yapmadan önce mevcut yapıyı anlamak istiyorum.
```

```
[X] özelliği neden çalışmıyor olabilir? Olası nedenleri sırala,
ama herhangi bir dosyayı değiştirmeden önce bana sor.
```

## 2. Değişiklik önerisi (Onayla adımı)

```
[Sayfa/bileşen]'de şu değişikliği yapmak istiyorum: [açıklama].
Önce bana bir önizleme/mockup göster, ben onaylamadan
gerçek dosyayı değiştirme.
```

```
Bu değişikliğin [X] sayfasını nasıl etkileyeceğini açıkla.
Başka hangi sayfalar/bileşenler bundan etkilenir?
```

## 3. Uygulama (Uygula adımı)

```
Onayladım, şimdi uygula. Ama önce [dosya adı]'nın yedeğini
[.backup-TARİH-SAAT] formatında al, sonra değişikliği yap.
Tek seferde yalnızca bu değişikliği yap, başka bir şeye dokunma.
```

```
Bu değişikliği Türkçe karakterler bozulmadan, UTF-8 kodlamasıyla
uygula.
```

## 4. Test (Test Et adımı)

```
Değişikliği uyguladıktan sonra ilgili sayfanın hâlâ doğru
çalıştığını doğrula: JS hatası var mı, sayfa yükleniyor mu,
[X] özelliği beklendiği gibi davranıyor mu?
```

```
Şu standart kontrol listesini çalıştır: dil seçici, kullanıcı
menüsü, arama kutusu, galeri görüntüleme, mobil görünüm.
Herhangi biri bozulduysa bildir.
```

## 5. Hata durumunda geri alma

```
Bu değişiklik beklenmedik bir sonuç verdi. Yedekten geri dön
ve neyin yanlış gittiğini açıkla. Yeni bir değişiklik önerme,
önce sorunu birlikte anlayalım.
```

## 6. Kapsam disiplini (her istekte hatırlatılan ilke)

```
Yalnızca belirttiğim değişikliği yap. Başka bir iyileştirme
fark edersen bana ayrıca söyle, ama onaylamadığım hiçbir şeyi
uygulama.
```

---

## Notlar

- Bu kalıplar, DSpace/XMLUI tabanlı bir kurumsal arşiv bağlamında
  geliştirilmiştir; farklı sistemlerde uyarlama gerekebilir.
- Yapay zekâya hiçbir istekte kişisel veri, kullanıcı hesap bilgisi
  veya sunucu erişim kimlik bilgisi verilmemiştir.
- "Tek seferde tek değişiklik" ilkesi, hata ayıklamayı kolaylaştırdığı
  için tutarlı biçimde uygulanmıştır.
