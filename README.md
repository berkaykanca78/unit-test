# Unit Test
---
## Introduction
### Three Unit Test Concepts: NUnit - XUnit - MSTest
- NUnit: Eski .NET sürümlerini barındırır. Eskiden kullanımı daha yaygındı yerini XUnit ve MSTest'e bırakmıştır.
- XUnit: Güncel olarak en fazla kullanılan türdür. Topluluk tarafından geliştirilir daha yenilikçi ve kullanım açısından daha iyidir.
- MSTest: Microsoft tarafından geliştirilir.
---
## Fundamentals
### İsimlendirme Kuralları: 
- Proje ismimizin sonunda Unit olduğunu belirtmemiz gerekir. Örneğin: ****.Test.Unit gibi.
- Class ismimiz ana projeyi içerecek şekilde yazılmalı. Örneğin: *****.Tests.cs gibi.
- Metod ismi içerisinde yaptığımız işlem belirtilmeli. ***_Should***_When*** gibi should ve wheni şu durumda şu yapılıyor şeklinde belirtmekte kullanmalıyız.
### Arrange, Act, Assert: İlgili alanlarda yapılıp kodun okunabilirliği ve yönetilebilirliği için avantaj sağlar.
- Arrange: Class veya service newlenip instance düzeltilip değer set edildiği kısım. (Class-service oluşturma)
- Act: Metodların çağrıldığı,çalıştırldığı,sonuçların yakalandığı kısımdır. (Metod tetikleme)
- Asset: Sonuç kontrol edildiği ne olması gerektiğini uygualamya söylediğimiz kısımdır. (Sonuç kontrol)
---
## Techniques
---
## Concepts
---
## Real Worlds
---
#### Kaynakça
- Taner Saydam - Udemy - YouTube
