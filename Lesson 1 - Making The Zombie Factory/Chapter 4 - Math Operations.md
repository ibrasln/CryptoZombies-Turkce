# Bölüm 4: Matematiksel Operatörler

Solidity'de matematik oldukça basittir. Aşağıdaki işlemler çoğu programlama dilindeki ile aynıdır:

- Toplama: x + y
- Çıkarma: x - y
- Çarpma: x * y
- Bölme: x / y
- Modül(Kalan): x % y (Örneğin, 25 % 7 = 4'tür. Çünk 25'i 7'ye bölerseniz kalan 4'tür)

Solidity ayrıca üstel işlemi de destekler. (yani 'x üzeri y'):

    uint x = 5 ** 2; // eşittir 5^2  = 25
    
    
## Uygulama

Zombimizin DNA'sının sadece 16 karakter olduğundan emin olmak için _dnaModulus_ adında _10^16_'ya eşit olacak bir uint değişken oluşturmamız isteniyor.
**16 basamağını kısaltmak için % operatörünü kullanabiliriz.**
 
 _dnaModulus_ isimli uint değişkeni 10 üssü _dnaDigits_'e eşitleyelim.
 
    pragma solidity >=0.5.0 <0.6.0;
    
    contract ZombieFactory {
      uint dnaDigits = 16;
      
      uint dnaModulus = 10 ** dnaDigits;
    }
