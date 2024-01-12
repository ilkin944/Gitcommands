Git Terminal Əmrləri
============

## Tez-tez istifadə olunan Git əmrlərinin siyahısı

### Proyekt Yaratmaq və Çəkmək

| Əmr | Açıqlama |
| ------- | ----------- |
| `git init` | Local Git repo yaratmaq |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Xarici bir reponu local-a kopyalamaq |

### Əsas Snapshot

| Əmr | Açıqlama |
| ------- | ----------- |
| `git status` | Dəyişiklikləri yoxlamaq |
| `git add [fayl adı.txt]` | Stage sahəsinə fayl əlavə edin |
| `git add -A` | Bütün yeni və dəyişdirilmiş faylları stage sahəsinə əlavə edin |
| `git commit -m "[kommit mesajı]"` | Dəyişikliklərə mesaj yazın |
| `git rm -r [fayl adı.txt]` | Faylı silin |

### Budaqlanma və birləşmə

| Əmr | Açıqlama |
| ------- | ----------- |
| `git branch` | Filialların siyahısı (ulduz cari filialı göstərir) |
| `git branch -a` | Bütün branchları sadalayın (local və remote) |
| `git branch [filial adı]` | Yeni filial yaradın |
| `git branch -d [filial adı]` | Filialı silin |
| `git push origin --delete [filial adı]` | Uzaq filialı silin |
| `git checkout -b [filial adı]` | Yeni filial yaradın və ona keçin |
| `git checkout -b [filial adı] origin/[filial adı]` | Uzaq filialı klonlayın və ona keçin |
| `git branch -m [köhnə filial adı] [yeni filial adı]` | Local filialın adını dəyişdirin |
| `git checkout [filial adı]` | Göstərilən filiala keçin |
| `git checkout -` | Son yoxlanılan filiala keçin |
| `git checkout -- [fayl adı.txt]` | Fayldakı dəyişiklikləri silin |
| `git merge [filial adı]` | Filialı aktiv filiala birləşdirin |
| `git merge [mənbə filialı] [hədəf filialı]` | Filialı hədəf filiala birləşdirin |
| `git stash` | Dəyişiklikləri çirkli iş qovluğunda saxlayın |
| `git stash clear` | Bütün saxlanan qeydləri silin |

### Layihələrin Paylaşılması və Yenilənməsi

| Əmr | Açıqlama |
| ------- | ----------- |
| `git push origin [filial adı]` | Uzaq repoya filial göndərin |
| `git push -u origin [filial adı]` | Dəyişiklikləri uzaq repoya göndərmə (və filialı xatırlaması) |
| `git push` | Dəyişiklikləri uzaq repoya göndərmək (və filialı xatırlayın) |
| `git push origin --delete [filial adı]` | Uzaq filialı silin |
| `git pull` | Local reponu son öhdəliyə yeniləyin |
| `git pull origin [filial adı]` | Uzaq repodan dəyişiklikləri çəkin |
| `git remote add source ssh://git@github.com/[username]/[repository-name].git` | Uzaqdan repo əlavə et |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Reponun başlanğıc filialını SSH | olaraq təyin edin

### Nəzərdən keçirmə və müqayisə

| Əmr | Açıqlama |
| ------- | ----------- |
| `git log` | Dəyişikliklərə baxın |
| `git log --summary` | Dəyişikliklərə baxın (ətraflı) |
| `git log --oneline` | Dəyişikliklərə baxın (qısaca) |
| `git diff [mənbə filialı] [hədəf filial]` | Birləşmədən əvvəl dəyişiklikləri nəzərdən keçirin |
