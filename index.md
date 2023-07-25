# Master1
Aciklama yaoildi
Burada bir paragraf vardir
Burada bir paragraf vardir
Burada bir paragraf vardir
Burada bir paragraf vardir
Burada bir paragraf vardir

git init -> igt dosyasi olusturuldu
git status
git log -> commit gecmisi
cd .. -> bir ust dizine cikma
ls -> osya iscerigi goruntuleme
-> commit atma 1<-
git add index.md 
git commit -m "Master2 | add content" 
-> commit atma 2 <-
git add .
git commit -m "Master2 | add content" 
-> bir onceki commit mesajini guncelleme kodu da gunceller <-
git add .
git commit --amend

-> bir onceki sadece commit mesaji guncellem <-
git commit --amend -m "bu amend ile eklenmis bir mesajdir"
 -> commit silme<- hash id yi kullanarak silcez
 git revert commit <hash id>
  -> commit silme idsiz<-
git log -n 1 ->  sondan 1. commiti getir
git log -n 2 ->  sondan 1. ve 2. commiti getir
git log -n 2 ->  sondan 1. 2. ve 3. commiti getir
revert i revert edebiliyoruuz

git reset --hard -> bunu dikkatli kullan

commitler arasindaki farkliliklari getir
git diff  <hash id1>.. <hash id2> index.md 1 den 2 ye kadar olan farklari getirir

<- branch acma->
git branch <-var olan branchlari olusturur->
git branch header <- header isimli bir branch acar -> ama hala masterda oldugumuzu soyler
 <-headera gecme->
git checkout header
<- branch olustrup direkt gecis yapma->
git checkout -b footer
<-branch silme->
 
 <-gıt stash son comitten itibaren yaptığınız tüm değişiklikler saklan->
 saklanan veri ne bir committir ne de kayıt sadece depo
 git stash
 git log
 git stash clear -> temizler
 git stash pop en üstteki kaydı geri getirir
 <<<MERGE>>>
<-git merge squash -> merge işleminde son bir commit fırsatı verir
<-git rebase-> birleşimleri direkt mastera çakar  sanki birleşim yokmuş vibeı verir. son bir coomit attırmaz