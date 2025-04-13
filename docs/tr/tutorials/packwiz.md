## Packwiz ile daha kolay Modpack oluşturmak

Gördüğüm kadarıyla bazılarınız Packwiz nedir bilmiyor. Ya da mrpack dosyaları. Direkt modların jar dosyalarını zipleyip discorddan vs. paylaşıyor...

Bu tam bir güvenlik sorunu değil mi? Ya bir mod virüs ise?

Aynı zamanda çok fazla mod var ise dosya da çok büyük oluyor. Kendinize bu işkenceyi yapmayın.

**Packwiz** minecraft modpacklerini paylaşmanızı sağlayan bir araç. Çalışma prensibi kolay. Ama [Prism Launcher](https://prismlauncher.org/) gibi bir MultiMC launcheri kullanırsan - bence kullanmayan çok şey kaçırıyor.

> bkz. [packwiz dokümentasyon](https://packwiz.infra.link/)
> bkz. [packwiz repo](https://github.com/packwiz/packwiz)
> (aşağıda kurulumu yazıyor)
> bkz. [prism launcher cracked](https://github.com/Diegiwg/PrismLauncher-Cracked/releases) (Windows-MSVC-Setup)

1. Oyuncular `.mrpack`/vb dosyasını indiriyor

2. Bu dosyayı herhangi MultiMC/Prism Launcher launcherindan o dosyayı açıyor

3. Launcher kendisi kuruyor .minecraft klasörünü vb.

4. Oyunu her açtığınızda minecraft'ın jar dosyasından önce `packwiz-bootstrap.jar` diye birşey çalışıyor. Bunun tek amacı **packwiz modpackinin** güncel olup olmadığını sorması.
   - Eğer gerekli modlar yoksa kendisi indirip kuruyor
   - Eğer opsiyonel modlar var ise, onları da sana seçme özelliği ile sunuyor
   - Aynı zamanda gerekli diğer dosyaları da koyuyor
   - Bu modlar ve dosyaların hepsi *modpackin* belirlendiği yerden belirleniyor

5. Packwiz-bootstrap çalıştıktan ve herşeyin güncel olduğundan emin olduktan sonra ise normal oyunu çalıştırıyor.

Yani evet, otomatik yükleme ve güncelleme. Neden kullanmıyorsunuz?!

### Packwiz kurulumu

Packwiz'i kullanabilmek için indirmeniz ve path'e eklemeniz gerekiyor.

- İndirmek için [buraya girin](https://github.com/packwiz/packwiz/actions/workflows/go.yml)
  1. Listenin başındakine tıklayın
  2. Sayfanın altından **Artifacts**'den windows'u indirin

     ![image](https://user-images.githubusercontent.com/43997085/247555401-1587d626-fbc3-444b-bc0b-0a4b4d07581e.png)

     **Not:** Bu bir kurucu değil - direk `.exe` bunu cmd'de çalıştıracaksınız.
- Diğer gereksinimler için bakınız:
  - [Path - ne bu? ne işe yarıyo? nasıl eklicem?](#path)

### Packwiz ile modpack oluşturma örneği

örnek olarak bu modpacklere bakabilirsiniz:

- [Modrinth SMP](https://github.com/modrinth-smp/pack)
- [lctr-modpack](https://github.com/TheAlan404/lctr-modpack) (ben yaptım!)
- [packwiz example pack](https://github.com/packwiz/packwiz-example-pack)

Şimdilik [bu linkteki](https://packwiz.infra.link/tutorials/creating/getting-started/) ingilizce tutorial'ı takip edin, daha sonra buraya türkçesini yazıcağım. Ama ondan önce [github nasıl kullanılır](#github-nedir-nasıl-kullanılır) kısmını okumanızı öneriyorum çünkü örnek verdiğim 3 modpack de github'u kullanıyor.
