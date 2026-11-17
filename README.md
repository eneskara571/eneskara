# eneskara

## Cep Asistanı (telefon uygulaması)

`app/` klasöründe her telefonda (Android ve iPhone) çalışan, ana ekrana eklenebilen bir web uygulaması (PWA) var:

- **Görevler** – yapılacaklar listesi, ilerleme çubuğu, filtreler
- **Notlar** – otomatik kaydedilen, aranabilir notlar
- **Hesap Böl** – bahşiş ve kişi başı tutar hesabı (₺)
- **Sayaç** – odak/mutfak zamanlayıcısı; bitince titreşim + ses

Veriler sadece telefonun kendisinde (tarayıcı hafızasında) saklanır, hiçbir sunucuya gitmez. Bir kez açıldıktan sonra internetsiz de çalışır.

### Telefona kurulum (GitHub Pages ile, ücretsiz)

1. GitHub'da bu depoda **Settings → Pages** bölümüne gir.
2. *Source*: **Deploy from a branch**, *Branch*: uygulamanın bulunduğu dal, klasör: **/ (root)** → **Save**.
3. 1-2 dakika sonra adres: `https://eneskara571.github.io/eneskara/app/`
4. Telefonda bu adresi aç:
   - **iPhone (Safari):** Paylaş düğmesi → **Ana Ekrana Ekle**
   - **Android (Chrome):** sağ üstteki ⋮ menü → **Ana ekrana ekle / Uygulamayı yükle**
5. Ana ekrandaki **Cep** simgesine dokun; uygulama tam ekran açılır.

> Not: GitHub Pages ücretsiz planda yalnızca **herkese açık** depolarda çalışır.

### Bilgisayarda denemek

```bash
cd app
python3 -m http.server 8000
# tarayıcıda http://localhost:8000 adresini aç
```
