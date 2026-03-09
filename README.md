# MVA
Şoyle bir uygulama istiyorum HTML ,CSS, JavaScript ve başka ne gerekiyorsa kullanabilirsin uygulamaya input olarak bir şarkı vereceyiz sonra uygulama yapay zeka yardimi ile sesi batari, gitar , bass gitar,solo , söz olarak ayıracak hata ses seviyesini ayıracagiz  .

şimdi  siteye bir temel atalım beyaz tonları kullanalım. 


 ekranı üçe bölelim  sol üst input ve ayaraları 
Sağ üst output ve ayaraları.  Aşagısı batari gitar bass gitar solo söz ses seviyesini ayaralamak için kullanalım output a MP3 indirme olsun     aı promptu :Uygulama Adı: AI Audio Splitter & Mixer (Ses Ayrıştırıcı ve Karıştırıcı)
Görsel Tasarım: * Baskın renk beyaz ve açık gri tonları (Minimalist/Modern).
Ekran üçe bölünmüş yapıda:
Sol Üst: Giriş paneli (Dosya yükleme ve ayarlar).
Sağ Üst: Çıkış paneli (İşlem durumu ve MP3 indirme).
Alt Panel: Karıştırıcı (Mixer) katı. Bateri, Gitar, Bass Gitar, Solo ve Söz için ayrı kanallar.
Kullanılacak Teknolojiler ve Kütüphaneler:
Frontend (Arayüz):
HTML5 & CSS3: Temel yapı ve beyaz tonlu modern tasarım.
JavaScript (Vanilla): Uygulama mantığı ve slider kontrolleri.
Wavesurfer.js: Ayrıştırılan her ses kanalının dalga formunu (waveform) görselleştirmek için.
Axios: Frontend'den Backend'e ses dosyası transferi ve API iletişimi için.
Backend (Yapay Zeka ve İşleme):
Python (FastAPI): Hızlı ve asenkron bir API yapısı kurmak için.
Facebook Demucs (veya Spleeter): Sesi yapay zeka ile 4 veya 5 kanala (Vocal, Drums, Bass, Other) ayırmak için ana motor.
FFmpeg: Ses formatlarını dönüştürmek ve işlemek için sistem kütüphanesi.
Pydub: Kullanıcının alt paneldeki slider ayarlarını (ses seviyelerini) baz alarak kanalları birleştirip tek bir MP3 çıktısı oluşturmak için.
İşlevsel Gereksinimler:
Kullanıcı bir şarkı yüklediğinde, AI motoru arka planda çalışıp enstrümanları ayırmalı.
Alt paneldeki her kanalın kendine ait bir ses seviyesi (volume) slider'ı ve "Mute/Solo" butonu olmalı.
Kullanıcı ses seviyelerini ayarladıktan sonra "Dışa Aktar" dediğinde, bu ayarlarla yeni bir MP3 dosyası oluşturulup indirilebilmeli.