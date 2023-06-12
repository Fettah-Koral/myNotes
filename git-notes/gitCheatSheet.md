
# GitHub Cheatsheets
  
  <h3>Not</h3>
  <p>merge işlemi yaparken text editörüne notlar yazılır ardından <code>:q!</code> komutu ile kaydedilip editörden çıkılır. </p>

   <h2>Projei önceki versiyonuna döndürme</h2>
  <p><code>$ git checkout "[filename]"</code>
  dosyayı en son commit'in eklendiği zamanki haline geri döndürür.</p>
  

  <code>$ git checkout "[commit_id]"</code>
  <p>projeyi herhangi bir commit'in eklendiği spesifik bir versiyona döndürür.</p>

  <h2>Branchler arasında geçiş yapma</h2>
  <p>Eğer hedef şube mevcut değilse “-c” seçeneğini belirtmeniz gerekir (“şube oluştur” için), aksi halde o şubeye geçerken hata mesajı alırsınız.</p>

  <code>

  $ git switch [existing_branch]

  $ git switch -c [non_existing_branch]

  $ git checkout [existing_branch]

  </code>

   <h2>Hazırlık alanında (Stage)  bulunan öğelerden izlemeyi kaldırmak</h2>
   <code>git rm --cached -r .</code>



  
  <h2>Takım yapılandırma</h2>
  <p>Tüm yerel depolar için kullanıcı bilgilerini yapılandırın</p>
  
  <p><code>$ git config --global user.name "[name]"</code></p>
  
  <p>Tüm yerel depolar için kullanıcı bilgilerini yapılandırın</p>
  
  <p><code>$ git config --global user.email "[email address]"</code></p>
  
  <p>Tüm yerel depolar için eposta bilgilerini yapılandırın</p>
  
  <h2 >Depolar oluşturun</h2>
  <p>Yeni bir depo başlatın veya mevcut bir URL’den bir tane edinin</p>
  
  <p><code>$ git init [project-name]</code></p>
  
  <p>Belirtilen adla yeni bir yerel depo oluşturur</p>
  
  <p><code>$ git clone [url]</code></p>
  
  <p>Bir projeyi ve tüm sürüm geçmişini indirin</p>
  
      
  <h2>Değişiklik yapmak</h2>
  <p>Düzenlemeleri inceleyin ve bir işlem gerçekleştirin</p>
  
  <p><code>$ git status</code></p>
  
  <p>Taahhüt edilecek tüm yeni veya değiştirilmiş dosyaları listeler</p>
  
  <p><code>$ git diff</code></p>
  
  <p>Henüz aşamalandırılmamış dosya farklarını gösterir</p>
  
  <p><code>$ git add [file]</code></p>
  
  <p>Sürüm hazırlığı için dosyanın anlık görüntüsünü al.</p>
  
  <p><code>$ git diff --staged</code></p>
  
  <p>Hazırlama ve son dosya sürümü arasındaki dosya farklarını gösterir.</p>
  
  <p><code>$ git reset [file]</code></p>
  
  <p>Dosyayı dizinden kaldırır ama içeriği korur.</p>
  
  <p><code>$ git commit -m"[descriptive message]"</code></p>
  
  <p>Sürüm geçmişinde dosya anlık görüntülerini kalıcı olarak kaydeder</p>
  
  <h2>Grup değişiklikleri</h2>
  <p>Bir dizi taahhüt adı verin ve daha önce tamamlanmış olan çabaları birleştirin</p>
  
  <p><code>$ git branch</code></p>
  
  <p>Geçerli depodaki tüm yerel dalları listeler</p>
  
  <p><code>$ git branch [branch-name]</code></p>
  
  <p>Yeni bir dal oluştur</p>
  
  <p><code>$ git switch -c [branch-name]</code></p>
  
  <p>Belirtilen dala geçer ve çalışma dizinini günceller</p>
  
  <p><code>$ git merge [branch-name]</code></p>
  
  <p>Belirtilen dalın geçmişini mevcut dalla birleştirir</p>
  
  <p><code>$ git branch -d [branch-name]</code></p>
  
  <p>Belirtilen dalı siler</p>
  

      
  <h2>Dosya Yenileme</h2>
  <p>Sürümlü dosyaları taşıma ve silme</p>
  
  <p><code>$ git rm [file]</code></p>
  
  <p>Dosyayı çalışma dizininden siler ve dizini günceller</p>
  
  <p><code>$ git rm --cached [file]</code></p>
  
  <p>Dosyayı sürüm kontrolünden kaldırır ancak dosyayı yerel olarak korur</p>
  
  <p><code>$ git mv [file-original] [file-renamed]</code></p>
  
  <p>Dosya adını değiştirir ve işleme için hazırlayın</p>
  
  <h2>İzlemeyi bastır</h2>
  <p>Geçici dosyaları ve yolları hariç tut</p>
  
  <pre><code>*.log
  build/
  temp-*
  </code></pre>
  
  <p><code>.Gitignore</code> adlı bir metin dosyası, belirtilen kalıplarla eşleşen dosya ve yolların yanlışlıkla sürümlendirilmesini bastırır.</p>
  
  <p><code>$ git ls-files --others --ignored --exclude-standard</code></p>
  
  <p>Bu projedeki yok sayılan tüm dosyaları listeler</p>
  
  <h2>Parçaları kaydet</h2>
  <p>Eksik değişiklikleri sakla ve geri yükle</p>
  
  <p><code>$ git stash</code></p>
  
  <p>Değiştirilmiş tüm sürüm dosyalarını geçici olarak kaydedin</p>
  
  <p><code>$ git stash pop</code></p>
  
  <p>En son saklanan dosyaları geri yükler</p>
  
  <p><code>$ git stash list</code></p>
  
  <p>Önbelleğe alınmış tüm değişiklikleri listeler</p>
  
  <p><code>$ git stash drop</code></p>
  
  <p>En son saklanan değişiklikleri atar</p>
  

      
  <h2>Geçmişi incele</h2>
  <p>Proje dosyalarının gelişimini izlemek ve incelemek</p>
  
  <p><code>$ git log</code></p>
  
  <p>Geçerli dalın sürüm geçmişini listeler</p>
  
  <p><code>$ git log --follow [file]</code></p>
  
  <p>Yeniden adlandırmalar dahil, dosyanın sürüm geçmişini listeler</p>
  
  <p><code>$ git diff [first-branch]...[second-branch]</code></p>
  
  <p>İki dal arasındaki içerik farklarını gösterir</p>
  
  <p><code>$ git show [commit]</code></p>
  
  <p>Belirtilen taahhüdün meta verilerini ve içerik değişikliklerini göster</p>
  
  <h2>Tekrarlama işlemleri</h2>
  <p>Hataları temizle ve değiştirme geçmişini yaz</p>
  
  <p><code>$ git reset [commit]</code></p>
  
  <p>Değişiklikleri yerel olarak koruyarak, <code>[taahhüt]</code> sonrasında verilen tüm taahhütleri geri alır.</p>
  
  <p><code>$ git reset --hard [commit]</code></p>
  
  <p>Tüm geçmişi iptal eder ve belirtilen taahhütte yapılan değişiklikleri geri alır</p>
  
  <h2>Değişiklikleri eşle</h2>
  <p>Bir uzaktan (URL) kaydedin ve depo geçmişini değiştirin</p>
  
  <p><code>$ git fetch [remote]</code></p>
  
  <p>Tüm geçmişi uzak depodan indirir</p>
  
  <p><code>$ git merge [remote]/[branch]</code></p>
  
  <p>Uzak dalı geçerli yerel dalla birleştirir</p>
  
  <p><code>$ git push [remote] [branch]</code></p>
  
  <p>Tüm yerel dal işlemlerini GitHub’a yükler</p>
  
  <p><code>$ git pull</code></p>
  
  <p>Yer imi geçmişini indirir ve değişiklikleri içerir</p>
  

      