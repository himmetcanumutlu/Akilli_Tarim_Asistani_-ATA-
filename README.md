ATA: Akıllı Tarım Asistanı

Yapay Zeka Destekli Mahsul Hastalığı Teşhis ve Dijital Zirai Danışmanlık Sistemi

Tarımsal üretimde verimliliği artırmak, hastalıkları erken evrede tespit etmek ve ürün kayıplarını minimize etmek amacıyla geliştirilmiş uçtan uca bir derin öğrenme ve üretken yapay zeka (Generative AI) projesidir.

Proje Hakkında

Akıllı Tarım Asistanı (ATA), tarım profesyonellerinin ve çiftçilerin tarlalarındaki ürün hastalıklarını saniyeler içinde, yüksek doğrulukla tespit etmelerini sağlayan modern bir yapay zeka ekosistemidir. Sistem, yalnızca hastalık tespiti yapmakla kalmaz; tespit edilen anomaliye, mahsulün türüne ve gelişim evresine göre Google Gemini AI entegrasyonu sayesinde kullanıcıya özel, bilimsel temellere dayanan bir "Acil Zirai Eylem Planı" sunar.


Öne Çıkan Teknolojik Özellikler

- EfficientNet-B4 ile Gelişmiş Teşhis: 12 farklı mahsul türünde, yaprak yapısındaki mikroskobik deformasyonları dahi algılayabilen, hesaplama maliyeti optimize edilmiş yüksek doğruluklu derin öğrenme mimarisi.

- Açıklanabilir Yapay Zeka (XAI - Grad-CAM): Kara kutu (black-box) model yapısını şeffaflaştırmak adına, yapraktaki enfeksiyonlu bölgeler ısı haritası (Heatmap) ile görselleştirilir. Modelin karar mekanizması son kullanıcıya kanıt niteliğinde sunulur.

- Test Zamanı Veri Artırımı (TTA): Tahmin (Inference) aşamasında görüntüye uygulanan simetrik varyasyonlar sayesinde, anlık saha koşullarından (ışık parlamaları, gölgeler, çekim açıları) kaynaklanabilecek kararsızlıklar minimize edilir.

- Üretken Ziraat Mühendisi (Gemini 1.5 Flash): Teşhis edilen hastalık sonuçlarını işleyen LLM (Büyük Dil Modeli) tabanlı asistan, kullanıcıya doğal dil işleme yetenekleriyle kültürel ve kimyasal mücadele yöntemlerini detaylandırır.

- Otonom Eğitim ve Loglama: Yeni veri setleri eklendiğinde otonom olarak öğrenme sürecini başlatan, aşırı öğrenmeyi (Overfitting) engelleyen EarlyStopping mekanizmasına sahip ve eğitim metriklerini estetik grafiklerle raporlayan dinamik eğitim döngüsü.

- Model Performansı ve Kapsam / Model Performance and Scope


Model, gelişmiş Albumentations veri artırma teknikleri ve Karışık Hassasiyetli Eğitim (Mixed Precision) kullanılarak eğitilmiştir. Bu sayede ışık parlamaları, görüntü bozulmaları ve zorlu saha koşulları altında bile yüksek başarı göstermesi hedeflenmiştir.


Aşağıdaki doğruluk oranları modelin farklı mahsuller üzerindeki performansını göstermektedir:

| Mahsul | Doğruluk Oranı |
| :--- | ---: |
| Domates | %99.49 |
| Mısır | %97.12 |
| Soya Fasulyesi | %96.65 |
| Üzüm | %96.45 |
| Kayısı | %96.07 |
| Pirinç | %94.76 |
| Çilek | %92.33 |
| Elma | %92.96 |
| Buğday | %92.81 |
| Arpa | %92.59 |
| Patates | %90.55 |
| Şeftali | %85.58 |



## Proje Mimarisi ve Klasör Yapısı

Sistemin sürdürülebilirliği ve modülerliği için aşağıdaki dizin yapısı benimsenmiştir:

```bash
ATA-Projesi/
├── data/
│   └── raw/                   # Eğitim fotoğraflarının (12 mahsul sınıfı) bulunduğu ana dizin
├── grafikler/                 # Eğitim sürecinde otonom olarak üretilen Loss ve Accuracy metrik grafikleri
├── gradcam_ornekleri/         # Modelin odaklandığı patolojik alanları gösteren Grad-CAM çıktıları
├── egitim_otomatik.py         # Mahsulleri sırayla eğiten, ağırlıkları kaydeden ve loglayan ana script
├── test_gui.py                # LLM (Gemini) entegrasyonlu, Tkinter tabanlı grafiksel kullanıcı arayüzü
├── requirements.txt           # Proje bağımlılık ve kütüphane listesi
└── README.md                  # Proje dokümantasyonu


Kurulum ve Sistem Gereksinimleri

Gereksinimler

- Python 3.8 veya üzeri

- CUDA destekli GPU (Eğitim sürelerini optimize etmek için şiddetle tavsiye edilir)




Kurulum Adımları

1. Depoyu bilgisayarınıza klonlayın:

   git clone [https://github.com/](https://github.com/)<UfukAlparslan19>/ATA-Projesi.git
   cd ATA-Projesi


(Not: <UfukAlparslan19> kısmını kendi GitHub kullanıcı adınızla değiştirmeyi unutmayın.)

2. Gerekli bağımlılıkları yükleyin:

   pip install -r requirements.txt


(Eğer ortamınızda requirements.txt kullanmıyorsanız, aşağıdaki komutla manuel kurulum yapabilirsiniz:)

  pip install torch torchvision opencv-python numpy albumentations matplotlib grad-cam google-generativeai tqdm


3. LLM API Entegrasyonu (Önemli):
Projenin üretken zirai danışmanlık özelliğinin çalışabilmesi için, test_gui.py dosyasının konfigürasyon bölümünde yer alan GEMINI_API_KEY değişkenine kendi Google AI Studio API anahtarınızı tanımlamanız gerekmektedir.



Kullanım Kılavuzu

1. Model Eğitimi (Geliştirici Modu)

Kendi veri setlerinizle modeli sıfırdan eğitmek, ağırlık dosyalarını (.pth) güncellemek ve modelin başarım grafiklerini derlemek için aşağıdaki komutu çalıştırın:

  python egitim_otomatik.py


2. Grafiksel Kullanıcı Arayüzü (Son Kullanıcı Modu)

Tarımsal araziden çekilmiş bir yaprak görüntüsünü sisteme yüklemek, Grad-CAM ile enfeksiyon analizini görmek ve Gemini yapay zeka asistanından anlık tavsiye almak için arayüzü başlatın:

   python test_gui.py




Katkıda Bulunma 

ATA, bilginin paylaştıkça çoğaldığına inanan açık kaynaklı bir topluluk projesidir. Algoritma optimizasyonları, yeni mahsul veri setleri veya arayüz iyileştirmeleri gibi konulardaki katkılarınızı bekliyoruz:

1.Bu depoyu fork edin.

2.Üzerinde çalışacağınız yeni bir özellik dalı oluşturun: git checkout -b feature/YeniOzellik

3.Geliştirmelerinizi taahhüt edin: git commit -m 'Özellik: X eklendi ve Y optimize edildi'

4.Dalınızı uzak sunucuya gönderin: git push origin feature/YeniOzellik

5. Bir Pull Request (Çekme İsteği) oluşturarak inceleme sürecini başlatın.


Lisans

Bu proje MIT Lisansı koşulları altında açık kaynak olarak sunulmuştur. Detaylı bilgi ve yasal çerçeve için dizindeki LICENSE dosyasını inceleyebilirsiniz.

Yasal Uyarı ve Sorumluluk Reddi: ATA - Akıllı Tarım Asistanı, zirai süreçlerde erken teşhise yardımcı olmak ve veri odaklı karar almayı desteklemek amacıyla tasarlanmış bir yapay zeka aracıdır. Kritik zirai müdahalelerde, ilaçlama dozajlamalarında ve kesin hasar tespitlerinde nihai kararın lisanslı bir ziraat mühendisi tarafından verilmesi gerekmektedir.

⚠️ Çok Önemli: Danışmanlık özelliğinin çalışabilmesi için test_gui.py kodunun üst kısmında yer alan GEMINI_API_KEY değişkenine kendi Google AI Studio API anahtarınızı eklemeyi unutmayın!
