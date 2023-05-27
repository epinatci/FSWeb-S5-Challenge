# Uygulamalı JavaScript Sprint Mücadelesi

**Bu talimatları dikkatlice okuyun. Bu Sprint Mücadelesine başlamadan önce tam olarak ne beklendiğini anlayın.**

Bu mücadele, geçmiş sprint boyunca öğrenilen kavramları ve teknikleri uygulamanıza ve bunları somut bir projede kullanmanıza olanak tanır. Bu sprint sayesinde **Uygulamalı JavaScript** 'i keşfettiniz. Bu sprint boyunca **DOM ve bileşenler**'i öğrendiniz. Bu mücadelede, **çevrimiçi bir Teknoloji Gazetesi** oluşturarak bu becerilerdeki ustalığınızı göstereceksiniz.

Bu projeyi, herkesin kendisinin yapması beklenmektedir. Tüm iş size ait olmalıdır. Mücadele puanınız, bu sprint boyunca işlenen materyali kullanarak bağımsız çalışma yeteneğinizin bir ölçüsüdür. Önceki Sprint'te tanıtılan ve uygulanan kavram ve hedeflerde yeterlilik göstermeniz gerekir.

Bu sprint mücadelesi sırasında işbirliği yapmanıza izin verilmez.

### Proje Kurulumu

* [ ] Bu projenyi forklayarak bir kopyasını oluşturun.
* [ ] Reponun kendi versiyonunuzu klonlayın.
* [ ] Commitinizi pushlayın: `git push origin main`.

## Proje Açıklaması

### Giriş

Bir teknoloji gazetesi oluşturacaksınız. İşiniz, gazetenin ana sayfasını oluşturan bileşenleri oluşturmak olacak..

Aşağıda listelenen minimum uygulanabilir ürün (MVP) spesifikasyonlarını karşılayan projeniz, aşağıda bağlantısı verilen görüntüye benzer görünmelidir.:

[Teknoloji Zamanı](/tasarım.png)

### Detaylar

- [ ] Komut satırınızla projenin kök dizinine gidin.
- [ ] `package.json` dosyasında listelenen bağımlılıkları indirmek için `npm install` komutunu çalıştırın.
- [ ] Projeyi derlemek ve sunmak için `npm start` komutunu çalıştırın.
- [ ] Chrome'da `http://localhost:3000` konumuna gidin
- [ ] Testleri çalıştırmak için ayrı bir terminalde `npm test` komutunu yazın.

**MVP için adımlar:**

- [ ] Adım 1 ve 2 `src/bileşenler/header.js` dosyasında açıklandı.
- [ ] Adım 3 ve 4 `src/bileşenler/tabs.js` dosyasında açıklandı.
- [ ] Adım 5 ve 6 `src/bileşenler/card.js` dosyasında açıklandı.

**Önemli Notlar:**

- Lütfen **dosyaları ya da klasörleri taşımayın ve isimlerini değiştirmeyin** .
- Geliştirme sunucunuz "otomatik yeniden yüklemeyi" durdurursa, `CTRL+C` ile manuel olarak sonlandırın ve yeniden başlatın.
- `package.json` 'ı değiştirmeyin, sadece NPM ile dosyaları indirin (Axios _halihazırda_ `package.json` 'a eklendi).
- Çözümünüzde en iyi uygulamaları izlemeniz, temiz ve profesyonel sonuçlar üretmeniz önemlidir.
- Yazım denetimi ve dilbilgisi denetimi de dahil olmak üzere çalışmanızı gözden geçirmek, iyileştirmek için zaman planlayın.
- MVP'yi karşılayan bir meydan okuma göndermek, çok fazla detayla uğraşılıp da çalışmayan bir kod göndermekten daha iyidir.


## Ek Sorular

Aşağıdaki soruları yanıtlayarak bu sprint'in kavramlarını anladığınızı gösterin. Her sorudan sonra yanıtlarınızı eklemek için bu belgeyi düzenleyin.

1. DOM nedir?
DOM (Document Object Module) HTML dökümanları içerisinde bulunan nesnelere kolaylıkla erişim sağlamak ve üzerinde işlemler yapabilmek için tasarlanan bir modeldir. DOM ile HTML dosyamızda bulunan her şeye erişim sağlayabilirsiniz.

2. Bir event nedir?
Olay (Event) arabirimi, DOM'da gerçekleşen herhangi bir olayı temsil eder; Bazıları kullanıcı tarafından üretilen (mouse veya klavye etkinlikleri gibi) diğerleri ise API'lar tarafından üretilir (bir animasyonun çalışıp çalışmadığını, videolar duraklatıldığını gösteren etkinlikler gibi). Birçok olay türü vardır, bunların bazıları ana Olay arayüzüne dayalı diğer arayüzleri kullanır. Olayın kendisi, tüm olaylarda ortak olan özellikleri ve methodları içerir.

3. Bir event dinleyici(listener) nedir?
Bazen bir web sayfası oluştururken, biri web sitenizde belirli bir etkinlik türünü tetiklediğinde bir kod parçası yürütmek isteyebilirsiniz.
Javascript addEventListener methodu ile bunu hızlı ve kolay bir şekilde yapabilirsiniz.
addEventListener() methodu, belirtilen öğeye bir olay işleyicisini ekler. Bu olay meydana geldiğinde, dinleyici fonksiyon yürütülür. Bu method bir değer döndürmez.

4. Neden bir NodeList'i Array'e dönüştürelim??
JavaScript'te bir NodeList'i Array'e dönüştürmenin birkaç nedeni vardır. İşte bazıları:

Daha fazla dizi yöntemine erişim: NodeList, Array'in bir alt kümesidir ve yalnızca NodeList'e özgü yöntemlere sahiptir. Bunlar, forEach, map, filter, ve reduce gibi kullanışlı dizi yöntemlerini içermez. Eğer bu dizi yöntemlerini kullanmak isterseniz, NodeList'i Array'e dönüştürerek bu yöntemlere erişebilirsiniz.

Genel olarak daha fazla esneklik: Array'ler, dinamik boyutlara sahip olabilirken NodeList'ler sabit bir boyuta sahiptir. NodeList'i Array'e dönüştürerek, elemanları ekleyebilir, çıkarabilir veya değiştirebilirsiniz.

Tarayıcı uyumluluğu: NodeList, bazı tarayıcılarda ve eski tarayıcı sürümlerinde kullanılan bir türdür. Bazı durumlarda, NodeList'i Array'e dönüştürerek tarayıcı uyumluluğunu artırabilirsiniz.

5. Bileşen nedir?
Web Bileşenleri, yeniden kullanılabilir özel öğeler oluşturmanıza olanak tanıyan farklı teknolojilerden oluşan bir pakettir ( işlevleri kodunuzun geri kalanından uzakta kapsüllenerek ) ve bunları web uygulamalarınızda kullanın.