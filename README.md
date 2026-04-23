# LinkedIn Feed İçerik Filtresi

LinkedIn ana akışını daha okunabilir hale getirmek için hazırlanmış bir **Tampermonkey userscript**.

Bu script; anket, kutlama, iş yıl dönümü ve benzer kalıp paylaşımlarını otomatik olarak tespit edip gizler.

## Özellikler

- Varsayılan içerik filtreleri:
  - `anket`
  - `poll`
  - `kutlama`
  - `kutluyorum`
  - `work anniversary`
  - `heyecanla duyuruyorum`
  - `excited to share`
  - `thrilled to announce`
- Özel regex deseni ekleme desteği
- Gizlenen gönderi sayacı
- Son gizlemeyi geri alma butonu
- Tek tek gönderi bazında geri alma / geçici gösterme
- Filtreyi durdur / yeniden başlat butonu

## Kurulum

### 1) Tampermonkey kur
Tarayıcına Tampermonkey eklentisini yükle.

### 2) Script'i ekle
- Tampermonkey panelini aç
- **Create a new script** seç
- İçeriği sil
- `linkedin-feed-content-filter.user.js` dosyasındaki kodu yapıştır
- Kaydet

### 3) LinkedIn feed'i aç
Script şu sayfalarda çalışır:

- `https://www.linkedin.com/*`

En iyi sonuç için LinkedIn ana akışında kullan.

## Kullanım

Script aktif olduğunda sağ altta **Feed İçerik Filtresi** paneli görünür.

Buradan şunları yapabilirsin:

- **Regex Ayarla**: Kendi özel filtre desenlerini ekler
- **Son Gizlemeyi Geri Al**: En son gizlenen postu geri getirir
- **Filtreyi Durdur / Başlat**: Script'i geçici olarak kapatır veya yeniden açar

Gizlenen her gönderinin yerinde küçük bir kutu görünür. Bu kutudan:

- **Geri al**: O postu kalıcı olarak geri getirir
- **Geçici göster**: 8 saniyeliğine gösterir

## Notlar

- LinkedIn arayüzü zaman zaman değiştiği için seçiciler ileride güncellenmek zorunda kalabilir.
- Script metin tabanlı filtreleme kullandığı için bazen yanlış pozitif üretebilir.
- Bu yüzden hem sayaç hem de geri al mekanizması eklendi.

## Geliştirme fikirleri

- Kelime listesi için ayar ekranı
- Farklı filtre profilleri
- Belirli hesapları asla gizleme (allowlist)
- Dışa / içe aktarılabilir filtre ayarları
- İstatistik paneli

## ⚠️ Yasal Uyarı

Bu script LinkedIn ile herhangi bir bağlantısı olmayan bağımsız bir topluluk aracıdır. LinkedIn'in [Kullanım Koşulları](https://www.linkedin.com/legal/user-agreement)'na uygun şekilde kullan.

---

## 📄 Lisans

[MIT License](LICENSE)


## Lisans

MIT
