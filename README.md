# GitHub Slideshow (GitHub Learning Lab)

GitHub Learning Lab'ın "Introduction to GitHub" kursu için oluşturulan alıştırma deposu. Kursta issue, dal (branch), commit ve pull request akışı, bu depodaki Jekyll tabanlı slayt gösterisine yeni slayt eklenerek öğrenilir.

> **Not:** Bu depo GitHub'ın eğitim şablonundan (githubtraining) oluşturuldu; içerik büyük ölçüde GitHub eğitim ekibine aittir. Son değişiklik 2020 yılındadır ve artık güncellenmiyor. Bağımlılıkları eskidir ve bilinen güvenlik açıkları içerebilir.

## İçerik

| Yol | Ne yapar |
|---|---|
| `_posts/` | Slaytlar; her Markdown dosyası bir slayttır |
| `_layouts/`, `_includes/` | Sunum, tek slayt ve yazdırma sayfa şablonları |
| `_config.yml` | Jekyll ve reveal.js ayarları (tema, geçişler vb.) |
| `node_modules/reveal.js/` | Slaytları çalıştıran reveal.js 3.9.2. Şablonlar doğrudan bu klasöre bağlandığı için bilerek depoda tutuluyor |
| `script/` | Kurulum (`setup`), yerel sunucu (`server`) ve derleme kontrolü (`cibuild`) betikleri |

## Teknolojiler

- Jekyll (`github-pages` gem'i), Ruby, Bundler
- reveal.js 3.9.2
- `html-proofer` (bağlantı kontrolü)

## Çalıştırma

Ruby ve Bundler kurulu olmalıdır.

```
script/setup
script/server
```

Ardından tarayıcıda `http://localhost:4000` adresini açın. Sağ ok tuşuyla slaytlar arasında gezilir.

## Lisans ve teşekkür

Slayt altyapısı açık kaynak [reveal.js](https://github.com/hakimel/reveal.js/) projesine dayanır; projenin kendi geçmişi ve katkıda bulunanları için orijinal depoya bakın. Jekyll şablonunun lisansı `LICENSE` dosyasındadır (MIT).
