# Slash App Mobile

Slash, işletmelerin kampanyalarını influencerlar aracılığıyla geniş kitlelere duyurmasını sağlayan, kullanıcıları, influencerları ve işletmeleri tek çatı altında buluşturan yenilikçi bir mobil uygulamadır.

## 🚀 Özellikler

- Kampanyaları keşfetme ve filtreleme
- Influencer'ları takip etme
- Kampanya detaylarını görüntüleme
- Bildirimler alma
- Profil yönetimi
- Çoklu dil desteği (Türkçe)
- Kullanıcı kimlik doğrulama (e-posta/şifre, Google, Facebook)
- Kampanya kaydetme ve paylaşma
- Influencer takip etme

## 🛠️ Teknolojiler

- React Native
- Expo
- Expo Router
- React Navigation
- React Native Elements
- i18next (Çoklu dil desteği)
- AsyncStorage
- Firebase (Auth, Firestore)

## 📱 Ekranlar

- Splash/Onboarding
- Giriş/Kayıt
- Ana Sayfa (Keşfet)
- Arama
- Bildirimler
- Profil
- Kampanya Detay
- Influencer Profil

## 🔥 Firebase Entegrasyonu

Uygulama, aşağıdaki Firebase servislerini kullanmaktadır:

### 🔐 Kimlik Doğrulama (Authentication)
- E-posta/şifre ile kayıt ve giriş
- Google ile giriş
- Facebook ile giriş
- Şifre sıfırlama
- Türkçe hata mesajları

### 💾 Veritabanı (Firestore)
Uygulama aşağıdaki koleksiyonları kullanmaktadır:

1. **kullanicilar**: Kullanıcı profilleri ve tercihleri
2. **kampanyalar**: Kampanya detayları ve istatistikleri
3. **influencerlar**: Influencer profilleri ve istatistikleri
4. **kategoriler**: Kampanya ve influencer kategorileri
5. **bildirimler**: Kullanıcı bildirimleri

### 📁 Servis Yapısı
Firebase servisleri `src/services/firebase` dizininde bulunmaktadır:

- `config.js`: Firebase yapılandırması
- `auth.js`: Kimlik doğrulama işlemleri
- `users.js`: Kullanıcı veritabanı işlemleri
- `campaigns.js`: Kampanya veritabanı işlemleri
- `influencers.js`: Influencer veritabanı işlemleri
- `notifications.js`: Bildirim veritabanı işlemleri
- `categories.js`: Kategori veritabanı işlemleri
- `index.js`: Tüm servisleri dışa aktaran ana dosya

## 🚀 Başlangıç

```bash
# Bağımlılıkları yükleyin
npm install

# Firebase yapılandırmasını ayarlayın
# src/services/firebase/config.js dosyasındaki firebaseConfig nesnesini güncelleyin

# Uygulamayı başlatın
npm start

# iOS simülatöründe çalıştırın
npm run ios

# Android emülatöründe çalıştırın
npm run android
```

## 📝 Firebase Kurulumu

1. [Firebase Console](https://console.firebase.google.com)'a gidin ve yeni bir proje oluşturun
2. Web uygulaması ekleyin ve yapılandırma bilgilerini alın
3. Authentication servisini etkinleştirin ve giriş yöntemlerini yapılandırın
4. Firestore veritabanını oluşturun ve güvenlik kurallarını yapılandırın
5. `src/services/firebase/config.js` dosyasındaki `firebaseConfig` nesnesini kendi yapılandırma bilgilerinizle güncelleyin

## 🔒 Güvenlik Notları

- API anahtarlarını ve gizli bilgileri doğrudan kodda saklamaktan kaçının
- Firestore güvenlik kurallarını dikkatli bir şekilde yapılandırın
- Kullanıcı kimlik doğrulama ve yetkilendirme kontrollerini uygulayın
