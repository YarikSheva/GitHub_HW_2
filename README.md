# GitHub_HW_2
создаём и kлонируем внешний репозиторий git clone , не забыть перейти в главную ветку

На локальном репозитории сделать ветки для:
-Postman

git branch Postman

#or создать и сразу в неё перейти
git checkout -b Postman

#вернуться обратно на главную ветку
git checkout main
-Jmeter

git branch Jmeter
-CheckLists

git branch CheckLists
-Bug_Reports

git branch Bug_Reports
-SQL

git branch SQL
-Charles

git branch Charles
-Mobile_testing

git branch Mobile_testing
#проверить все ли ветки создались

git branch
Запушить все ветки на внешний репозиторий
git push origin --all
В ветке Bug Reports сделать текстовый документ со структурой баг репорта
  git checkout Bug_Reports  --> 
  vim Bug_Reports.txt
  .
  .
  Esc
:wq

 or
 
  git checkout Bug_Reports -->
  cat > Bug_Reports.txt
  ^C
    
|ID|Version|Environment|Summary|STR|Expected Result|Actual Result|Severity|Priority|Attachments|
  
  or 
Environment:
ID:
Summary:
Steps to reproduce:
Actual Result:
Expected Result:
Attachments:
#проверить создание файла
git status
Запушить структуру багрепорта на внешний репозиторий
git add Bug_Reports.txt  -->
git commit -m "add file bug_reports"  -->
git push --set-upstream origin Bag_reports
Вмержить ветку Bug Reports в Main
git checkout main  -->
git merge Bug_Reports
Запушить main на внешний репозиторий.
 git push
В ветке CheckLists набросать структуру чек листа.
git checkout CheckLists  -->
vim CheckLists.txt
.
.
Esc
:wq

or
git checkout CheckLists  -->
cat > CheckLists.txt
^C    
    
|ID|Check|Result|Comment|

 
or 

ID:
Check:
Result:
Comment:
 
Запушить структуру на внешний репозиторий
git add .  -->
git commit -m "add file checklis"  -->
git push origin CheckLists
На внешнем репозитории сделать Pull Request ветки CheckLists в main
#in web Compare & pull request ▶️ Create pull request ▶️ Merge pull request ▶️ Confirm merge

Синхронизировать Внешнюю и Локальную ветки Main
git checkout main
    
#посмотреть были ли изменения
git fetch
--> 
git pull
