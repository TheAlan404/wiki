# Github Nedir? Nasıl Kullanılır?

Github, genelde yazılımcıların kullandığı bir "sürüm kontrol" sitesi - **git** diye bir sistem kullanıyorlar ve en çok github'da kullanıyorlar.

Aşağıdaki pratiği deneyin ve bence neden bu kadar çok kullanıldığını siz de anlarsınız.

## Pratik

Öğrenmeniz için biraz pratik yapalım:

### 1. Github hesabın yoksa oluştur

   [Buradan](https://github.com/signup) oluşturabilirsin. Eposta şifre vb.

### 2. Repo oluştur

    Sağ üst köşedeki (`+`) -> `New Repository` butonuna tıkla

   ![image](https://user-images.githubusercontent.com/43997085/247526767-6452fdf5-ee5a-4e9e-ae56-77cd259b8b97.png)

   Çıkan sayfadan reponun ismini, açıklamasını, görünürlüğünü, vb. ayarlayabilirsin.

   - Bunları daha sonra değiştirebilirsin
   - **Add README** ayarı senin için README.md oluşturur, onu tikle.
   - **Add .gitignore** ve **Choose a liscense**'ı şimdilik atlayabilirsin.
   - Ayarladıktan sonra aşağıdaki **[Create Repository]** butonuna tıkla.

   ![image](https://user-images.githubusercontent.com/43997085/247527187-8e7ab7ff-3550-426a-8958-d63fee8dccde.png)

### 3. git'i kur

   Tabikide git'i de kurman gerekiyor. Hemen sana [direkt indirme linki](https://github.com/git-for-windows/git/releases/download/v2.41.0.windows.1/Git-2.41.0-64-bit.exe) vereyim :3 (windows 64 bit)

   Çoğu ayarı pes geçebilirsin, varsayılanlar iyi - ama editüru görürsen değiştirirsen iyi olur.

### 4. Repo'yu klonla

   Git'i kurduktan sonra repo'yu kendi bilgisayarımıza klonlamamız gerekiyor.

   Reponun klonlanacağı yeri seçin, örneğin masaüstünüze 'repolarım' diye bir klasör açabilirsiniz.

   Normalde buraya [komut istemi](./cmd.md) ile `git clone` komutunu açıklayacaktım, ama daha kolay olsun diye silip baştan yazıyorum:

   [vscode](https://code.visualstudio.com/) kurun! Başlayanlar için daha pratik çünkü git ve github'a entegrasyonu var.

   Kurduktan sonra Welcome kısmından **Clone Git Repository**'e basın. Github hesabınızı vscode bağlanacak vb. vb. - Github'dan kendi reponuzu bulun ve seçin. Açılan dosya gezgini penceresinden ise 'repolarım' diye oluşturduğumuz klasörü seçin (git, seçtiğniz klasörde repo için bir klasör açıp onun içine klonlayacak zaten.)

   Klonlandıktan sonra aç/open butonu ile vscode'dan repoyu açabilirsiniz.

### 5. README.md'yi değiştir

   README.md özel bir dosya - github'da reponun dosyalarının altındaki bütün yazılar o dosyanın içindeki yazılardan oluşuyor. `.md` ise Markdown dosya formatı. Discord mesajlarına çok benziyor - sadece biraz daha formatlama var.

   Bizim bu alıştırmamız için README'ye istediğin ne varsa yaz. Şimdilik minecraft sunucunun kurallarını yazıyormuş gibi birşeyler yaz.

### 6. Commit oluştur
  
   vscode'da, sol kısımdaki ikonlardan üçüncüsüne tıklayıp **Source Control** kısmına gel.

   Burada hangi dosyaları değiştirdiğini sana göstericektir. (ekleme, oluşturma, silme)

   Bir commit mesajı yaz ve Commit butonuna bas. Bu bütün değişikliklerini bir commit olarak paketlicektir.

   Sana 'staged changes' ile ilgili birşeyler derse şöyle anla: ilk önce commit'ine ne ekleyeceğini seçmeni istiyor (staging) - ama vscode 'bütün hepsini commitliyeceğim' diye bir buton sunuyor diyalogda. Eğer manuel olarak eklemek istersen (`+`) ve (`-`) butonlarını kullanabilirsin.

### 7. Değişikliklerini (commitler) gönder

   Commit oluşturduktan sonra Github'a yeniden göndermek için 'Sync Changes'e bas.

   - **Pull** => Uzaktan (github) commitleri çekmek
   - **Push** => Kendi atmadığımız commitleri uzağa (github) yüklemek
   - **Sync** => Pull + Push

   Yaptığın değişiklikler github reponun sayfasında gözükmeli. (bir refresh atman gerekebilir)

### 8. Ekstra: Branchler

   Branchler aynı anda birkaç şeyi değiştirmene yardımcı olan bir sistem. Her değişiklik bir commit olduğundan böyle bir grafik oluşturabiliriz:

   ![git](https://blogs.halodoc.io/content/images/2022/05/branch3.png)

   Mavi noktalar 'main' yani ana branch'e ait diye düşünelim. Mor ise bir arkadaşının branch'i olsun.

   Sen main'de değişiklikler yaparken (örn. sunucu kuralları yazılarını değiştirirken) aynı anda arkadaşın farklı birşeyleri değiştirebilir (örn. sunucu logoları vb.)

   Daha sonra ise bu branch'ler birbirine yeniden birleşebiliyor! (Merging)

### 9. Ekstra: Fork & PR

   Eğer github repo'n public (herkese) ise diğer kişiler repo'nu **Fork**'layabilir. Forkladıklarında kendi hesaplarında bir branch açmışlar gibi düşünebilirsin. Forklanan repo orjinal repoya bağlıdır ve orjinal repodaki yeni commitleri forklanan repoya merge yapabilirsin.

   Mesela bir başkasının artık bakmadığı bir projesini forklayıp kendi forkladığın repodan devam edebilirsin.

   Ve, forklanan repodaki commitleri **Pull Request (PR)** ile orjinal repo'ya birleştirme isteğinde bulunabilirsin.

   Pratik yapmak istiyorsan, bir arkadaş bul - eğer git/github kullanmayı bilmiyorsa ona bu dökümanı at, ama **2. adımda repo oluşturması yerine senin repo'nu forklamasını söyle**

   Fork butonu burada:

   [image](https://user-images.githubusercontent.com/43997085/247549248-883c91c9-08c8-4239-a51c-483ed6dcfaae.png)

   Arkadaşın forklayıp, yazığın listeye yeni bir kural ekleyebilir örnek olarak. Daha sonra yaptığı commitleri kendi repo'na ekleyebilmek için arkadaşının açacağı Pull Request'i kabul edebilirsin.
