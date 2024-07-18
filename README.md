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
| ```git init``` | Yerli Git repo-nu buraxın |
| ```git clone ssh://git@github.com/[username]/[repository-name].git``` | Uzaqdan repo-nun yerli surətini yaradın  |
</details>




<details>
<summary><b>Əsas Snapshot:</b></summary> 

| Əmr | İzahat |
| ------- | ----------- |
| ```git status``` | Vəziyyəti yoxlayın |
| ```git add [file-name.txt]``` | Səhnə sahəsinə fayl əlavə edin |
| ```git add -A``` | Bütün yeni və dəyişdirilmiş faylları quruluş sahəsinə əlavə edin|
| ```git commit -m "[commit message]"``` | Dəyişiklikləri qəbul edin |
| ```git rm -r [file-name.txt]``` | Faylı (və ya qovluğu) silin |
</details>

<details>
<summary><b>Budaqlanma və birləşmə:</b></summary> 

| Əmr | İzahat |
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
</details>

<details>
<summary><b>Layihələrin Paylaşılması və Yenilənməsi:</b></summary> 

| Əmr | İzahat |
| ------- | ----------- |
| `git push origin [branch name]` | Uzak repoya bir branch gönder |
| `git push -u origin [branch name]` | Değişiklikleri uzak repoya aktarın (ve branch'i hatırla) |
| `git push` | Değişiklikleri uzak repoya aktarın (ve branch'i hatırla) |
| `git push origin --delete [branch name]` | Uzak branch'i sil |
| `git pull` | Yerel repoyu en yeni commit'e güncelleyin |
| `git pull origin [branch name]` | Değişiklikleri uzak repodan çek |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Uzak repo ekle |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Bir reponun başlangıç branch'ini SSH olarak ayarla |
</details>

<details>
<summary><b>Nəzərdən keçirmə və müqayisə:</b></summary> 
  
| Əmr | İzahat |
| ------- | ----------- |
| `git log` | Değişiklikleri görüntüle |
| `git log --summary` | Değişiklikleri görüntüle (detaylı) |
| `git log --oneline` | Değişiklikleri görüntüle (kısaca) |
| `git diff [source branch] [target branch]` | Birleştirmeden önce değişiklikleri önizle |
</details>
