# Unit Test

![Unit Test](https://files.realpython.com/media/Python-unittest_Watermarked.f6549bba7422.jpg)

---

## Giriş

### Test Çeşitleri

#### Fonksiyonel Testler

| #  | Test Türü                  |
|----|----------------------------|
| 1  | Unit Testing               |
| 2  | Integration Testing         |
| 3  | End-to-End Testing          |
| 4  | Smoke Testing              |
| 5  | Sanity Testing             |
| 6  | Regression Testing         |
| 7  | Acceptance Testing         |
| 8  | White-box Testing          |
| 9  | Black Box Testing          |
| 10 | Interface Testing          |

#### Fonksiyonel Olmayan Testler

| #  | Test Türü                      |
|----|--------------------------------|
| 1  | Performance Testing            |
| 2  | Security Testing               |
| 3  | Load Testing                   |
| 4  | Failover Testing               |
| 5  | Compatibility Testing          |
| 6  | Usability Testing              |
| 7  | Scalability Testing            |
| 8  | Volume Testing                 |
| 9  | Stress Testing                 |
| 10 | Maintainability Testing        |
| 11 | Compliance Testing             |
| 12 | Efficiency Testing             |
| 13 | Reliability Testing            |
| 14 | Endurance Testing              |
| 15 | Disaster Recovery Testing      |
| 16 | Localization Testing           |
| 17 | Internationalization Testing   |

### 3 Unit Test Concepts

- **NUnit**: Eski .NET sürümlerini barındırır. Eskiden kullanımı daha yaygındı, yerini XUnit ve MSTest'e bırakmıştır.
- **XUnit**: Güncel olarak en fazla kullanılan türdür. Topluluk tarafından geliştirilir ve daha yenilikçi bir yapıya sahiptir.
- **MSTest**: Microsoft tarafından geliştirilir.

---

## Tanımlar

### İsimlendirme Kuralları

| Kural           | Açıklama                                                                                     |
|-----------------|----------------------------------------------------------------------------------------------|
| Proje İsmi       | Proje ismimizin sonunda "Unit" kelimesini belirtmemiz gerekir. Örneğin: `*****.Test.Unit` gibi. |
| Class İsmi       | Class ismimiz ana projeyi içerecek şekilde yazılmalıdır. Örneğin: `*****.Tests.cs` gibi.       |
| Metod İsmi       | Metod ismi içerisinde yaptığımız işlem belirtilmelidir. `***_Should_***_When_***` gibi should ve when ifadeleri kullanılarak "şu durumda şu yapılıyor" şeklinde belirtilebilir. |

### Arrange, Act, Assert

| Adım    | Açıklama                                                                                           |
|---------|----------------------------------------------------------------------------------------------------|
| Arrange | Class veya service newlenip instance oluşturulur ve değer set edilir. (Class-service oluşturma)   |
| Act     | Metodların çağrıldığı, çalıştırıldığı ve sonuçların yakalandığı kısımdır. (Metod tetikleme)      |
| Assert  | Sonuç kontrol edilir, ne olması gerektiği uygulanmaya söylenir. (Sonuç kontrol)                   |

### Ignore Test (Skip)

`Fact` veya `Theory` kullanırken içerisine parametre olarak `Skip('Neden')` ekleyebilirsiniz. Bu, unit testlerinizin başında ünlem işareti çıkar ve bu testi atlayacağını belirtir.

### Parameterizing Testing

`Theory` kullanarak, altına `InlineData` içerisinde parametrelerinizi ekleyebilir ve testlerinizi birden fazla veri ile sağlayabilirsiniz. Kod kopyalamak yerine bu yöntemle birçok veri ile test edebilirsiniz.

---

## Teknikler

### Fluent Assertion

| Kavram            | Açıklama                                                                                 |
|-------------------|------------------------------------------------------------------------------------------|
| Fluent Assertions | xUnit'deki Assert kısmına "Should Be" gibi daha anlaşılır ifadeler ekleyen bir Nuget kütüphanesidir. Assert işlemleri için tercih edilmesi tavsiye edilir. Daha okunaklı ve özellikli bir kütüphanedir. İngilizce yazım gibidir ve sadedir. |

### Tiplere Göre Testler

| #  | Test Türü             |
|----|-----------------------|
| 1  | String Test           |
| 2  | Number Test           |
| 3  | Date Test             |
| 4  | Object Test           |
| 5  | Enumerables Test      |
| 6  | Throw Exception Test  |
| 7  | Raised Events Test    |
| 8  | Private Method Test   |
| 9  | Internal Method Test  |

---

## Konsept

### Mocking

| Kavram    | Açıklama                                                                                                  |
|-----------|-----------------------------------------------------------------------------------------------------------|
| Mocking   | Sahte nesnelerle test yapılmasını sağlar. Moq ve NSubstitute Nuget paketleri ile bu işlem gerçekleştirilir. NSubstitute yazım olarak Moq kütüphanesinden daha basittir ve tercih edilebilir. |

---

## Gerçek Dünya

---

## Kaynakça

| Yazar           | Kaynak         |
|-----------------|----------------|
| Taner Saydam    | Udemy - YouTube|
| Nursema Gülmez  | Medium         |
