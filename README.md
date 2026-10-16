# GBMC Aktiviteler

PDU Circle ve CoE eğitimlerinin **Türkçe okulunda** LearnWorlds'e **Embed** olarak yerleştirilen etkileşimli aktiviteler (assessment, oyun). GitHub Pages ile yayınlanır:
`https://murat-gbmc.github.io/gbmc-aktiviteler/`

## Klasörler

| Klasör | Eğitim | Dosyalar |
|---|---|---|
| `risk-yonetimi/` | Risk Yönetimi: Tanımlamadan Aksiyona | `assessment-1.html` (Modül 2 sonrası) · `assessment-2.html` (Modül 4 sonrası) · `risk-butcesi.html` (oyun) |

## Adres parametreleri

- `name={{USER_NAME}}` — LearnWorlds kullanıcı adı; yalnızca ilk ad ekranda selamlamada gösterilir. Hiçbir yere kaydedilmez veya gönderilmez.

Örnek embed kodu:

```html
<iframe src="https://murat-gbmc.github.io/gbmc-aktiviteler/risk-yonetimi/risk-butcesi.html?name={{USER_NAME}}"
        width="100%" height="900" style="border:0" allow="fullscreen"></iframe>
```

## Kurallar

- Bu depodaki aktiviteler yalnızca Türkçedir. İngilizce okulun aktiviteleri ayrı kurgulanacak.

- Depo herkese açıktır. **Final sınavları ve not verilen içerikler buraya konmaz** (LearnWorlds'ün kendi sınav aracında kalır).
- Kişisel veri (e-posta, kullanıcı kimliği) adres parametresi olarak gönderilmez ve saklanmaz.
- Her dosya tek parça HTML'dir; dış kütüphane veya sunucu gerektirmez.
- Aktivite tamamlandığında üst sayfaya `postMessage({type: "gbmc-activity-complete", ...})` gönderilir.
