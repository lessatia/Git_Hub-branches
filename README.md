# Git_Hub-branches
Предварительно создать внешний репозиторий. Для работы клонировать его через терминал на локалку.

На локальном репозитории сделать ветки для:
Postman
Jmeter
CheckLists
Bag Reports
SQL
Charles
Mobile testing
git branch Postman
git branch Jmeter
git branch CheckList
git branch Bug_Reports 
git branch SQL
git branch Charles
git branch Mobile_testing
Запушить все ветки на внешний репозиторий
git push -u --all
В ветке Bag Reports сделать текстовый документ со структурой баг репорта
git checkout Bug_Reports
vim pattern_bug_report.txt
#  перехожу в режим редактирования (I) и прописываю 
1. Summary
2. Project
3. Component
4. Version
5. Severity
6. Priority
7. Steps to Reproduce
8. Actual Result
9. Expected Result
10. Additional Information
#  ESC 
#  :wq
Запушить структуру багрепорта на внешний репозиторий
git add .
git commit -m "bug report"
git push
Вмержить ветку Bag Reports в Main
git merge Bug_Reports
Запушить main на внешний репозиторий.
cd ..
git add .
git commit -m "merge vetok"
git push
В ветке CheckLists набросать структуру чек листа.
git checkout CheckList
vim pattern_checklist.txt
#  перехожу в режим редактирования (I) и прописываю
1. ID
2. Tester Action
3. Actual Result
4. Comment
#  ESC 
#  :wq
Запушить структуру на внешний репозиторий
git add .
git commit -m "checlistt"
git push
На внешнем репозитории сделать Pull Request ветки CheckLists в main
Интуитивно понятно (в нужном  внешнем репозитории сверху будет кнопка для pull. 
Далее кликаем по зеленым кнопкам и все сохраняем)
Синхронизировать Внешнюю и Локальную ветки Main
git checkout master
git pull
