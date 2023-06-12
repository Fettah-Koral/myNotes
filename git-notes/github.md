## GitHub nedir?

GitHub, sürüm kontrolü ve işbirliği için bir kod barındırma platformudur. Sizin ve diğer kişilerin her yerden projeler üzerinde birlikte çalışmasına olanak tanır.

## Repository nedir? (depo)
Bir depo genellikle tek bir projeyi organize etmek için kullanılır. Depolar, projenizin ihtiyaç duyduğu her şeyi içeren klasörler ve dosyalar, resimler, videolar, elektronik tablolar ve veri kümeleri içerebilir.

## Branch nedir? (dal)
Dallanma, aynı anda bir reponun farklı sürümlerine sahip olmanızı sağlar.
Varsayılan olarak, deponuz, kesin dal olarak kabul edilen ``main`` adlı bir dala (ana dal) sahiptir. Deponuzda main dışında ek dallar oluşturabilirsiniz.Aynı anda bir projenin farklı sürümlerine sahip olmak için dalları kullanabilirsiniz. Bu, ana kod kaynağını değiştirmeden bir projeye yeni özellikler eklemek istediğinizde faydalıdır. Farklı dallarda yapılan işler siz birleştirene kadar ana şubede görünmeyecek


Ana daldan bir dal oluşturduğunuzda, ana dalın o andaki haliyle bir kopyasını veya anlık görüntüsünü yapmış olursunuz. Siz farklı bir dalla çalışırken başka biri ana dalda değişiklik yaptıysa, bu güncellemeleri alabilirsiniz.
![Alt text](https://docs.github.com/assets/cb-23923/mw-1440/images/help/repository/branching.webp)

## Commits (Teslim etmek ,işlemek)

Deponuzdaki dosyalarda değişiklik yapabilir ve kaydedebilirsiniz. GitHub'da kaydedilen değişikliklere commits denir. Her teslim, belirli bir değişikliğin neden yapıldığını açıklayan bir açıklama olan ilişkili bir teslim mesajı vardır. Teslim mesajları, diğer katkıda bulunanların ne yaptığınızı ve neden yaptığınızı anlayabilmesi için değişikliklerinizin geçmişini yakalar.

## Pull Requests (çekme istekleri)
Ana daldan türetilen bir dalda değişiklik yaptıktan sonra bir çekme isteği açabilirsiniz.

Çekme istekleri, GitHub'da işbirliğinin kalbidir. Bir çekme talebi açtığınızda, değişikliklerinizi öneriyorsunuz ve birisinin katkınızı inceleyip çekmesini ve bunları kendi dallarında birleştirmesini talep ediyorsunuz.

Çekme istekleri, içeriğin her iki koldan farklılıklarını veya farklılıklarını gösterir. Değişiklikler, eklemeler ve çıkarmalar farklı renklerde gösterilir.Bir teslim de bulunur bulunmaz, bir çekme isteği açabilir ve daha kod bitmeden bir tartışma başlatabilirsiniz.

Çekme isteği mesajınızda GitHub'ın ``@mention`` özelliğini kullanarak, koridorun sonunda veya 10 saat dilimi uzakta olsunlar, belirli kişilerden veya ekiplerden geri bildirim isteyebilirsiniz.

![](https://docs.github.com/assets/cb-32937/mw-1440/images/help/repository/diffs.webp)

## Merging pull request (Çekme isteğini birleştirme)

Bu son adımda, düzenlemeleri yaptığınız diğer dalınızı ana dalla birleştireceksiniz. Çekme isteğinizi birleştirdikten sonra, düzenlemeleri daldaki değişiklikler main'e dahil edilecektir.

Bazen bir çekme isteği, ana koddaki mevcut kodla çakışan kod değişiklikleri getirebilir. Herhangi bir çakışma varsa GitHub, çakışan kod hakkında sizi uyaracak ve çakışmalar çözülene kadar birleştirmeyi engelleyecektir.

Çakışmaları çözen bir  teslimatta (commit) bulunabilir veya çekme isteğindeki yorumları ekip üyelerinizle çatışmaları tartışmak için kullanabilirsiniz


![](https://miro.medium.com/v2/resize:fit:880/1*byFLi3Ljdzc8_x6B6el2EA.jpeg)