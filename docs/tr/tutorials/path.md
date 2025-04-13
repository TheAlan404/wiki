# PATH

[Komut istemi](#cmd-nasıl-açarım)nde herhangi bir komut yazarsanız aslında o komut bir `.exe` dosyasını çalıştırır (bazı özel komutlar dışında). Örneğin, `java` yazarsanız komut istemi `java.exe`'yi çalıştırır.

Ama bu `.exe` programlarını komut istemi nasıl buluyor? Cevap `PATH` değişkeni.

Cmd'ye `path` komutunu yazarsanız size path değişkeninizi gösterir. Fark ederseniz aslında `;` ile ayrılmış bir dosya yolları listesi. Cmd'de bir komut yazınca cmd teker teker her dosya yolunda yazdığınız komuttaki `.exe` dosyasını arar ve ilk bulduğunu çalıştırır.

**Peki nasıl birşeyi path'e ekleyebilirim?**

2 yolu var:

- **1. Yol** (önerilen)
  1. `C:/bin` diye bir klasör oluşturun.
  2. Sistem ayarlarından ortam değişkenlerinden path değişkeninin sonuna `;C:\bin` ekleyin

     ![a](https://www.teknoloskop.net/wp-content/uploads/2019/02/Screenshot_56.png.webp)

     ![a](https://www.teknoloskop.net/wp-content/uploads/2019/02/Screenshot_57.png)

     ![a](https://www.teknoloskop.net/wp-content/uploads/2019/02/Screenshot_58.png)

     ![a](https://www.teknoloskop.net/wp-content/uploads/2019/02/Screenshot_60.png)

     **Not:** `C:\bin` klasörü olması zorunlu değil - ben kolay erişilebiliyor diye öyle öneriyorum. Eğer (örneğin) düzgün eklenmemiş ise Program Files/BirProgram gibi birşeyi de ekleyebilirsiniz. (başka durumlarda)

     **Not:** Path'in değişmesini açık olan işlemler pek anlayamadığından açık olan cmd'leri yeniden başlatmanız gerekebilir. Windows'u yeniden başlatırsanız herşeyin yeni path'i görmesi garantidir.

  3. Eklemek istediğini o klasöre at

- **2. Yol**
  1. Path'de var olan bir klasöre git
  2. Eklemek istediğini o klasöre at

     Bu biraz daha kaotik ve düzensiz ama işe yarar.

**Dipnot:** Cmd, kısayolları da okur. Yani `C:\bin` path'de ise ve o klasöre bir kısayol koyarsanız o kısayolu da kullanabilirsiniz.
