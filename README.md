# GitHub_BRANCH_HW_2
#  GitHub. HW_2
1.  **На локальном репозитории сделать ветки для :**

     `git branch Postman`
  
      `git branch Jmeter`
  
      `git branch CheckLists`
  
      `git branch BugReports`
  
      `git branch SQL`
  
      `git branch Charles`
  
      `git branch MobileTesting`
  

2.  **Запушить все ветки на внешний репозиторий :**

     
     `git push -u origin Postman`
     
     `git push -u origin Jmeter`
     
     `git push -u origin CheckLists`
     
     `git push –u origin BugReports`		 
     
     `git push -u origin SQL`
     
     `git push -u origin Charles`
     
     `git push -u origin MobileTesting`

3. **В ветке BugReports сделать текстовый документ со структурой баг репорта :**
     `git checkout BugReports`
     `vim BR.txt-> i -> `

id- уникальный номер дефекта 
severity - серьезность дефекта
Environment - окружение на котором обнаружен дефект
Title - краткое описание дефекта (что? где? когда?)
Steps - шаги для воспроизведения дефекта
Expected Result - ожидаемый результат
Actual Result - фактический результат
Attachment - ссылка на видео или фото дефекта 

-> Esc :wq -> Enter
 git add BR.txt
 git commit –m "new_BR"

4. Запушить структуру багрепорта на внешний репозиторий ==== git push

5. Вмержить ветку BugReports в Main ===
 git checkout main
 git merge BugReports

6. Запушить main на внешний репозиторий. === git push –u origin main

7. В ветке CheckLists набросать структуру чек листа. ===
  git checkout CheckList 
 vim checklict.txt -> i ->
 1. ID
 2. TITLE
 3. STATUS
 4. LINK

-> Esc :wq -> Enter
 git add checklict.txt
 git commit –m “chlt”

8. Запушить структуру на внешний репозиторий === git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main === 
 Git hub -> выбираем ветку CheckList -> нажимаем Pull request ->      выбираем checklist в main ->  жмем Compare & pull request
-> Create pull request -> Merge pull request -> Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main  ===  
    На локальном в терменале переходим в ветку main
  git checkout main
  git fetch
  git pull
