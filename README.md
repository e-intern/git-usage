# GIT KULLANIMI 

Bu dokümanın sadece hatırlatma için eklenmiştir, daha detaylı bilgi ve eğitim serisi için Barış Aslan'ın hazırlamış olduğu   [eğitim serisini buraya tıklayıp](https://www.youtube.com/watch?v=rWG70T7fePg&list=PLPrHLaayVkhnNstGIzQcxxnj6VYvsHBHy) izlemenizi kesinlike tavsiye ederim.
<br/>
<br/>
Ayrıca bu doküman hazırlanırken [Help Github](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax), [Markdown Syntax için](https://daringfireball.net/projects/markdown/syntax) ve [Git Life Cycle (Yaşam Döngüsü) için](https://www.toolsqa.com/git/git-life-cycle) ilgili kaynaklar yalnızca bilgilendirme amaçlı kullanılmıştır.
<br/>
Doküman sonunda oluşturulmuş olan [.gitignore](#gitignore)  için [Git](https://git-scm.com/docs/gitignore) üzerinde ki bilgiler de kullanılmıştır.
<br/>

## Git Nedir?
> Versiyon kontrol sistemidir.

## GitHub - GitLab - BitBucket Nedir?
> Hepsi birer versiyon kontrol sistemi yönetebilmek için üretilmiş ürünlerdir. <br/>
> Aralarında ki farklar sadece ürün kullanım kısıtları ve arayüzleridir.

## Git Nasıl Kurulur?
> Kendi orjinal sitesi olan [Git](https://www.git-scm.com)'e gidip ilgili işletim sistemine ait olan dosyayı indirip kolaylıkla kurabilirsiniz.

## Bilgisayarımda Git Kurulumu?
> İşletim sisteminizden komut penceresine geçiş yapıp
`git --version` ile kurulu ise versiyon bilgisini öğrenebilirsiniz. <br/>
> Kurulu bir işletim sitemi üzerinde örnek çıktı `git version 2.26.0.windows.1` şeklindedir.

## Git Kurulu Bilgisayarlarda
### Git GUI
> Git'i GUI (Graphical User Interface) bir arayüz ile kullanmaya olanak sağlar. 

### Git Bash
> Git'i metinsel arayüz ile kullanmaya olanak sağlar.

### Git Cmd
> Git'i metinsel arayüz ile kullanmaya olanak sağlar.

### Git Bash vs Git Cmd 
> Her ikisi arasında ki temel fark syntax (yazım şeklidir) 'tir.

### Git İle Birlikte Kullanılan Temel Komutlar
`pwd` komutu ile Git komutlarını yazmak için bulunulan dizinin neresi olduğunu öğrenmek için kullanılır. <br/>
`ls` komutu ile bulunulan dizin üzerinde ki dosya ve klasörleri listelemek için kullanılır.  <br/>
`dir` komutu ile bulunulan dizin üzerinde ki dosya ve klasörleri listelemek için kullanılır.  <br/>
`ls -a` komutu ile bulunulan dizin üzerinde ki tüm (gizli dosyalar ve klasörler dahil) dosya ve klasörleri listelemek için kullanılır.  <br/>
`dir -a` komutu ile bulunulan dizin üzerinde ki tüm (gizli dosyalar ve klasörler dahil) dosya ve klasörleri listelemek için kullanılır.  <br/>
`cd` komutu ile klasörler arasında geçiş yapabilmeye olanak sağlar. <br/>
`mkdir` komutu ile mevcut dizin üzerinde klasör oluşturmaya olanak sağlar. <br/>
`cls` komutu ile komut ekranında daha önce yazılmış/getirilmiş kodları ekrandan silmeye olanak sağlar. <br/>
`clear` komutu ile komut ekranında daha önce yazılmış/getirilmiş kodları ekrandan silmeye olanak sağlar. <br/>
`cat >> filename.txt` komut ile bulunulan dizin üzerinde **filename.txt** isimli bir dosya oluşturulup içine bilgi girişi yapmamıza olanak sağlar.  *Not Dosya içerisine bilgi girişini bitirebilmek için `CTRL + C` komutunu kullanılmalıdır.* <br/>
`touch filename.txt` Mevcut dizin üzerine **filename.txt** isimli dosya eklemek için kullanılır. <br/>
`touch filename{2..5}.txt` Mevcut dizin üzerine **filename2.txt, filename3.txt, filename4.txt ve filename.txt** isminde **4** adet dosya oluşturmaya olanak sağlar.

## Sık Kullanılan Git Komutları
`git config --global user.name "kullanıcı adı"` komutu ile ~işletim sistemi~ için *global* olarak **kullanıcı adı**  tanımlamaya olanak sağlar. <br/>

`git config --global user.email "mail@adresiniz.buraya"` komutu ile ~işletim sistemi~ için *global* olarak **mail adresi**  tanımlamaya olanak sağlar. <br/>

`git config --global user.name` komutu ile ~işletim sistemi~ için *global* olarak kayıt edilmiş **kullanıcı adı**  bilgisini gösterir. <br/>

`git config --global user.email` komutu ile ~işletim sistemi~ için *global* olarak kayıt edilmiş **mail adresi**  bilgisini gösterir. <br/>

## **Git Life Cycle (~Yaşam Döngüsü~)**
![Git Life Cycle Görüntülenemiyor](https://raw.githubusercontent.com/umitkarabacak/git-usage/master/Git-LifeCycle.png) 
<br/>


## Git Komutları
<br/>

> *Söz konusu komutlar kullanılırken her zaman için yukarıda ki yaşam döngüsü hatırlanmalıdır. Bu sayede kullanımına daha kısa bir sürede adapte olunacaktır.* <br/>
> _Unutmayın `git status` her zaman sizin yanınzda._


`git init` komutu ile mevcut dizini bir git projesi olarak oluşturmak için kullanılır. <br/>

`git add .` komutu ile git projesi üzerinde ki bütün eklenmiş/düzenlenmiş/silinmiş olan klasör/dosyaları geçiş bölgesine (Staging Area)'ya taşımak için kullanılır. <br/>

`git add filename.txt` komutu ile **filename.txt** dosyası üzerinde yapılmış olan değişiklikler geçiş bölgesine (Staging Area)'ya taşımak için kullanılır. </br>

`git commit -m "commit açıklaması buraya"` komutu ile geçiş bölgesinde bulunan (Staging Area) dosya/klasörleri Git Repository'sine eklemek için kullanılır. *Commit açıklaması ne kadar açıklayıcı olursa o kadar faydalı olacaktır.* <br/>

`git log` komutu ile git projesinin mevcut geçmişi listelenecektir. *Listeleme commit history olarak düşünülebilir.* <br/>

`git status` komutu ile git projesinin mevcut durumu hakkında bilgi alabiliriz, bu komut git projesenin her anında bilgi vermektedir. **Aslında bu komut ile neler yapabileceğimize dair ip uçları bulabiliriz.** <br/>

`git diff` komutu ile git projesi üzerinde ki değişiklikleri toplu bir şekilde görebilmemize olanak sağlar. <br/> 

`git diff filename.txt` komutu ile git projesi üzerinde ki **filename.txt** dosyası üzerinde ki değişiklikleri satır satır görebilmemize olanak sağlar. <br/>

`git diff --staged` komutu ile git repository'si ile geçiş bölgesi (staging area) arasında ki değişiklikleri görebilmemize olanak sağlar. <br/>

`git diff branchName destinationBranchName` komutu ile belirtilmiş olan her iki branch arasında ki farklılıkları görebilmemize olanak sağlar. Genellikle `git diff branchName` şeklinde kullanılır. Bunun bir sebebi ise git projesi üzerinde bir branch üzerinde çalışmak zorunlu olduğu için **destinationBranchName** o anda kullanılan branch olarak kabul edilir. <br/>

`git rm filename.txt` komutu ilg git üzerinden **filename.txt** dosyasını silebilirsiniz. *Bu işlemin bilgisayar kullanımında ki dosya silme işleminden herhangi bir farkı yoktur, fakat git projesi kontrol ediliyorken tamamen GIT komutları kullanılması tavisye edilmektedir.* <br/>

`git rm -r folderName` komutu ilg git üzerinden **folderName** klasörünü ve içerisinde ki tüm dosyaları silebilirsiniz. *Bu işlemin bilgisayar kullanımında ki klasör silme işleminden herhangi bir farkı yoktur, fakat git projesi kontrol ediliyorken tamamen GIT komutları kullanılması tavisye edilmektedir.* <br/>

`git mv eskiDosya.txt yeniDosya.txt` komutu ile **eskiDosya.txt** dosyasının adı **yeniDosya.txt** olarak değiştirilecektir.
_Bu işlem sonrasında `git status` komutu ile durum kontrol edildiği zaman **eskiDosya.txt** dosyası silinmiş, **yeniDosya.txt** dosyası yeniden eklenmiş gibi gözükecektir. Aslında git üzerinde proje takibinde bu anlama gelmektedir. <br/>_

`git mv filename.txt folderName` komutu ile **filename.txt** dosyası **folderName** klasörü altına taşınacaktır. <br/>

`git checkout -- filename.txt` komutu ile **filename.txt** dosyası için geçiş bölgesine (Staging Area)'ya gönderilmemiş haline (`git add .` yapılmamış haline) geri almak için kullanılır. _Unutulmaması gereken bir nokta burda **Staging Area Gönderilmemiş**_ <br/> 

`git checkout commitNumber -- .` git projesi üzerinde **commitNumber** numaralı versiyona geçiş yapmak için kullanılmalıdır. `-- .` _komutu ile projede ki bütün dosyalar için versiyon geçişi olacağı belirtilmektedir._ <br/>

`git checkout commitNumber -- filename.txt` git projesi üzerinde ki **filename.txt** dosyası için **commitNumber** numaralı versiyona geçiş yapmak için kullanılmalıdır <br/>

`git checkout branchName` komutu ile git projesinde ki **branchName** branch'e geçiş yapmak için kullanılır. <br/>

`git reset HEAD filename.txt` komutu ile değiştirilmiş/düzenlenmiş/silinmiş ve geçiş bölgesine (staging area) gönderilmiş (`git add .` komutu çalıştırılmıştır) **filename.txt** dosyasını eski haline geri getirebilmek için kullanılır. <br/>

> [Checkout vs Reset vs Revert](https://stackoverflow.com/questions/8358035/whats-the-difference-between-git-revert-checkout-and-reset) konusuna bir bakmanızı yine tavsiye ederim.

> ![Git Life Cycle Görüntülenemiyor](https://raw.githubusercontent.com/umitkarabacak/git-usage/master/Git-LifeCycle.png) 
<br/>


`git remote add origin https://github.com/umitkarabacak/git-usage` komutu ile mevcut git projesi **origin** takma adıyla **https://github.com/umitkarabacak/git-usage** adresine (git depolama alanına) gönderilmek için kayıt edilmiştir. <br/>

`git remote` komutu ile projenin hangi takma isimle kayıt edildiği bilgisine erişilebilmektedir. <br/>

`git remote get-url origin` komutu ile projenin hangi **origin** takma isminin hangi git repository adresine kayıt edildiği bilgisine erişim sağlanabilir. <br/>

`git remote remove origin` komutu ile projenin git repositoryleriyle olan bütün bilgileri temizlenmektedir. <br/>

`git push -u origin branchName` komutu ile depolanmış **branchName** branch'inde depolanmış **origin** takma ismiyle kayıt edilmiş git repository'sine gönderilecektir. **_Bu işlem ilk defasında yapıldığı zaman kullanıcı adı ve şifre bilgisi isteyebilir_** <br/>

`git pull` komutu ile Git Remote Repository üzerinde ki geçerli branch (üzerinde çalışılan branch) Local Repository üzerine almak için kullanılır. <br/>

`git branch` komutu ile Git Local Repository üzerinde ki branchlerin tamamını listelemeye olanak sağlar. <br/> 

`git branch --all` komutu ile Git Remote Repository üzerinde ki tüm branchlerin tamamını listelemeye olanak sağlar. <br/> 

`git branch branchName` komutu ile Local repository üzerinde **branchName** isimli bir branch oluşturmak için kullanılır. <br/>

`git merge currentBranch destinationBranch` komutu ile **currentBranch**'ını **destinationBranch**'ın üzerine birleştirmek için kullanılır. <br/>

# .gitignore 
`.gitignore` dosyası genellikle `git init` komutu ile birlikte oluşturulmaktadır. Bu dosyanın asıl amacı git projesi üzerinde takip edilmemesini yada özellikle takip edilmesini istediğimiz dosya/klasör ve uzantıları belirtebilmek için kullanılır. 
<br/>
**_Unutulmaması gereken bir hatırlatma .gitignore dosyasının geçerliliğinin olabilmesi için `git commit -m "commit description"` komutundan önce oluşturulması gerekmektedir!_** <br/>

`*` operatörü dizin içerisinde ki bütün dosyaları git projesinin takibinin dışına çıkartmak için kullanılır. <br/>
Örneğin `Notes/*` komutu ile git projesinde ki **Notes** klasörünün içerisinde ki tüm dosyaları git'in takibinden çıkartmak için kullanılır.
<br/>

`!` operatörü haricinde işlem yapmak için kullanılmaktadır. <br/>
Örneğin `!Notes/lifecycle.png` komutu ile git takibi yapılırken `Notes/lifecycle` dosyasının kesinlikle git üzerinde olması gerektiğinin bilgisini vermek için kullanılır.
<br/>

`#` operatörü yorum satırı oluşturabilmek için kullanılmaktadır. <br/>
Örneğin `# .gitignore dosya/klasör takip işlemlerinin konfigürasyonun yapıldığı bir dosyadır.` şeklinde dosya içerisinde hatırlatma yada açıklama yapmak için yorum satırı yazmak için kullanılır.

`[ ]` operatörü _yada_ işlemi için kullanılmaktadır.<br/>
Örneğin `[Bb]in/` komutu ile hem `Bin` klasörü ve altındakileri hemde `bin` klasörü ve altındakileri git projesine dahil etmeyecektir.
