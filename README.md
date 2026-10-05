<p align="center">
  <img src="banner.png" alt="Muzogram v2" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Dart-0175C2?logo=dart&logoColor=white" alt="Dart">
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white" alt="Supabase">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Android%20%7C%20iOS%20%7C%20Web-FFD60A" alt="Platformlar">
</p>

**Muzogram**, fotoğraf paylaşıp arkadaşlarınla takipleşebildiğin ve gerçek zamanlı mesajlaşabildiğin bir sosyal medya uygulaması. Tek bir Flutter kod tabanından **Android**, **iOS** ve **web** için derleniyor.

> **Neden v2?** İlk Muzogram'ı 2022'de üniversitedeyken Kotlin ve Firebase ile yazmıştım ([Muzo](https://github.com/MustafaAkcicek/Muzo)). v2, aynı fikrin modern teknolojilerle sıfırdan, çok daha kapsamlı olarak yeniden yazılmış hâli.

<p align="center">
  <img src="screenshots.jpg" alt="Muzogram ekran görüntüleri" width="100%">
</p>

## ✨ Özellikler

| | |
|---|---|
| 📸 **Fotoğraf paylaşımı** | Galeriden veya kameradan, açıklamayla birlikte |
| ❤️ **Beğeni ve yorum** | Çift dokunuşla kalp animasyonu, yorum yazma ve silme |
| 👥 **Takip sistemi** | Takip et / takipten çık, takipçi ve takip edilen listeleri |
| 🧭 **Takip & Keşfet akışı** | Sadece takip ettiklerin ya da herkesin gönderileri |
| 💬 **Direkt mesajlar** | Gerçek zamanlı sohbet, okunmamış rozeti, okundu bilgisi (✓✓) |
| 🔍 **Kullanıcı arama** | Kullanıcı adı veya isme göre anında arama |
| 👤 **Profil** | Profil fotoğrafı, biyografi, gönderi ızgarası |
| 🌗 **Açık / koyu tema** | Telefonun temasına otomatik uyum |

## 🛠 Teknolojiler ve mimari

- **Flutter & Dart**: tek kod tabanıyla üç platform
- **Supabase Auth**: e-posta ile kayıt ve giriş
- **PostgreSQL**: `profiles`, `posts`, `likes`, `comments`, `follows`, `messages` tabloları, ilişkiler ve tetikleyiciler
- **Row Level Security**: herkes sadece kendi verisini değiştirebilir, mesajları sadece gönderen ve alan görebilir
- **Supabase Storage**: fotoğraf ve profil resimleri, kullanıcı başına klasör izolasyonu
- **Supabase Realtime**: sayfa yenilemeden canlı mesajlaşma ve bildirim rozeti
- **Web (PWA)**: iPhone'da "Ana Ekrana Ekle" ile uygulama gibi kullanım

```
lib/
├── models/      Post, Comment, Profile, Message, Conversation
├── services/    Veritabanı, depolama ve realtime işlemleri (tek API katmanı)
├── screens/     Giriş, kayıt, akış, arama, paylaş, mesajlar, sohbet, profil
└── widgets/     Gönderi kartı, avatar, logo, kullanıcı satırı
```

## 🔒 Erişim

Muzogram şu an davetle kullanılan kapalı bir uygulama ve kaynak kodu özel bir depoda tutuluyor. Uygulamayı denemek ya da kodu incelemek isteyen işverenler ve geliştiriciler [LinkedIn](https://www.linkedin.com/in/mustafaakcicek) üzerinden bana ulaşabilir.

## 👨‍💻 Geliştirici

**Mustafa Akçiçek** · [LinkedIn](https://www.linkedin.com/in/mustafaakcicek) · [GitHub](https://github.com/MustafaAkcicek)

<sub>© 2026 Mustafa Akçiçek. Tüm hakları saklıdır.</sub>
