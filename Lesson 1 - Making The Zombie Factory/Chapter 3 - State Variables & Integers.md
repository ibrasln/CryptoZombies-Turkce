## Bölüm 3: Durum Değişkenleri ve Integer'lar

Harika! Kontratımızın iskeletini oluşturduğumuza göre şimdi sıra kontrat içerisinde kullanılabilir değişkenleri inceleyelim.

Durum değişkenleri, kontrat deposunda kalıcı olarak saklanır. Yani Ethereum blokzincirine yazıldıkları anlamına gelir. Bunları bir DB'ye yazmak gibi düşünebilirsiniz.
Örneğin:

    contract Example {
      // Aşağıdaki değişken blokzincirinde kalıcı olarak depolanacaktır.
      uint myUnsignedInteger = 100;
    }
    
## Unsigned Integers: *uint*

uint veri türü işaretsiz bir tamsayıdır, yani değeri negatif olamaz. Ayrıca işaretli tamsayılar için bir int veri türü vardır.

>NOT: Solidity'de uint, aslında 256 bitlik işaretsiz bir tamsayı olan uint256 için bir takma addır. uint'leri daha az bit ile bildirebilirsiniz - uint8, uin16, uint32 vb. Ama genel olarak, daha sonraki derslerde bahsedeceğimiz belirli durumlar dışında uint'i kullanmak isteyeceksiniz.

## Uygulama

Zombi DNA'mızın 16 haneli olacağını söylemiştik. Bizden _dnaDigits_ isminde bir _uint_ değişken oluşturmamız ve bunu 16ya eşitlememiz isteniyor.

    pragma solidity >=0.5.0 <0.6.0;
    
    contract ZombieFactory {
      uint dnaDigits = 16;
    }
