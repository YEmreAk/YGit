---
description: Yeni başlayanlar için Git (Versiyon Kontrol Sistemi) kitabı
---

# 📕 Türkçe Git 101

## 🗽 Ufak Bilgiler

- ❗ Bu içerik [YEmreAk.com](https://yemreak.com)'a ait değildir.
- Projenin aslına [git101_book](https://github.com/aliozgur/git101_book) bağlantısından erişebilirsin.
- [**Kitabın basılı halini online olarak da satın alabilirsiniz**](https://www.dikeyeksen.com/products/git-ile-versiyon-kontrolu)

> GitHub üzerinde **ücretsiz** olarak sunulduğu için sitemde (kendimce) daha güzel ve indekslenebilir bir yapıya çevirerek sunum hizmeti vermekteyim.

## Önsöz

---

Bu kitapta son 4-5 yılda yazılım geliştiricilerin ve yazılım şirketlerinin vazgeçilmez araçlarından biri olan ve benim de bir yazılım geliştirici olarak çok başarılı bulduğum Git Dağıtık Versiyon Kontrol Sistemini \(Distributed Version Control System\) örnekler ile ele alarak size tanıtmaya çalışacağım.

İster kıdemli bir yazılım geliştirici olun isterseniz yazılım geliştirme işine yeni başlayan bir profesyonel iş görüşmelerinde temel bilgisayar bilimleri, programlama dilleri ve veri tabanları ile ilgili sorulardan sonra ilk 5 soru içinde yer alacak konulardan birisi de Git olacaktır. Özellikle 2009 yılı itibariyle bulut tabanlı bir sistem olarak kullanıma açılan GitHub’ın yıllar içindeki yükselişi ile birlikte GitHub profiliniz, GitHub’da takip ettiğiniz ve katkı yaptığınız projeler işverenler açısından sizinle ilgili önemli ipuçları sağlayan bir bilgi olarak değerlendirilmektedir.

Versiyon kontrol sistemi olarak Git’in yükselişi GitHub’ın yükselişi ile paralellik göstermiştir. 2005 yılında ilk stabil sürümü yayınlanan Git, 2009 ve 2010 yılına kadar sadece Linux ile iç içe olan çevrelerin takip edip kullandığı dağıtık bir versiyon kontrol sistemiydi. Ancak 2009 itibariyle GitHub’ın açık kaynak projeler için ücretsiz Git hizmeti vermeye başlaması, hemen ardından aynı yıllarda Bitbucket’ın ve sonrasında GitLab’ın benzer Git servislerin sağlamaya başlaması Git’in daha geniş kitlelere ulaşmasını ve farklı profillerdeki yazılım geliştiriciler tarafından yoğun bir şekilde kullanılmasını sağladı.

Yazılım Geliştirme ile ilgili çoğu konuda olduğu gibi Git ile ilgili kaynaklar da ağırlıklı olarak İngilizce yazılmaktadır. Türkçe bir kaynak kitap hazırlamanın terminoloji anlamında en büyük zorluğu İngilizce terimler için uygun Türkçe karşılıklarını bulmaktır. Ancak bu kitapta İngilizce-Türkçe geçişini birebir yapmayacağız, mümkün olduğu kadar Versiyon Kontrolü ve Git ile ilgili terimlerin İngilizce hallerine yer vereceğiz. Yazılım Geliştirme alanında kullanılan araçların çoğu kendi terminolojisi ve jargonu ile bilinir bu nedenle kullandığımız İngilizce terimleri İngilizce birere kelime olarak değil Git ile çalışmanın terminolojisi ve jargonu olarak düşünebilirsiniz. Bu terimler profesyonel yaşamınızda ekip arkadaşlarınız ile yapacağınız konuşmalarda sıkça duyup kullanacağınız Git’e dair terimler olarak zihninize yerleştirmelisiniz.

Konuların diziliminde ve içeriğin oluşturulmasında kendi kişisel tecrübemin yansıra Git’i öğrenme ve kendi ekibime bu bilgileri aktarma aşamasında faydalandığım birçok basılı ve çevrimiçi kaynaktan faydalanılmıştır.

Bu kitapta yer verdiğimiz giriş ve temel seviyedeki konuları iyice kavrayıp kendi projelerinizde uyguladıktan sonra daha ileri seviyede Git öğrenmek isterseniz ücretsiz e-kitap olarak yayınlanan ve her zaman güncel tutulan Pro Git isimli kitaptan faydalanabilirsiniz. Pro Git kitabı Git’in temel kaynaklarından birisidir ve Git ile ilgili yayınlanan çoğu basılı ve çevrimiçi kaynak bu kitaba atıfta bulunmaktadır.

Kitaptaki örneklerimizi Terminal \(komut satırı veya command line olarak da tabir edilen\) üzerinden Apple OSX ve Windows işletim sistemleri üzerinde oluşturacağız. Bu kaynağın oluşturulduğu sırada kullanılan OSX ve Git sürüm bilgileri şöyleydi

* OSX 10.12.3 \(Sierra\)

* Git  2.9.3 \(Apple Git-75\)

Windows tarafında ise sürüm bilgileri şu şekilde

* Windows 10 Pro 64 bit
* Git 2.9.2 \(Git for Windows\)

Git, OSX'in yanısıra tüm Linux dağıtımları ve Windows'da da çalışmaktadır. Git komutları kullandığınız işletim sistemine göre değişmez ancak Git kurulumu ve kullanacağımız yardımcı araçlar işletim sistemine göre değişebilir.

