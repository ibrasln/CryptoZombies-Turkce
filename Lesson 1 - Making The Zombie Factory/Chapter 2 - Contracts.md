## Bölüm 2: Kontratlar

Temellerle başlayalım:

Solidity kodu kontratlarda yer alır. Bir kontrat, Ethereum uygulamalarının temel yapı taşıdır - tüm değişkenler ve fonksiyonlar bir kontrata aittir ve bu tüm projelerinizin başlangıç noktası olacaktır.

*HelloWorld* isimli boş bir kontrat şu şekilde gözükür:

    contract HelloWorld {

    }

## Pragma Versiyon

Her Solidity kaynak kodu sürüm bilgisi ile başlamak zorundadır. Bu sayede derleyicinin hangi sürümde kullanılacağı belli olur. Bu, kodunuzu bozabilecek değişiklikler getiren ilerideki Solidity sürümleriyle ilgili sorunları önlemek için alınan bir önlemdir.

>Bizler sürümü 0.5.0 (dahil) ile 0.6.0 (hariç) aralığındaki herhangi bir derleyici sürümüyle derleyebiliceğimizi belirttik.

    pragma solidity >=0.5.0 <0.6.0;
 
Kısacası her projeye başlamadan önce yazacağınız ilk şey şu olacaktır:
        
    pragma solidity >=0.5.0 <0.6.0;
    
    contract HelloWorld {
    
    }
    
##Uygulama

Zombi ordumuzu yaratmaya başlamak için ZombieFactory isimli bir ana kontrat oluşturmamız isteniyor.

    pragma solidity >=0.5.0 <0.6.0;
    
    contract ZombieFactory {
    
    }
    
İşlemi bitirdiğiniz zaman aşağıdaki **Check Answer** butonuna tıklayınız. Eğer zor durumda kalırsanız, **Hint** butonuna tıklayabilirsiniz.
