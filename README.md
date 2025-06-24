# Instagram Yorum Beğeni Otomasyonu 🤖❤️

Bu proje, Python ve Selenium kullanılarak geliştirilen bir Instagram otomasyon botudur. Belirtilen bir gönderinin altında yer alan tüm yorumları otomatik olarak **beğenir**. Ek olarak, kullanıcı giriş bilgileriyle Instagram'a giriş yapar, kullanıcı araması yapar ve ilgili gönderiye yönlenir.

## 🚀 Özellikler

- Instagram hesabına otomatik giriş yapar.
- Belirlenen bir kullanıcıyı arar ve profiline gider.
- Belirtilen bir gönderiye erişir.
- Gönderinin altındaki **tüm yorumları tespit eder ve beğenir**.
- Yorumları yüklemek için sayfayı otomatik olarak kaydırır.
- Otomatik tekrar ile tüm yorumlar beğenilene kadar devam eder.

## 🛠 Kullanılan Teknolojiler

- Python
- Selenium (Web Otomasyonu)
- Firefox WebDriver
- BeautifulSoup (şu an kullanılmasa da ileride içerik analizinde kullanılabilir)
- time & argparse modülleri

## 🔐 Giriş Bilgileri

Kullanıcı adı, şifre ve aranacak kullanıcı adı bilgileri `loginInfo.py` dosyasından alınmaktadır. Bu dosya şu şekilde yapılandırılmalıdır:

```python
# loginInfo.py
USERNAME = "kullanici_adiniz"
PASSWORD = "sifreniz"
ARANILAN = "aranacak_kullanici"
⚠️ Bu dosya güvenlik nedeniyle .gitignore dosyasına eklenmeli ve GitHub'a yüklenmemelidir!

💻 Kurulum ve Kullanım
Bu projeyi klonlayın:

git clone https://github.com/kullaniciadi/instagram-comment-liker.git
cd instagram-comment-liker
Gereksinimleri yükleyin:

pip install selenium
Firefox WebDriver sisteminizde kurulu olmalıdır. GeckoDriver sayfasından işletim sisteminize uygun sürümü indirip, çalıştırılabilir dosyayı sistem PATH’ine ekleyin.

loginInfo.py dosyasını oluşturun ve bilgilerinizi girin (detay yukarıda).

Python scriptini çalıştırın:

python script_adi.py
📸 Hedef Gönderi URL'si
Otomasyonun yorum beğenme işlemi yaptığı gönderi URL'si scriptin içinde şu şekilde ayarlanmıştır:

post_url = "https://www.instagram.com/p/C5ldpkdtaQS/?img_index=1"
Bu URL’yi kendi hedefinize göre güncelleyebilirsiniz.

⚠️ Uyarılar
Bu proje yalnızca öğrenme ve kişisel projeler amacıyla geliştirilmiştir.

Instagram'ın kullanım şartlarına aykırı otomasyon faaliyetleri hesabınızın askıya alınmasına neden olabilir.

Her zaman bu tür araçları kullanmadan önce Instagram API ve kullanım kurallarını göz önünde bulundurun.
