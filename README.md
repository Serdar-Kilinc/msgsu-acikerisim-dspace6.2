# MSGSÜ Açık Bilim ve Sanat Arşivi — Yapay Zekâ ile Yeniden İnşa Yöntemi

**ANKOSLink 2026 poster sunumuna eşlik eden yöntem belgesi.**

Bu depo, Mimar Sinan Güzel Sanatlar Üniversitesi Açık Bilim ve Sanat Arşivi'nin
(DSpace 6.2) dış teknik destek ve ek bütçe olmadan, yapay zekâ destekli ve
kütüphaneci denetimli bir işbirliğiyle dört ayda yeniden yapılandırılması
sürecinde izlenen yöntemi belgeler.

Amaç, benzer kaynak kısıtı yaşayan üniversite kütüphanelerinin bu süreci
kendi kurumlarında tekrarlayabilmesidir.

---

## İçindekiler

- [`kontrol-listesi.md`](kontrol-listesi.md) — Doğrula → Onayla → Uygula → Test Et
  döngüsünün her adımı için somut kontrol maddeleri
- [`prompt-ornekleri.md`](prompt-ornekleri.md) — Kullanılan istek (prompt) kalıplarından
  örnekler, genelleştirilmiş şablon hâlinde

## Bağlam

- **Kurum:** Mimar Sinan Güzel Sanatlar Üniversitesi, Kütüphane ve Dokümantasyon
  Daire Başkanlığı, Dijital Arşiv Birimi
- **Sistem:** DSpace 6.2, XMLUI
- **Süre:** 4 ay
- **Ekip:** 1 kütüphaneci
- **Yapay zekâ aracı:** Anthropic Claude (üretken yapay zekâ, yalnızca doğrulama
  ve onaydan geçen değişiklikleri uygulayan bir araç olarak kullanılmıştır)
- **Maliyet:** Yüklenici, danışmanlık veya ek bütçe yok. Tek gider: bireysel
  bir Claude Pro aboneliği.

## Temel İlke

> Yapay zekâ karar verici değil, araçtır. Her değişiklik kütüphaneci onayıyla,
> yedeklenerek ve geri alınabilir şekilde uygulanmıştır. Metadata bütünlüğü
> (Dublin Core) ve telif durumu insan tarafından doğrulanmıştır.

## Sınırlılıklar

Bu yöntem, alan bilgisi olan bir kütüphanecinin sürekli ve aktif denetimini
gerektirir; yapay zekâyı "bırakıp unutma" şeklinde çalıştırmak için
**tasarlanmamıştır**. Tek kurumda, tek yazılım sürümünde (DSpace 6.2)
denenmiştir. Yapay zekâya kişisel veri, kullanıcı hesap bilgisi veya sunucu
erişim bilgisi gönderilmemiş; yalnızca şablon, yapılandırma ve örnek veri
paylaşılmıştır.

## Atıf

Bu depoyu kullanırsanız veya yönteme atıfta bulunursanız, lütfen ANKOSLink 2026
poster sunumuna referans veriniz:

> Kılınç, S. (2026). *Yapay Zekâ Destekli Kurumsal Arşiv Dönüşümü: Dış Kaynak
> Kullanmadan Bir Yeniden İnşa Deneyimi — MSGSÜ Açık Bilim ve Sanat Arşivi
> Örneği.* ANKOSLink 2026 Uluslararası Konferansı, Antalya.

## İletişim

**Serdar Kılınç** — Şube Müdürü, MSGSÜ Akademi Kütüphanesi
Kütüphane ve Dokümantasyon Daire Başkanlığı, Dijital Arşiv Birimi
serdar.kilinc@msgsu.edu.tr

## Lisans

Bu belgeler [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.tr)
lisansı altında paylaşılmıştır — kaynak gösterilerek serbestçe kullanılabilir,
uyarlanabilir ve dağıtılabilir.
