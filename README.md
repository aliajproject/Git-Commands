Gedin Əmrləri
============

_Tez-tez istifadə olunan Git əmrlərinin siyahısı_

Git ləqəbləri ilə maraqlanırsınızsa, burada mövcud olan '.bash_profile'-ə nəzər salın: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

*Tərcümədə mühüm ingiliscə sözlərin orijinalı qorunub saxlanılıb, “repository” sözü “repo”, “local” sözü “local”, “remote” sözü “remote” kimi tərcümə edilib. "uzaq". Bunları nəzərə alaraq sənəddən yararlana bilərsiniz”.

---

<details>
<summary><b>Layihələrin idxalı və yaradılması:</b></summary> 

| Əmr | İzahat |
| ------- | ----------- |
| ```git init``` | Yerli Git repo işə salın |
| ```git clone ssh://git@github.com/[username]/[repository-name].git``` | Uzak bir reponun yerel bir kopyasını oluştur |
</details>




<details>
<summary><b>Əsas Snapshot:</b></summary> 

| Komut | Açıklama |
| ------- | ----------- |
| ```git status``` | Durumu kontrol et |
| ```git add [file-name.txt]``` | Hazırlama alanına bir dosya ekle |
| ```git add -A``` | Tüm yeni ve değiştirilen dosyaları hazırlama alanına ekleyin |
| ```git commit -m "[commit message]"``` | Değişiklikleri commit et (açıkla) |
| ```git rm -r [file-name.txt]``` | Dosyayı (ya da dizini) sil |
</details>
### Dallanma ve Birleşme

| Komut | Açıklama |
| ------- | ----------- |
| `git branch` | Bracnh'leri listeleyin (yıldız işareti mevcut branch'i gösterir) |
| `git branch -a` | Tüm brach'leri listele (yerel ve uzak) |
| `git branch [branch name]` | Yeni bir branch oluştur |
| `git branch -d [branch name]` | Branch'i sil |
| `git push origin --delete [branch name]` | Uzak branch'i sil |
| `git checkout -b [branch name]` | Yeni bir branch oluştur ve ona geçiş yap |
| `git checkout -b [branch name] origin/[branch name]` | Uzak branch'i klonla ve ona geçiş yap |
| `git branch -m [old branch name] [new branch name]` | Yerel branch'i yeniden adlandır |
| `git checkout [branch name]` | Belirtilen branch'e geçiş yap |
| `git checkout -` | Son kontrol edilen branch'e geç |
| `git checkout -- [file-name.txt]` | Bir dosyadaki değişiklikleri sil |
| `git merge [branch name]` | Bir branch'i aktif branch ile birleştir |
| `git merge [source branch] [target branch]` | Branch'i hedef branch ile birleştir |
| `git stash` | Yarım kalan bir çalışma dizinindeki değişiklikleri saklayın |
| `git stash clear` | Saklanan tüm girişleri kaldır |

### Projeleri Paylaşma ve Güncelleme

| Komut | Açıklama |
| ------- | ----------- |
| `git push origin [branch name]` | Uzak repoya bir branch gönder |
| `git push -u origin [branch name]` | Değişiklikleri uzak repoya aktarın (ve branch'i hatırla) |
| `git push` | Değişiklikleri uzak repoya aktarın (ve branch'i hatırla) |
| `git push origin --delete [branch name]` | Uzak branch'i sil |
| `git pull` | Yerel repoyu en yeni commit'e güncelleyin |
| `git pull origin [branch name]` | Değişiklikleri uzak repodan çek |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Uzak repo ekle |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Bir reponun başlangıç branch'ini SSH olarak ayarla |

### İnceleme ve Karşılaştırma

| Komut | Açıklama |
| ------- | ----------- |
| `git log` | Değişiklikleri görüntüle |
| `git log --summary` | Değişiklikleri görüntüle (detaylı) |
| `git log --oneline` | Değişiklikleri görüntüle (kısaca) |
| `git diff [source branch] [target branch]` | Birleştirmeden önce değişiklikleri önizle |
