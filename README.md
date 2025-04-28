# 🕵️‍♂️ İnsan Tespiti ve Sayımı - CCTV Görüntüleri Üzerinden

Bu proje, **ELM463 Dönem Projesi** kapsamında, güvenlik kameralarından elde edilen görüntüler üzerinde **sadece dijital görüntü işleme teknikleri** kullanılarak insan tespiti ve sayımı yapmayı amaçlamaktadır.

## İçerik

- Canny Edge Detection ile kenar çıkarımı
- Gölge kaldırma (Fourier Transform + Yüksek Geçiş Filtresi)
- Hough Transform ile düz çizgi temizleme
- Dilation (genleşme) işlemleri
- Connected Component Analysis (Bağlantılı Bileşen Analizi)
- Alan ve oran filtreleme
- İnsan sayımı ve sınırlayıcı kutular çizimi

## Proje Dosyaları

- `ŞULE NUR_DEMİRDAŞ_PRJ_REPORT.pdf` : Projenin ayrıntılı açıklamasını içeren rapor dosyası.
- `main.ipynb` : Projede kullanılan Python kodlarının yer aldığı Jupyter Notebook dosyası.

## Kullanılan Teknolojiler

- Python 3
- OpenCV
- NumPy
- Matplotlib

## Kurulum

Projeyi çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

```bash
git clone https://github.com/SuleDemirdas/cctv-human-detection-counting.git
cd cctv-human-detection-counting
pip install -r requirements.txt
```

> Not: `requirements.txt` dosyası yoksa, aşağıdaki temel paketlerin yüklü olduğundan emin olun:
> - opencv-python
> - numpy
> - matplotlib

## Çalıştırmak

Jupyter Notebook ortamında `main.ipynb` dosyasını açarak adım adım çalıştırabilirsiniz.

## Sonuçlar

Geliştirilen yöntem:
- Basit ve orta zorluktaki CCTV görüntülerinde yüksek doğruluk sağlamıştır.
- Karmaşık arka plan, düşük ışık gibi durumlarda doğrulukta düşüş gözlenmiştir.

Bazı örnek sonuçlar:
- Kolay görüntü: Başarılı tespit
- Gece görüntüsü: Kısmen başarılı
- Zor arka plan: Hatalı sayımlar

## Avantajlar

- Düşük maliyetli ve kolay uygulanabilir yöntem
- Gerçek zamanlı uygulamalara uygun altyapı
- Ekstra öğrenmeye gerek kalmadan temel görüntü işleme teknikleri ile çözüm

## Kısıtlamalar

- Düşük kaliteli görüntülerde hata oranı artabilir
- Gölgeler, düşük ışık ve karmaşık arka planlar sonuçları etkileyebilir
- Benzer renkli nesneler ayrımda zorluk çıkarabilir

## Kaynakça

- G. D. Finlayson, S. D. Hordley, Cheng Lu and M. S. Drew,  
  _"On the removal of shadows from images,"_  
  IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 28, no. 1, pp. 59-68, Jan. 2006.
