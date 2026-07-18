# reyevAntiTarget

AverisCraft BoxMining sunucusu için geliştirilmiş, yüksek performanslı ElytraTarget & AutoFirework anti-cheat eklentisi.

## 🚀 Proje Hakkında
`reyevAntiTarget`, özellikle yüksek oyuncu kapasiteli (300+) sunucularda işlemciyi yormadan çalışması için tasarlanmıştır. Geleneksel Ağır elytratarget korumalarının aksine tamamen bir performans canavarıdır.

## ✨ Temel Özellikler
* **RayTrace & Reach Koruması:** `RayTrace` desteği ile duvar arkası vuruşları (WallHit) ve `3.15` blok ötesinden yapılan (Reach) vuruşlarını kesin olarak tespit eder.
* **Matematiksel Tespit:** `RotationConsistency` (Yaw/Pitch sapması) ve `Snap-to-Target` analizleri ile insan dışı kafa kilitleme hareketlerini ayırt eder.
* **Esnek Yaptırım Mekanizması:** İhlal eşikleri (Violation Threshold) aşıldığında otomatik ban/kick/mesaj sistemi.

## ⚙️ Teknik Gereksinimler
* **Sunucu Yazılımı:** Paper 1.21.4
* **Java:** 17 veya üzeri

## 📋 Kurulum
1. `reyevAntiTarget.jar` dosyasını sunucunuzun `plugins` klasörüne atın.
2. Sunucuyu başlatın (Eklenti `POSTWORLD` aşamasında yüklenecektir).
3. Oluşturulan `config.yml` dosyasını kendi sunucunuza göre düzenleyin.

## 🛠 Ayarlar (config.yml)
Eklent, sunucu performansını korumak için optimize edilmiş varsayılan değerlerle gelir. 

## ✨ Sipariş
* **Sipariş için discord: reyev

```yaml
detection:
  auto-firework:
    enabled: true
    max-ms-threshold: 90
    violation-threshold: 5
  rotation-consistency:
    enabled: true
    max-std-dev-threshold: 0.008

