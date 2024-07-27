# Unit Test

![Unit Test](https://files.realpython.com/media/Python-unittest_Watermarked.f6549bba7422.jpg)

---

## Giriş

### Test Çeşitleri

#### Fonksiyonel Testler

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Test Türü</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Unit Testing</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Integration Testing</td>
    </tr>
    <tr>
      <td>3</td>
      <td>End-to-End Testing</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Smoke Testing</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Sanity Testing</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Regression Testing</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Acceptance Testing</td>
    </tr>
    <tr>
      <td>8</td>
      <td>White-box Testing</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Black Box Testing</td>
    </tr>
    <tr>
      <td>10</td>
      <td>Interface Testing</td>
    </tr>
  </tbody>
</table>

#### Fonksiyonel Olmayan Testler

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Test Türü</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Performance Testing</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Security Testing</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Load Testing</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Failover Testing</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Compatibility Testing</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Usability Testing</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Scalability Testing</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Volume Testing</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Stress Testing</td>
    </tr>
    <tr>
      <td>10</td>
      <td>Maintainability Testing</td>
    </tr>
    <tr>
      <td>11</td>
      <td>Compliance Testing</td>
    </tr>
    <tr>
      <td>12</td>
      <td>Efficiency Testing</td>
    </tr>
    <tr>
      <td>13</td>
      <td>Reliability Testing</td>
    </tr>
    <tr>
      <td>14</td>
      <td>Endurance Testing</td>
    </tr>
    <tr>
      <td>15</td>
      <td>Disaster Recovery Testing</td>
    </tr>
    <tr>
      <td>16</td>
      <td>Localization Testing</td>
    </tr>
    <tr>
      <td>17</td>
      <td>Internationalization Testing</td>
    </tr>
  </tbody>
</table>

### 3 Unit Test Concepts

- **NUnit**: Eski .NET sürümlerini barındırır. Eskiden kullanımı daha yaygındı, yerini XUnit ve MSTest'e bırakmıştır.
- **XUnit**: Güncel olarak en fazla kullanılan türdür. Topluluk tarafından geliştirilir ve daha yenilikçi bir yapıya sahiptir.
- **MSTest**: Microsoft tarafından geliştirilir.

---

## Tanımlar

### İsimlendirme Kuralları

<table>
  <thead>
    <tr>
      <th>Kural</th>
      <th>Açıklama</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Proje İsmi</td>
      <td>Proje ismimizin sonunda "Unit" kelimesini belirtmemiz gerekir. Örneğin: `*****.Test.Unit` gibi.</td>
    </tr>
    <tr>
      <td>Class İsmi</td>
      <td>Class ismimiz ana projeyi içerecek şekilde yazılmalıdır. Örneğin: `*****.Tests.cs` gibi.</td>
    </tr>
    <tr>
      <td>Metod İsmi</td>
      <td>Metod ismi içerisinde yaptığımız işlem belirtilmelidir. `***_Should_***_When_***` gibi should ve when ifadeleri kullanılarak "şu durumda şu yapılıyor" şeklinde belirtilebilir.</td>
    </tr>
  </tbody>
</table>

### Arrange, Act, Assert

<table>
  <thead>
    <tr>
      <th>Adım</th>
      <th>Açıklama</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Arrange</td>
      <td>Class veya service newlenip instance oluşturulur ve değer set edilir. (Class-service oluşturma)</td>
    </tr>
    <tr>
      <td>Act</td>
      <td>Metodların çağrıldığı, çalıştırıldığı ve sonuçların yakalandığı kısımdır. (Metod tetikleme)</td>
    </tr>
    <tr>
      <td>Assert</td>
      <td>Sonuç kontrol edilir, ne olması gerektiği uygulanmaya söylenir. (Sonuç kontrol)</td>
    </tr>
  </tbody>
</table>

### Ignore Test (Skip)

`Fact` veya `Theory` kullanırken içerisine parametre olarak `Skip('Neden')` ekleyebilirsiniz. Bu, unit testlerinizin başında ünlem işareti çıkar ve bu testi atlayacağını belirtir.

### Parameterizing Testing

`Theory` kullanarak, altına `InlineData` içerisinde parametrelerinizi ekleyebilir ve testlerinizi birden fazla veri ile sağlayabilirsiniz. Kod kopyalamak yerine bu yöntemle birçok veri ile test edebilirsiniz.

---

## Teknikler

### Fluent Assertion

<table>
  <thead>
    <tr>
      <th>Kavram</th>
      <th>Açıklama</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fluent Assertions</td>
      <td>xUnit'deki Assert kısmına "Should Be" gibi daha anlaşılır ifadeler ekleyen bir Nuget kütüphanesidir. Assert işlemleri için tercih edilmesi tavsiye edilir. Daha okunaklı ve özellikli bir kütüphanedir. İngilizce yazım gibidir ve sadedir.</td>
    </tr>
  </tbody>
</table>

### Tiplere Göre Testler

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Test Türü</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>String Test</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Number Test</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Date Test</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Object Test</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Enumerables Test</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Throw Exception Test</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Raised Events Test</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Private Method Test</td>
    </tr>
    <tr>
      <td>9</td>
      <td>Internal Method Test</td>
    </tr>
  </tbody>
</table>

---

## Konsept

### Mocking

<table>
  <thead>
    <tr>
      <th>Kavram</th>
      <th>Açıklama</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Mocking</td>
      <td>Sahte nesnelerle test yapılmasını sağlar. Moq ve NSubstitute Nuget paketleri ile bu işlem gerçekleştirilir. NSubstitute yazım olarak Moq kütüphanesinden daha basittir ve tercih edilebilir.</td>
    </tr>
  </tbody>
</table>

---

## Gerçek Dünya

---

## Kaynakça

<table>
  <thead>
    <tr>
      <th>Yazar</th>
      <th>Kaynak</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Taner Saydam</td>
      <td>Udemy - YouTube</td>
    </tr>
    <tr>
      <td>Nursema Gülmez</td>
      <td>Medium</td>
    </tr>
  </tbody>
</table>
