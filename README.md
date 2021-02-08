[![](https://repository-images.githubusercontent.com/53238813/4038c700-61d2-11e9-805e-2d39adbf13ca)]()
# HomeBrew Nedir?
Mac OSX isletim sistemi uzerinde yazilim kurulumunun kolaylastiran bir paket yoneticisidir. Hem ucretsiz, hem de acik kaynakli bir yazilim paketidir. Ornek olarak mac'inize mongodb,redis,git kurmak mi istiyorsunuz? bunu homebrew ile terminal ekranina belli basli kodlar yazaraktan hizli bir kurulum gerceklestirebilirsiniz. 

>Homebrew ayrica Apple'in ihtitaca duymadigi ama size lazim olan paketleride kendi icerisinde indirir. Ornek vericek olursam mac'im de, jmeter kullanarak load test yaparken cokmus ve mac'i bastan yapilandirmam gerekmisti ve herseyi mac'e bastan kurdum. Kurulum islemlerinde sira git'e geldiginde, git yukleme asamasinda bir cok problem cikardi, cikan sorunnlari cozdukce bir baskasi cikti ve burada imdadima homebrew yetisti.

Homebrew haricinde benzer iki paket yoneticisi de bulunmakta fink ve macports adi altinda, ben kullanmadim ama zamaniniz varsa denenebilir. 

## Nasil Kurulur? 
Terminal ekraniniziz acin ve asagida ki komutu yapistirin.
```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
### Kurulumu test etmek icin komutunu calistirin
```sh
brew -v
```

### Brew Komutu
Brew komutunu calistirdiginizda size homebrew ile neler yapabileceginizi ozetleyen bir liste ile karsilasirsiniz
```sh
brew
```

### Ornek olarak Bir uygulamayi Homebrew'da aramak
Diyelim ki postman'i homebrew ile kurmak istiyoruz diyelim ama oncelikle formula'si (formula kavramini birazdan deginicem) var mi yok mu bilmiyioruz once search etmemiz gerekiyor 

```sh
brew search postman
```
veya 
```sh
brew search redis
```

### Uygulamayi indirmek icin
>Search olarak 
```sh
brew install postman
```

### Formula kavrami Nedir Peki? 

Formula aslinda sizin indirmek istediginiz uygulamaya verilen isim bir alias aslinda yani.Formulalar ruby dili ile yaziliyor, kaynak kodunuzu nereden indirilecegi, indirildikten sonra nasil kurulacagi ve kurulduktan sonra basarili bir sekilde kurulup kurulmadigi testini yapan mini uygulama gibi dusunebilirsiniz aslinda bir container.

> sizde bir custom formula yazip homebrew'e koyabilirsiniz. 

```sh
brew install <formula>
```
Sevgiler Saygilar...
