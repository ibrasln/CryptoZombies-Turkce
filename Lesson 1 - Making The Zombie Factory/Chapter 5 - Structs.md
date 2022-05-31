# Bölüm 5: Struct'lar

Bazen karmaşık bir veri tipine ihtiyaç duyarız. Bunun için, Solidity bize _struct_'ları sağlar. Struct'lar, birden çok özelliğe sahip daha karmaşık veri türleri oluşturmanıza olanak tanır.

    struct person {
      uint age;
      string name;
    }
    
> NOT: Yukarıdaki kodda _string_ isimli yeni bir tip belirttik. String'ler rastgele uzunluktaki UTF-8 verileri için kullanılır. Örneğin:
    
    string greeting = "Hello World!";
    
## Uygulama

Uygulamamızda birden fazla zombi yaratmak isteyeceğiz ve zombilerimizin özellikleri farklı olacaktır. Bu nedenle bizden zombiler için bir struct oluşturmamız isteniyor.

1. Zombie isimli bir struct oluştur.
2. Zombie struct'ı 2 özelliğe sahip olsun: _name_ (string), _dna_ (uint)

       pragma solidity >=0.5.0 <0.6.0;
       
       contract ZombieFactory {
        uint dnaDigits = 16;
        uint dnaModulus = 10 ** dnaDigits;
        
        struct Zombie {
          string name;
          uint dna;
        }
       }
