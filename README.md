# ATA - Akıllı Tarım Asistanı / Intelligent Agriculture Assistant

## Türkçe

ATA - Akıllı Tarım Asistanı, yapay zeka destekli bitki hastalığı teşhis ve dijital zirai danışmanlık sistemi olarak geliştirilmiştir. Projenin temel amacı, tarımda verimi artırmak ve ürün kaybını teknoloji desteğiyle azaltmaktır. Sistem, çiftçilerin tarlalarındaki ürün hastalıklarını saniyeler içinde yüksek doğrulukla tespit etmelerine yardımcı olur.

Akıllı Tarım Asistanı yalnızca hastalığı teşhis etmekle kalmaz; tespit edilen hastalığa, mahsul türüne ve bitkinin boyuna göre çiftçiye özel, anlaşılır ve hemen uygulanabilir bir Acil Zirai Eylem Planı da sunar. Bu danışmanlık süreci Google Gemini AI desteğiyle doğal, açıklayıcı ve uygulanabilir öneriler üretecek şekilde tasarlanmıştır.

## English

ATA - Intelligent Agriculture Assistant is developed as an AI-powered plant disease diagnosis and digital agricultural consulting system. The main goal of the project is to increase productivity in agriculture and reduce crop loss with the help of technology. The system helps farmers detect crop diseases in their fields within seconds and with high accuracy.

The Intelligent Agriculture Assistant does not only diagnose the disease; it also provides a personalized, clear, and immediately applicable Emergency Agricultural Action Plan based on the detected disease, crop type, and plant size. This consulting process is designed to generate natural, explanatory, and practical recommendations with the support of Google Gemini AI.

---

# Proje Hakkında / About the Project

## Türkçe

Akıllı Tarım Asistanı (ATA), modern yapay zeka tekniklerini kullanarak çiftçilere hızlı ve güvenilir bitki hastalığı teşhisi sunar. Sistem, yüklenen bitki görüntüsünü analiz eder, hastalık belirtilerini sınıflandırır ve sonuçları kullanıcıya anlaşılır biçimde gösterir. Böylece çiftçiler, hastalıkları erken fark ederek zamanında müdahale etme şansı elde eder.

Proje, görüntü sınıflandırma, açıklanabilir yapay zeka, test zamanı veri artırımı ve üretken yapay zeka destekli danışmanlık gibi bileşenleri bir araya getirir. Bu yapı sayesinde hem teknik doğruluk hem de son kullanıcı için anlaşılabilirlik hedeflenmiştir.

## English

The Intelligent Agriculture Assistant (ATA) uses modern artificial intelligence techniques to provide farmers with fast and reliable plant disease diagnosis. The system analyzes the uploaded plant image, classifies disease symptoms, and presents the results to the user in an understandable way. This allows farmers to detect diseases early and take action on time.

The project combines components such as image classification, explainable artificial intelligence, test-time augmentation, and generative AI-supported consulting. With this structure, the project aims to achieve both technical accuracy and usability for end users.

---

# Öne Çıkan Özellikler / Key Features

## Türkçe

ATA, derin öğrenme tabanlı teşhis özelliğiyle 12 farklı tarımsal üründe hastalık tespiti yapabilir. Gelişmiş EfficientNet-B4 mimarisi kullanılarak mikroskobik düzeyde hassas teşhis hedeflenmiştir. Sistem; domates, mısır, soya fasulyesi, üzüm, kayısı, pirinç, çilek, elma, buğday, arpa, patates ve şeftali gibi mahsuller üzerinde çalışacak şekilde tasarlanmıştır.

Açıklanabilir Yapay Zeka (XAI) desteği sayesinde modelin kararını neye göre verdiği Grad-CAM algoritması ile görselleştirilir. Bu yöntem, yapraktaki hastalıklı bölgeleri bir röntgen görüntüsü gibi işaretleyerek kullanıcının model sonucunu daha kolay anlamasını sağlar. Test Zamanı Veri Artırımı (TTA) ise tahmin aşamasında simetrik varyasyonlar oluşturarak teşhisin daha kararlı ve güvenilir olmasına katkı sağlar.

Gemini 1.5 Flash desteğiyle çalışan üretken yapay zeka danışmanı, tespit edilen hastalığı analiz ederek çiftçiye kültürel ve kimyasal mücadele yöntemlerini doğal bir dille sunar. Ayrıca proje, yeni veriler eklendiğinde otonom olarak öğrenebilen, EarlyStopping ile durması gereken noktayı belirleyebilen ve eğitim sonuçlarını grafiklerle raporlayabilen akıllı bir eğitim döngüsüne sahiptir.

## English

ATA can detect diseases in 12 different agricultural crops with its deep learning-based diagnosis feature. Using the advanced EfficientNet-B4 architecture, the system aims to deliver highly sensitive diagnosis. It is designed to work with crops such as tomato, corn, soybean, grape, apricot, rice, strawberry, apple, wheat, barley, potato, and peach.

With Explainable Artificial Intelligence (XAI) support, the model's decision-making process is visualized using the Grad-CAM algorithm. This method highlights diseased areas on the leaf like an X-ray image, helping users better understand the model's prediction. Test-Time Augmentation (TTA) contributes to more stable and reliable diagnosis by generating symmetrical variations during the prediction stage.

The generative AI consultant powered by Gemini 1.5 Flash analyzes the detected disease and presents cultural and chemical control methods to the farmer in natural language. The project also includes an intelligent training loop that can learn autonomously when new data is added, determine when to stop using EarlyStopping, and report training results with visual graphs.

---

# Model Performansı ve Kapsam / Model Performance and Scope

## Türkçe

Model, gelişmiş Albumentations veri artırma teknikleri ve Karışık Hassasiyetli Eğitim (Mixed Precision) kullanılarak eğitilmiştir. Bu sayede ışık parlamaları, görüntü bozulmaları ve zorlu saha koşulları altında bile yüksek başarı göstermesi hedeflenmiştir.

Aşağıdaki doğruluk oranları modelin farklı mahsuller üzerindeki performansını göstermektedir:

| Mahsul | Doğruluk Oranı |
|---|---:|
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

## English

The model was trained using advanced Albumentations data augmentation techniques and Mixed Precision training. This approach aims to maintain high performance even under challenging conditions such as light reflections, image distortions, and difficult field environments.

The following accuracy rates show the model's performance across different crops:

| Crop | Accuracy Rate |
|---|---:|
| Tomato | 99.49% |
| Corn | 97.12% |
| Soybean | 96.65% |
| Grape | 96.45% |
| Apricot | 96.07% |
| Rice | 94.76% |
| Strawberry | 92.33% |
| Apple | 92.96% |
| Wheat | 92.81% |
| Barley | 92.59% |
| Potato | 90.55% |
| Peach | 85.58% |

---

# Klasör Yapısı / Folder Structure

## Türkçe

Projenin düzenli ve sürdürülebilir şekilde çalışması için aşağıdaki klasör yapısı önerilir:

```text
ATA-Projesi/
│
├── data/
│   └── raw/                   # Eğitim fotoğraflarının bulunduğu ana dizin
├── grafikler/                 # Eğitim sürecinde otomatik üretilen Loss/Acc grafikleri
├── gradcam_ornekleri/         # Modelin odak noktalarını gösteren Grad-CAM çıktıları
│
├── egitim_otomatik.py         # 12 mahsulü sırayla eğiten, grafikleri ve Grad-CAM'i çıkaran ana script
├── test_gui.py                # Gemini destekli, Tkinter tabanlı son kullanıcı arayüzü
├── requirements.txt           # Gerekli kütüphaneler
└── README.md                  # Proje dokümantasyonu
```

`data/raw/` klasörü eğitim görsellerinin bulunduğu ana dizindir. `grafikler/` klasörü eğitim sürecinde otomatik oluşturulan Loss ve Accuracy grafiklerini içerir. `gradcam_ornekleri/` klasörü modelin hangi bölgelere odaklandığını gösteren Grad-CAM çıktılarını saklar. `egitim_otomatik.py` ana eğitim scriptidir, `test_gui.py` ise Gemini destekli son kullanıcı arayüzünü başlatır.

## English

The following folder structure is recommended to keep the project organized and maintainable:

```text
ATA-Project/
│
├── data/
│   └── raw/                   # Main directory containing training images
├── grafikler/                 # Automatically generated Loss/Accuracy graphs during training
├── gradcam_ornekleri/         # Grad-CAM outputs showing the model's focus areas
│
├── egitim_otomatik.py         # Main script that trains 12 crops sequentially and generates graphs and Grad-CAM outputs
├── test_gui.py                # Gemini-supported Tkinter-based end-user interface
├── requirements.txt           # Required libraries
└── README.md                  # Project documentation
```

The `data/raw/` folder is the main directory containing training images. The `grafikler/` folder contains automatically generated Loss and Accuracy graphs during training. The `gradcam_ornekleri/` folder stores Grad-CAM outputs showing where the model focuses. `egitim_otomatik.py` is the main training script, while `test_gui.py` launches the Gemini-supported end-user interface.

---

# Kurulum ve Kullanım Başlangıcı / Installation and Getting Started

## Türkçe

Projeyi kullanmaya başlamak için öncelikle depoyu bilgisayarınıza klonlayın ve proje dizinine girin. Ardından gerekli yapay zeka ve görüntü işleme kütüphanelerini `requirements.txt` dosyası üzerinden yükleyin.

```bash
git clone https://github.com/KULLANICI_ADINIZ/ATA-Projesi.git
cd ATA-Projesi
pip install -r requirements.txt
```

Eğer `requirements.txt` dosyasını kullanmıyorsanız, gerekli temel paketleri aşağıdaki komutla manuel olarak kurabilirsiniz:

```bash
pip install torch torchvision opencv-python numpy albumentations matplotlib grad-cam google-generativeai tqdm
```

## English

To get started with the project, first clone the repository to your computer and enter the project directory. Then install the required artificial intelligence and image processing libraries using the `requirements.txt` file.

```bash
git clone https://github.com/YOUR_USERNAME/ATA-Project.git
cd ATA-Projesi
pip install -r requirements.txt
```

If you are not using the `requirements.txt` file, you can manually install the required core packages with the following command:

```bash
pip install torch torchvision opencv-python numpy albumentations matplotlib grad-cam google-generativeai tqdm
```

---

# Model Eğitimi / Model Training

## Türkçe

Geliştiriciler, kendi tarımsal verileriyle veya sağlanan veri setiyle modeli sıfırdan eğitmek için aşağıdaki komutu kullanabilir:

```bash
python egitim_otomatik.py
```

Bu komut, klasördeki tüm bitkileri sırayla gezer, modeli eğitir, en iyi `.pth` model ağırlıklarını kaydeder ve eğitim sonuç raporlarını üretir. Eğitim sürecinde Loss ve Accuracy grafikleri otomatik olarak oluşturulur. Grad-CAM çıktıları da modelin hangi bölgelere odaklandığını göstermek için kaydedilir.

## English

Developers can train the model from scratch using their own agricultural data or the provided dataset with the following command:

```bash
python egitim_otomatik.py
```

This command processes all plants in the folder sequentially, trains the model, saves the best `.pth` model weights, and generates training result reports. During training, Loss and Accuracy graphs are created automatically. Grad-CAM outputs are also saved to show which regions the model focuses on.

---

# Akıllı Asistanı Başlatma / Launching the Intelligent Assistant

## Türkçe

Çiftçilerin fotoğraf yükleyip Gemini AI üzerinden zirai tavsiye alabileceği görsel arayüzü başlatmak için aşağıdaki komutu kullanabilirsiniz:

```bash
python test_gui.py
```

Danışmanlık özelliğinin çalışabilmesi için `test_gui.py` dosyasının üst kısmında bulunan `GEMINI_API_KEY` değişkenine kendi Google AI Studio API anahtarınızı eklemeniz gerekir. API anahtarı eklenmeden üretken yapay zeka destekli tavsiye özelliği çalışmayabilir.

## English

To launch the visual interface where farmers can upload photos and receive agricultural advice through Gemini AI, use the following command:

```bash
python test_gui.py
```

For the consulting feature to work, you must add your own Google AI Studio API key to the `GEMINI_API_KEY` variable located at the top of the `test_gui.py` file. Without adding an API key, the generative AI-supported recommendation feature may not work.

---

# Not / Note

## Türkçe

Bu proje, tarımsal hastalık teşhisine yardımcı olmak ve çiftçilere dijital danışmanlık sağlamak amacıyla geliştirilmiştir. Sistem tarafından verilen öneriler destekleyici niteliktedir. Kritik zirai kararlar alınmadan önce uzman bir ziraat mühendisine veya yetkili bir tarım danışmanına başvurulması önerilir.

## English

This project was developed to assist with agricultural disease diagnosis and provide digital consulting support to farmers. The recommendations generated by the system are supportive in nature. Before making critical agricultural decisions, it is recommended to consult a professional agricultural engineer or an authorized agricultural advisor.
