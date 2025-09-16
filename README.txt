README - Dikotik Dinleme Izmir (Vercel deploy package)

Dosya açıklaması
- index.html  --> Tek sayfa, tüm deney arayüzü ve mantığı burada.
- sounds/      --> Bu paketin içinde ses dosyaları yok. Deploy etmeden önce repo içinde bir 'sounds' klasörü oluşturup WAV dosyalarını buraya koyun.
- Playlist-2.txt --> Deneyde kullanılacak dosya sıralaması index.html içinde 'playlist' dizisinde yer alır.

Hazırlık (adımlar)
1) GitHub repository oluştur (ör. idichotic-prototype).
2) Repo'ya index.html ve vercel.json dosyalarını ekleyin.
3) Repo içine 'sounds' adlı bir klasör oluşturun ve tüm .wav dosyalarını buraya yükleyin.
   Örnek: sounds/LBA-RKA.wav, sounds/LDA-RGA.wav, ... (dosya isimleri playlist ile birebir aynı olmalı).
4) Vercel ile GitHub hesabınızı bağlayıp repo'yu deploy edin.

E-posta gönderimi (opsiyonel)
Tarayıcıdan e-posta göndermek için EmailJS kullanabilirsiniz (kolay ve sunucusuz):
1) https://www.emailjs.com adresinden kayıt olun.
2) Bir 'Email Service' (örn. Gmail) ekleyin ve servis ID'sini alın.
3) Yeni bir 'Email Template' oluşturun; template içeriğinde message alanına CSV koyabilirsiniz.
4) EmailJS kullanıcı ID, service ID ve template ID'yi index.html içindeki ilgili yerlere girin:
   - EMAILJS_USER, EMAILJS_SERVICE, EMAILJS_TEMPLATE değişkenleri.
5) Kullanıcılar "E-posta Gönder" butonuna bastığında sonuçlar EmailJS aracılığıyla gönderilecektir.

Notlar
- Bu sürüm prototip amaçlıdır. Veri gizliliği / güvenlik için sunucu tarafı doğrulama eklenmelidir.
- Ses dosyalarını aynı repo altında barındırın (sounds klasörü) böylece site sorunsuz ses çalar.

