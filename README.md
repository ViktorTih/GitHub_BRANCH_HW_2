
#  GitHub. HW_2
1.  **На локальном репозитории сделать ветки для :**

    + Postman      `git branch Postman`
  
    + Jmeter      `git branch Jmeter`
  
    + CheckLists   `git branch CheckLists`
  
    + BugReports   `git branch BugReports`
  
    + SQL          `git branch SQL`
  
    + Charles      `git branch Charles`
  
    + MobileTesting `git branch MobileTesting`
  

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
     
       1. Id- уникальный номер дефекта
       2. Severity - серьезность дефекта
       3. Environment - окружение на котором обнаружен дефект
       4. Title - краткое описание дефекта (что? где? когда?)
       5. Steps - шаги для воспроизведения дефекта
       6. Expected Result - ожидаемый результат
       7. Actual Result - фактический результат
       8. Attachment - ссылка на видео или фото дефекта
       
     `-> Esc :wq -> Enter`

      `git add BR.txt`
 
      `git commit –m "new_BR"`

4. **Запушить структуру багрепорта на внешний репозиторий :**

      `git push`
    
5. **Вмержить ветку BugReports в Main :**

     `git checkout main`
 
     `git merge BugReports`

6. **Запушить main на внешний репозиторий :**
 
     `git push –u origin main`

7. **В ветке CheckLists набросать структуру чек листа :**

     `git checkout CheckList`
     
     `vim checklict.txt -> i ->`
     
       1. Id
       2. Title
       3. Status
       4. Link

      `-> Esc :wq -> Enter`

      `git add checklict.txt`
 
      `git commit –m “checklict.txt”`

8. **Запушить структуру на внешний репозиторий :** 

      `git push`

9. **На внешнем репозитории сделать Pull Request ветки CheckLists в main :**
 
      `заходим на Git hub -> выбираем ветку CheckList -> нажимаем Pull request ->`
      
      `выбираем checklist в main ->  жмем Compare & pull request->`
      
      `жмём Create pull request ->  жмём Merge pull request -> жмём Confirm merge`

10. **Синхронизировать Внешнюю и Локальную ветки Main :** 

        На локальном в "терменале" переходим в ветку main
        
      `git checkout main`
  
      `git fetch`
  
       `git pull`
