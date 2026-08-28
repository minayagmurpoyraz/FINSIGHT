# FINSIGHT — AI Destekli Fon Portföy Karar Destek Sistemi

**İnfina Akademi 2026 | FirstClass Ürün Ekibi**
🏆 *Ürün ve Süreç Yönetimi kategorisinde 1.'lik ödülü*

FINSIGHT, profesyonel portföy yöneticilerine (PY) yönelik, **human-in-the-loop** prensibiyle çalışan bir AI destekli fon portföy karar destek platformudur. Yapay zeka hiçbir zaman otonom karar almaz; öneri sunar, nihai kararı her zaman portföy yöneticisi verir.

Referans fon: **TIE — İş Portföy BIST 30 Endeksi Hisse Senedi Fonu**

🔗 **Canlı Demo:** [https://(https://github.com/minayagmurpoyraz/FINSIGHT)

---

## Ekranlar

1. **Login** — Giriş ekranı
2. **Fon Dashboard** — Anlık ve dönemsel KPI kartları, benchmark karşılaştırması
3. **AI Önerisi & Karar** — Kural tabanlı AI önerileri, top-10/"Diğer" hisse kırılımı
4. **Performans Karşılaştırması** — Simülasyon portföyü, benchmark analizi
5. **Stres Testi** — Senaryo bazlı sapma sınırı simülasyonu
6. **Karar Geçmişi** — Alınan kararların kayıt ve takibi
7. **Yönetim Paneli** — Yönetici görünümü

## Öne Çıkan Tasarım Kararları

- **Anlık vs. Dönemsel KPI mimarisi**: Toplam Portföy Değeri ve Günlük Getiri sabit noktasal metrikler; Birikimli Getiri ve Benchmark Farkı seçilen döneme göre yeniden hesaplanır.
- **±10pp sapma sınırı**: Varlık bazlı uygulanır, toplam %100 kısıtından bağımsızdır.
- **Top-10 / "Diğer" mimarisi**: AI yalnızca en büyük 10 hisseyi önerebilir; kalan grup ("Diğer") toplamı offset formülüyle korur.
- **applyDecision() tek doğruluk kaynağı**: Hem AI onaylı hem manuel kararlar bu fonksiyon üzerinden işlenir; gerçek ağırlıklar yalnızca açık "uygula" adımında güncellenir.
- **Üç katmanlı stres testi doğrulaması**: Sert sınırlar, yumuşak eşik uyarısı, matematiksel güvenlik tabanı.

## Kullanılan Yöntem ve Araçlar

Ürün stratejisi · PRD & teknik dokümantasyon · KPI/metrik tasarımı · kullanıcı senaryosu & test tasarımı · interaktif HTML/JS prototipleme · çapraz ekip koordinasyonu · jüri/paydaş sunumu

---

*Bu prototip mock/synthetic veri kullanmaktadır; gerçek İnfina servis verileri ve Ar-Ge tarafından geliştirilen ONNX tahmin modeli entegre edilmemiştir.*
