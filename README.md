# UYGULAMALI ÖDEV

## Profil Kartları Galerisi

---

## 🎯 Ödevin Amacı

Bu proje ile öğrenciler:

- Doğru HTML yapısı kurmayı
- CSS boyutlandırma (`width` / `height` / `min` / `max`) mantığını
- `outline` ve `outline-offset` ile etkileşimli vurgu oluşturmayı
- CSS combinator (seçici bağlaçları) kullanmayı
- Harici CSS dosyası ile stil yönetimini öğrenir.

---

## 🧩 Proje Tanımı

Bir sosyal ağ veya ekip tanıtım sayfası için **3 adet** profil kartı oluşturulacaktır.

Her kartta:

- Profil fotoğrafı
- Kullanıcı adı
- Kısa açıklama
- Bir bağlantı (LinkedIn vb.)

bulunacaktır.

Kartlar `section` veya `div` içinde galeri düzeninde yer alacaktır.

> Responsive zorunlu değildir.

---

## ✅ Teknik Gereksinimler

### 🏗️ Sayfa Yapısı

- Sayfanın üstünde bir **header** bölümü olmalı (başlık + alt yazı)
- Header arka plan rengi ve yazı rengi belirgin olmalı
- Kartlar bir `section` içinde **Flex düzeni** ile sıralanmalı:
  - `display: flex`
  - `flex-wrap: wrap`
  - `justify-content: center`
  - `gap: 20px`

### 📏 Boyutlandırma

- Kart genişliği sabit olabilir 
- Fotoğraf yüksekliği sabit olmalı
- Görsel taşmamalı → `object-fit`
- Aşağıdakilerden **en az biri** kullanılmalı:
  - `min-height`
  - `max-height`
  - `min-width`

### 🎨 Outline Kullanımı

- Kart **hover** olunca `outline` görünmeli
- Kart **focus** olunca `outline` görünmeli (`tabindex` eklemeyi unutma!)
- `outline-offset` kullanılmalı

### 🎭 Görsel Efektler

- Kartlara `box-shadow` ile gölge verilmeli
- Kartlara `border-radius` ile köşe yuvarlatma uygulanmalı
- `transition` ile geçiş animasyonu eklenmelidir
- Hover durumunda `transform` kullanılmalı (örn: `translateY`, `scale`)
- Hover'da `box-shadow` değişerek derinlik hissi artmalı

### 🔗 Link Stillendirme

- Kartlardaki bağlantılar **buton görünümünde** olmalı
- `background`, `padding`, `border-radius` ile stillendirilmeli
- Hover durumunda renk değişmeli
- `transition` ile yumuşak geçiş sağlanmalı

---

### 🎯 CSS Combinator Kullanımı (Zorunlu)

Her biri **en az 1 kez** kullanılmalıdır:

| Combinator     | Örnek              | Amaç                       |
| -------------- | ------------------ | --------------------------- |
| descendant     | `.card p`          | Kart içindeki açıklama      |
| child (`>`)    | `.card > img`      | Sadece direkt resim         |
| adjacent (`+`) | `.card + .card`    | Yanındaki kart              |
| general (`~`)  | `.card ~ .card`    | Sonraki kartlar             |

---

## Resim 
<img src="../img/odev2.png" alt="Ödev Görseli" width="600">
