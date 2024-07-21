# Unit Test
---
## Giriş:
### Test Çeşitleri
#### Fonskiyonel Testler:
- Unit testing
- Integration testing
- End-to-end testing
- Smoke testing
- Sanity testing
- Regression testing
- Acceptance testing
- White-box testing
- Black box testing
- Interface testing
#### Fonksiyonel Olmayan Testler:
- Performance testing
- Security testing
- Load testing
- Failover testing
- Compatibility testing
- Usability testing
- Scalability testing
- Volume testing
- Stress testing
- Maintainability testing
- Compliance testing
- Efficiency testing
- Reliability testing
- Endurance testing
- Disaster recovery testing
- Localization testing
- Internationalization testing
### 3 Unit Test Concepts: NUnit - XUnit - MSTest
- NUnit: Eski .NET sürümlerini barındırır. Eskiden kullanımı daha yaygındı yerini XUnit ve MSTest'e bırakmıştır.
- XUnit: Güncel olarak en fazla kullanılan türdür. Topluluk tarafından geliştirilir daha yenilikçi ve kullanım açısından daha iyidir.
- MSTest: Microsoft tarafından geliştirilir.
---
## Tanımlar:
### İsimlendirme Kuralları: 
- Proje ismimizin sonunda Unit olduğunu belirtmemiz gerekir. Örneğin: ****.Test.Unit gibi.
- Class ismimiz ana projeyi içerecek şekilde yazılmalı. Örneğin: *****.Tests.cs gibi.
- Metod ismi içerisinde yaptığımız işlem belirtilmeli. *** _Should *** _When *** gibi should ve wheni şu durumda şu yapılıyor şeklinde belirtmekte kullanmalıyız.
### Arrange, Act, Assert: İlgili alanlarda yapılıp kodun okunabilirliği ve yönetilebilirliği için avantaj sağlar.
- Arrange: Class veya service newlenip instance düzeltilip değer set edildiği kısım. (Class-service oluşturma)
- Act: Metodların çağrıldığı,çalıştırldığı,sonuçların yakalandığı kısımdır. (Metod tetikleme)
- Assert: Sonuç kontrol edildiği ne olması gerektiğini uygualamya söylediğimiz kısımdır. (Sonuç kontrol)
---
## Teknikler:
---
## Konsept:
### Mocking: Sahte nesnelerle test yapılmasını sağlar. Moq ve NSubtitute Nuget paketleri ile bu işlem gerçekleştirilir.
---
## Gerçek Dünya:
---
#### Kaynakça
- Taner Saydam - Udemy - YouTube
- Nursema Gülmez - Medium
