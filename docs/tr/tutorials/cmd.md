# CMD nasıl açarım?

Komut istemi, ya da cmd.exe ile bilinen programı, yani konsolu, birkaç şekilde açabilirsin.

**Not:** Komut isteminin bulunduğu klasöre her zaman dikkat et! Yazdığın her komut, bulunduğun klasöre göre çalışır. System32'de komut yazmak istediğini sanmıyorum.

1. **Yöntem** - en kolayı

   Windows Explorer (dosya gezgini) 'den *bulunduğun yol konumunun* kutucuğuna tıkla, herşeyi otomatik seçmiş olmalısın:

   ![image](https://user-images.githubusercontent.com/43997085/247529457-f4414c40-66de-48c1-a042-c81416b767fc.png)

   O kutuya **`cmd`** yazıp entera basarsan bulunduğun klasörde cmd açılmalı!

   ![image](https://user-images.githubusercontent.com/43997085/247529791-757c90db-db07-4f0c-84ab-8a500d25195f.png)

2. **Yöntem**

   Windows ikonuna sağ tıklarsan (kısayol olarak `Win`+`X` bu arada) orda 'Komut istemi' ya da 'Powershell'i görebilirsin.

   Powershell biraz daha yavaş ve fazla uzmanca olduğundan cmd'yi tercih ediyoruz. Powershell içine `cmd` yazarsan cmdyi powershell içinde çalıştırabilirsin (kötü bir şekilde).

   Ya da 3. yöntem gibi Powershell içinde `start cmd; exit` yazabilirsin - `start cmd` yeni pencerede cmd açar ve `exit` powershell'i kapatır

   **Not:** böyle yaparsanız cmd kötü klasörlerde açılabilir, alttaki kısmı okuyun.

3. **Yöntem** - en bilindik ama pratik olmayan

   Bu yöntem ise 'Çalıştır' kutusunu kullanır: `Win`+`R` kısayolu ya da Win ikonuna sağ tık ve 'Çalıştır'

   Çalıştır kutusuna yazdığın şey zaten `start` komutu gibi olduğundan oraya `cmd` yazarsan cmd açılır.

   **Not:** böyle yaparsanız cmd kötü klasörlerde açılabilir, alttaki kısmı okuyun.

## CMD'de Navigasyon

> [⬅️ İçindekiler](#daha-iyi-yöntemi-var)

![image](https://user-images.githubusercontent.com/43997085/247531103-eb718aee-3909-42c9-b6df-8367750ddead.png)

Gördüğünüz gibi bu cmd'nin konumu şu an `C:/Users/dennis`...

Bu komutları kullanarak istediğiniz klasöre gidebilirsiniz:

- `cd ..` => Bir önceki klasöre git
- `cd klasor` => klasor'e gir
- `cd C:\Users\dennis\Desktop\bin` => o uzun yoldaki bin klasörüne gir

Klasör her zaman yazdığınız yerin solunda, `>`'dan önce yazıcaktır.

- `dir` => bu komut ile klasördeki dosyaları listeleyebilirsiniz
- `explorer .` => bu komut ile dosya gezginini bulunduğun klasörde açabilirsin

Relativite:

- `.` => Bulunduğun klasör
- `..` => Bir önceki klasör
- Bunlar üst üste kullanılabilir: `../../../hello.txt` => çok geride bir dosya
