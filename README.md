# GIT_homework_2
Создала на Github репозиторий, перетащила его на комп
git clone https://github.com/natalisilina2022/GIT_homework_2.git

переключилась на него
cd GIT-homework_2

1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

git branch name, все по одной ветке создала

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch Jmeter

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch CheckLists

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch BagReports

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch SQL

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch Charles

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch MobileTesting

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git branch
  BagReports
  Charles
  CheckLists
  Jmeter
  MobileTesting
  Postman
  SQL
* main

2. Запушить все ветки на внешний репозиторий

git push -u --all

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git push -u --all
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/natalisilina2022/GIT_homework_2.git
 * [new branch]      BagReports -> BagReports
 * [new branch]      Charles -> Charles
 * [new branch]      CheckLists -> CheckLists
 * [new branch]      Jmeter -> Jmeter
 * [new branch]      MobileTesting -> MobileTesting
 * [new branch]      Postman -> Postman
 * [new branch]      SQL -> SQL
branch 'main' set up to track 'origin/main'.
branch 'BagReports' set up to track 'origin/BagReports'.
branch 'Charles' set up to track 'origin/Charles'.
branch 'CheckLists' set up to track 'origin/CheckLists'.
branch 'Jmeter' set up to track 'origin/Jmeter'.
branch 'MobileTesting' set up to track 'origin/MobileTesting'.
branch 'Postman' set up to track 'origin/Postman'.
branch 'SQL' set up to track 'origin/SQL'.

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git checkout BagReports
Switched to branch 'BagReports'
Your branch is up to date with 'origin/BagReports'.

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ touch bagReport.txt

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ vim bagReport.txt

4. Запушить структуру багрепорта на внешний репозиторий

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ git add bagReport.txt
warning: LF will be replaced by CRLF in bagReport.txt.
The file will have its original line endings in your working directory

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ git commit bagReport.txt
warning: LF will be replaced by CRLF in bagReport.txt.
The file will have its original line endings in your working directory
[BagReports e43aaab] add file bagReports txt
 1 file changed, 11 insertions(+)
 create mode 100644 bagReport.txt

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 521 bytes | 521.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/natalisilina2022/GIT_homework_2.git
   eea93de..e43aaab  BagReports -> BagReports

5. Вмержить ветку Bag Reports в Main

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (BagReports)
$ git checkout -
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git merge BagReports
Updating eea93de..e43aaab
Fast-forward
 bagReport.txt | 11 +++++++++++
 1 file changed, 11 insertions(+)
 create mode 100644 bagReport.txt

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

6. Запушить main на внешний репозиторий.

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/natalisilina2022/GIT_homework_2.git
   eea93de..e43aaab  main -> main

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

7. В ветке CheckLists набросать структуру чек листа.

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (main)
$ git checkout CheckLists
Switched to branch 'CheckLists'
Your branch is up to date with 'origin/CheckLists'.

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (CheckLists)
$ touch checkList.txt

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (CheckLists)
$ vim checkList.txt

8. Запушить структуру на внешний репозиторий

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (CheckLists)
$ git add checkList.txt
warning: LF will be replaced by CRLF in checkList.txt.
The file will have its original line endings in your working directory

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (CheckLists)
$ git commit -m "add file chekList"
[CheckLists c1fbc47] add file chekList
 1 file changed, 8 insertions(+)
 create mode 100644 checkList.txt

netty@DESKTOP-46NPOM6 MINGW64 ~/QA/GIT/GIT_homework_2 (CheckLists)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 403 bytes | 403.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/natalisilina2022/GIT_homework_2.git
   eea93de..c1fbc47  CheckLists -> CheckLists

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

10. Синхронизировать Внешнюю и Локальную ветки Main

Тут я сразу сделала git pull

но как я потом увидела в комментариях в чате, здесь я что-то пропустила, я должна была сначала сделать git fetch или
git remote?
