# Dosya Arama Uygulaması (Django Projesi)

## Proje Açıklaması
Bu proje, kullanıcıların belirli bir konuya ve dosya türüne göre Google dork kullanarak dosya aramaları yapmalarını sağlar. Uygulama, arama sonuçlarını veritabanına kaydeder ve geçmiş arama sonuçlarını listeleyerek kullanıcılara sunar.

## Özellikler
- Kullanıcılar, konu ve dosya türünü seçerek arama yapabilir.
- Arama, Google dork kullanılarak gerçekleştirilir.
- Geçmiş aramalar veritabanına kaydedilir ve geçmiş aramalar listelenir.

## Gerekli Yazılımlar
- Python 3.x
- Django

## Kurulum Adımları
1. Projeyi bilgisayarınıza indirin.
2. Terminalde proje klasörüne gidin ve sanal ortamı etkinleştirin:
    ```bash
    python -m venv env
    source env/bin/activate  # Linux/Mac için
    env\Scripts\activate  # Windows için
    ```
3. Gerekli bağımlılıkları yüklemek için:
    ```bash
    pip install -r requirements.txt
    ```
4. Django'nun veritabanı migrasyonlarını uygulayın:
    ```bash
    python manage.py migrate
    ```
5. Sunucuyu başlatın:
    ```bash
    python manage.py runserver
    ```

Projenizi tarayıcıda şu adreste görebilirsiniz: [http://127.0.0.1:8000/arama/](http://127.0.0.1:8000/arama/)

## Kullanım
- Kullanıcılar, `Konu` ve `Dosya Türü` (PDF, DOCX, HTML, PNG) seçeneklerini girerek arama yapabilirler.
- Yapılan aramalar veritabanına kaydedilir ve geçmiş aramalar listelenir.
