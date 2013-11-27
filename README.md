Whianex Css Sınıfları
==========

Whianex sistemi içerisinde kendi has bir css sınıf yapılanması içermektedir. Ana nesnelere prefix koyarak alt özelliklerini belirleyebileceğiniz bu sınıf yapılanması aynı zamanda tek düzenlemeyi birden çok nesneden kullanmanıza olanak sağlamaktadır.

[ Sınıf Tipi ] [ Ana Nese Adı ] [ Ana Nesne Adının İlk 3 Harfi - Nesne Alt Özellik ] [ Ana Nesne Adının İlk 3 Harfi - Nesne Alt Özellik ... ]

Örnek ;

.button but-blue -> [ Sınıf Tipi = . ] [ Ana Nesne Adı = button ] [ Nesne Alt Özellik = blue ]

Örnek 2 ;

.but but-blue but-large 

Mümkün olduğunca core dosyalara müdahale edilmemesi gerekir. Yeni bir yapı oluşturmak için ana sınıfa altında alt özellik ekleyebilirsiniz. Örneğin sarı renkli bir buton eklemek için ;

.but but-yellow{
  background : yellow !important;
}

Yeni tanımlayacağınız alt özelliklerin tam anlamıyla çalışabilmesi, sorun çıkarmaması için " !important " deyimini kullanmanızı öneririz. Başka bir örnekle devam edelim, şimdi de butonun sağ sol padding oranlarını arttırmak istiyoruz fakat böyle bir sınıf henüz mevcut değil, öyleyse hemen ana sınıfımızı alıp yeni bir alt özellik ekliyoruz ;

.but but-paddingLeft10{
  padding-left: 10px;
}

şeklinde tanımlanabilir.

Bu sınıfları nesnelere atarken ;

<a href="#" class="button but-blue">Button</a>

Şeklinde tanımlanabilir. Sınıf yapılarının amacı kullanımı kolaylaştırmak ve aynı zamanda sistemde kod fazlalığını atmak olacağı için id ile işlemlerinini mümkün oldukça az tutmanızı öneririz.

... Css işlemi bittikçe eklenecektir.
