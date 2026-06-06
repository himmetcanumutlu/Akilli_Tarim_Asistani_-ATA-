# 🌱 ATA - Akıllı Tarım Asistanı / Intelligent Agriculture Assistant

**Yapay Zeka Destekli Mahsul Hastalığı Teşhis ve Dijital Zirai Danışmanlık Sistemi**  
**AI-Powered Crop Disease Diagnosis and Digital Agricultural Consulting System**

---

## 🇹🇷 Türkçe

**ATA - Akıllı Tarım Asistanı**, yapay zeka destekli bitki hastalığı teşhis ve dijital zirai danışmanlık sistemi olarak geliştirilmiştir. Projenin temel amacı, tarımsal üretimde verimliliği artırmak, hastalıkları erken evrede tespit etmek ve ürün kayıplarını teknoloji desteğiyle azaltmaktır.

Sistem, çiftçilerin ve tarım profesyonellerinin tarlalarındaki ürün hastalıklarını saniyeler içinde yüksek doğrulukla tespit etmelerine yardımcı olur. Akıllı Tarım Asistanı yalnızca hastalığı teşhis etmekle kalmaz; tespit edilen hastalığa, mahsul türüne ve bitkinin gelişim durumuna göre kullanıcıya özel, anlaşılır ve uygulanabilir bir **Acil Zirai Eylem Planı** da sunar. Bu danışmanlık süreci **Google Gemini AI** desteğiyle doğal, açıklayıcı ve pratik öneriler üretecek şekilde tasarlanmıştır.

---

## 🇬🇧 English

**ATA - Intelligent Agriculture Assistant** is developed as an AI-powered plant disease diagnosis and digital agricultural consulting system. The main goal of the project is to increase productivity in agricultural production, detect diseases at an early stage, and reduce crop loss with the help of technology.

The system helps farmers and agricultural professionals detect crop diseases in their fields within seconds and with high accuracy. The Intelligent Agriculture Assistant does not only diagnose the disease; it also provides a personalized, clear, and applicable **Emergency Agricultural Action Plan** based on the detected disease, crop type, and plant development status. This consulting process is designed to generate natural, explanatory, and practical recommendations with the support of **Google Gemini AI**.

---

# 📌 Proje Hakkında / About the Project

## 🇹🇷 Türkçe

**Akıllı Tarım Asistanı (ATA)**, modern yapay zeka tekniklerini kullanarak çiftçilere hızlı ve güvenilir bitki hastalığı teşhisi sunar. Sistem, yüklenen bitki görüntüsünü analiz eder, hastalık belirtilerini sınıflandırır ve sonuçları kullanıcıya anlaşılır biçimde gösterir. Böylece çiftçiler, hastalıkları erken fark ederek zamanında müdahale etme şansı elde eder.

Proje; görüntü sınıflandırma, açıklanabilir yapay zeka, test zamanı veri artırımı ve üretken yapay zeka destekli danışmanlık gibi bileşenleri bir araya getirir. Bu yapı sayesinde hem teknik doğruluk hem de son kullanıcı için anlaşılabilirlik hedeflenmiştir.

## 🇬🇧 English

The **Intelligent Agriculture Assistant (ATA)** uses modern artificial intelligence techniques to provide farmers with fast and reliable plant disease diagnosis. The system analyzes the uploaded plant image, classifies disease symptoms, and presents the results to the user in an understandable way. This allows farmers to detect diseases early and take action on time.

The project combines components such as image classification, explainable artificial intelligence, test-time augmentation, and generative AI-supported consulting. With this structure, the project aims to achieve both technical accuracy and usability for end users.

---

# 🚀 Öne Çıkan Özellikler / Key Features

## 🇹🇷 Türkçe

| Özellik | Açıklama |
| :--- | :--- |
| 🧠 **EfficientNet-B4 ile Gelişmiş Teşhis** | 12 farklı mahsul türünde yüksek doğruluklu ve hesaplama maliyeti optimize edilmiş derin öğrenme tabanlı teşhis sağlar. |
| 🔍 **Açıklanabilir Yapay Zeka (XAI - Grad-CAM)** | Modelin karar verdiği bölgeleri ısı haritası olarak görselleştirir ve sonuçların daha anlaşılır olmasını sağlar. |
| 🔄 **Test Zamanı Veri Artırımı (TTA)** | Tahmin aşamasında görüntüye uygulanan simetrik varyasyonlarla model kararlılığını artırır. |
| 🤖 **Gemini 1.5 Flash Destekli Zirai Danışman** | Tespit edilen hastalığa göre kültürel ve kimyasal mücadele yöntemlerini doğal dille sunar. |
| 📊 **Otonom Eğitim ve Loglama** | Yeni veri setleriyle eğitim yapabilir, EarlyStopping ile aşırı öğrenmeyi azaltır ve eğitim grafiklerini raporlar. |

ATA; domates, mısır, soya fasulyesi, üzüm, kayısı, pirinç, çilek, elma, buğday, arpa, patates ve şeftali gibi mahsuller üzerinde çalışacak şekilde tasarlanmıştır.

## 🇬🇧 English

| Feature | Description |
| :--- | :--- |
| 🧠 **Advanced Diagnosis with EfficientNet-B4** | Provides high-accuracy deep learning-based diagnosis for 12 different crop types with optimized computational cost. |
| 🔍 **Explainable AI (XAI - Grad-CAM)** | Visualizes the model's focus areas as heatmaps and makes predictions easier to understand. |
| 🔄 **Test-Time Augmentation (TTA)** | Improves prediction stability by applying symmetrical variations during inference. |
| 🤖 **Gemini 1.5 Flash Agricultural Consultant** | Provides cultural and chemical control recommendations in natural language based on the detected disease. |
| 📊 **Autonomous Training and Logging** | Supports training with new datasets, reduces overfitting with EarlyStopping, and reports training graphs. |

ATA is designed to work with crops such as tomato, corn, soybean, grape, apricot, rice, strawberry, apple, wheat, barley, potato, and peach.

---

# 📈 Model Performansı ve Kapsam / Model Performance and Scope

## 🇹🇷 Türkçe

Model, gelişmiş **Albumentations** veri artırma teknikleri ve **Karışık Hassasiyetli Eğitim (Mixed Precision)** kullanılarak eğitilmiştir. Bu sayede ışık parlamaları, görüntü bozulmaları ve zorlu saha koşulları altında bile yüksek başarı göstermesi hedeflenmiştir.

Aşağıdaki doğruluk oranları modelin farklı mahsuller üzerindeki performansını göstermektedir:

| 🌾 Mahsul | 🎯 Doğruluk Oranı |
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
| Şeftali | %95.58 |

## 🇬🇧 English

The model was trained using advanced **Albumentations** data augmentation techniques and **Mixed Precision** training. This approach aims to maintain high performance even under challenging conditions such as light reflections, image distortions, and difficult field environments.

The following accuracy rates show the model's performance across different crops:

| 🌾 Crop | 🎯 Accuracy Rate |
| :--- | ---: |
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
| Peach | 95.58% |

---

# 🗂️ Proje Mimarisi ve Klasör Yapısı / Project Architecture and Folder Structure

## 🇹🇷 Türkçe

Sistemin sürdürülebilirliği ve modülerliği için aşağıdaki dizin yapısı benimsenmiştir:

```text
ATA-Projesi/
│
├── data/
│   └── raw/                   # Eğitim fotoğraflarının bulunduğu ana dizin
├── grafikler/                 # Eğitim sürecinde otomatik üretilen Loss ve Accuracy grafikleri
├── gradcam_ornekleri/         # Modelin odaklandığı alanları gösteren Grad-CAM çıktıları
│
├── egitim_otomatik.py         # Mahsulleri sırayla eğiten, ağırlıkları kaydeden ve loglayan ana script
├── test_gui.py                # Gemini destekli, Tkinter tabanlı grafiksel kullanıcı arayüzü
├── requirements.txt           # Proje bağımlılıkları
└── README.md                  # Proje dokümantasyonu
```

`data/raw/` klasörü eğitim görsellerinin bulunduğu ana dizindir. `grafikler/` klasörü eğitim sürecinde otomatik oluşturulan Loss ve Accuracy grafiklerini içerir. `gradcam_ornekleri/` klasörü modelin hangi bölgelere odaklandığını gösteren Grad-CAM çıktılarını saklar. `egitim_otomatik.py` ana eğitim scriptidir, `test_gui.py` ise Gemini destekli son kullanıcı arayüzünü başlatır.

## 🇬🇧 English

The following directory structure is used to keep the system sustainable and modular:

```text
ATA-Projesi/
│
├── data/
│   └── raw/                   # Main directory containing training images
├── grafikler/                 # Automatically generated Loss and Accuracy graphs during training
├── gradcam_ornekleri/         # Grad-CAM outputs showing the model's focus areas
│
├── egitim_otomatik.py         # Main script that trains crops sequentially, saves weights, and logs results
├── test_gui.py                # Gemini-supported Tkinter-based graphical user interface
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation
```

The `data/raw/` folder is the main directory containing training images. The `grafikler/` folder contains automatically generated Loss and Accuracy graphs during training. The `gradcam_ornekleri/` folder stores Grad-CAM outputs showing where the model focuses. `egitim_otomatik.py` is the main training script, while `test_gui.py` launches the Gemini-supported end-user interface.

---

# ⚙️ Kurulum ve Sistem Gereksinimleri / Installation and System Requirements

## Gereksinimler / Requirements

| Gereksinim | Açıklama |
| :--- | :--- |
| 🐍 Python | Python 3.8 veya üzeri / Python 3.8 or higher |
| 🚀 GPU | CUDA destekli GPU önerilir / CUDA-supported GPU is recommended for faster training |

---

## Kurulum Adımları / Installation Steps

Projeyi kullanmaya başlamak için depoyu bilgisayarınıza klonlayın ve proje dizinine girin:

```bash
git clone https://github.com/UfukAlparslan19/ATA-Projesi.git
cd ATA-Projesi
```

Gerekli bağımlılıkları yükleyin:

```bash
pip install -r requirements.txt
```

Eğer `requirements.txt` dosyasını kullanmıyorsanız, gerekli temel paketleri aşağıdaki komutla manuel olarak kurabilirsiniz:

```bash
pip install torch torchvision opencv-python numpy albumentations matplotlib grad-cam google-generativeai tqdm
```

To get started, clone the repository to your computer and enter the project directory:

```bash
git clone https://github.com/UfukAlparslan19/ATA-Projesi.git
cd ATA-Projesi
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

If you are not using the `requirements.txt` file, you can manually install the required core packages with the following command:

```bash
pip install torch torchvision opencv-python numpy albumentations matplotlib grad-cam google-generativeai tqdm
```

---

# 🔑 LLM API Entegrasyonu / LLM API Integration

## 🇹🇷 Türkçe

Projenin üretken zirai danışmanlık özelliğinin çalışabilmesi için `test_gui.py` dosyasının üst kısmında yer alan `GEMINI_API_KEY` değişkenine kendi **Google AI Studio API** anahtarınızı tanımlamanız gerekmektedir. API anahtarı eklenmeden üretken yapay zeka destekli tavsiye özelliği çalışmayabilir.

## 🇬🇧 English

For the generative agricultural consulting feature to work, you must define your own **Google AI Studio API** key in the `GEMINI_API_KEY` variable located at the top of the `test_gui.py` file. Without adding an API key, the generative AI-supported recommendation feature may not work.

---

# 🧪 Kullanım Kılavuzu / Usage Guide

## 1. Model Eğitimi / Model Training

Kendi veri setlerinizle veya sağlanan veri setiyle modeli sıfırdan eğitmek, ağırlık dosyalarını güncellemek ve modelin başarım grafiklerini oluşturmak için aşağıdaki komutu çalıştırın:

```bash
python egitim_otomatik.py
```

Developers can train the model from scratch using their own agricultural data or the provided dataset, update model weights, and generate performance graphs with the following command:

```bash
python egitim_otomatik.py
```

---

## 2. Grafiksel Kullanıcı Arayüzü / Graphical User Interface

Tarımsal araziden çekilmiş bir yaprak görüntüsünü sisteme yüklemek, Grad-CAM ile enfeksiyon analizini görmek ve Gemini yapay zeka asistanından anlık tavsiye almak için arayüzü başlatın:

```bash
python test_gui.py
```

To upload a leaf image, view infection analysis with Grad-CAM, and receive instant advice from the Gemini AI assistant, launch the interface:

```bash
python test_gui.py
```

---

# 🤝 Katkıda Bulunma / Contributing

## 🇹🇷 Türkçe

ATA, açık kaynaklı bir topluluk projesi olarak katkılara açıktır. Algoritma optimizasyonları, yeni mahsul veri setleri veya arayüz iyileştirmeleri gibi konulardaki katkılarınızı bekliyoruz.

1. Bu depoyu fork edin.
2. Üzerinde çalışacağınız yeni bir özellik dalı oluşturun:

```bash
git checkout -b feature/YeniOzellik
```

3. Geliştirmelerinizi commit edin:

```bash
git commit -m "Özellik: X eklendi ve Y optimize edildi"
```

4. Dalınızı uzak sunucuya gönderin:

```bash
git push origin feature/YeniOzellik
```

5. Bir Pull Request oluşturarak inceleme sürecini başlatın.

## 🇬🇧 English

ATA is open to contributions as an open-source community project. Contributions such as algorithm optimizations, new crop datasets, or interface improvements are welcome.

1. Fork this repository.
2. Create a new feature branch:

```bash
git checkout -b feature/NewFeature
```

3. Commit your changes:

```bash
git commit -m "Feature: Added X and optimized Y"
```

4. Push your branch to the remote repository:

```bash
git push origin feature/NewFeature
```

5. Open a Pull Request to start the review process.

---

# 📄 Lisans / License

## 🇹🇷 Türkçe

Bu proje MIT Lisansı koşulları altında açık kaynak olarak sunulmuştur. Detaylı bilgi ve yasal çerçeve için dizindeki `LICENSE` dosyasını inceleyebilirsiniz.

## 🇬🇧 English

This project is released as open source under the terms of the MIT License. For detailed information and legal terms, please review the `LICENSE` file in the repository.

---

# ⚠️ Yasal Uyarı ve Sorumluluk Reddi / Legal Notice and Disclaimer

## 🇹🇷 Türkçe

ATA - Akıllı Tarım Asistanı, zirai süreçlerde erken teşhise yardımcı olmak ve veri odaklı karar almayı desteklemek amacıyla tasarlanmış bir yapay zeka aracıdır. Sistem tarafından verilen öneriler destekleyici niteliktedir. Kritik zirai müdahalelerde, ilaçlama dozajlamalarında ve kesin hasar tespitlerinde nihai kararın lisanslı bir ziraat mühendisi veya yetkili bir tarım danışmanı tarafından verilmesi gerekmektedir.

## 🇬🇧 English

ATA - Intelligent Agriculture Assistant is an artificial intelligence tool designed to assist with early diagnosis in agricultural processes and support data-driven decision-making. The recommendations generated by the system are supportive in nature. For critical agricultural interventions, pesticide dosage decisions, and final damage assessments, the final decision should be made by a licensed agricultural engineer or an authorized agricultural consultant.

---

> ⚠️ **Çok Önemli / Important:** Danışmanlık özelliğinin çalışabilmesi için `test_gui.py` kodunun üst kısmında yer alan `GEMINI_API_KEY` değişkenine kendi Google AI Studio API anahtarınızı eklemeyi unutmayın.
