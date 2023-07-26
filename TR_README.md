# Toplu E-posta Gönderme Programı
-----------------------
Bu program, Python ile Excel dosyasından alıcı bilgilerini okuyarak kişiselleştirilmiş e-postalar oluşturup, toplu e-posta gönderimini otomatikleştirmek için tasarlanmıştır.

# Özellikler
-----------------------
Excel dosyasından alıcı bilgilerini çekme ve e-posta şablonuna yerleştirme.
SMTP sunucusunu kullanarak e-postaları gönderme.
E-posta gönderimi sırasında bekleme süresi ekleyerek spam önlemlerine dikkat eder. (Dakikada 20 mail gönderiyor. Bu süre artırılıp azaltılabilir.)

# Kullanım
-----------------------
mailler.py dosyasındaki smtp_server, smtp_port, sender_email ve sender_password değişkenlerini kendi e-posta sağlayıcınıza ve kimlik doğrulama bilgilerinize göre düzenleyin.
email_template içindeki şablonu istediğiniz gibi özelleştirin ve yer tutucuları ({{name}}, {{surname}}, {{age}}, {{city}}, vb.) uygun alıcı bilgileriyle değiştirin.
Alıcı bilgilerini içeren bir Excel dosyası oluşturun. Excel dosyanızda sütun başlıkları name, surname, age, city gibi olmalıdır ve her alıcı bir satıra yerleştirilmelidir.
Python scriptini çalıştırarak e-posta gönderimini başlatın: python3 mailler.py

# Uyarılar
-----------------------
E-posta gönderim hızını, e-posta sağlayıcınızın politikalarına uygun bir şekilde düzenlemeyi unutmayın. Aşırı hızlı gönderim, e-postalarınızın spam olarak işaretlenmesine neden olabilir.
Toplu e-posta gönderimi yaparken, alıcıların iznini aldığınızdan ve izinli e-posta pazarlama yasalarına uyduğunuzdan emin olun.