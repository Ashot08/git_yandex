# Git terminal commands

---

```
git config --global user.name NAME    				
```

задать имя пользователя = NAME


```
git config --global user.email EMAIL				
```

задать email = EMAIL


```
git config --list						
```

посмотреть конфиг


```
cat ~/.gitconfig 						
```

посмотреть конфиг


```
git init							
```

инициализировать Гит в проекте


```
rm -rf .git							
```

удалить Гит из проекта


```
git status							
```

показать текущее состояние репозитория


```
git add FILENAME						
```

добавить все файл с именем FILENAME к отслеживанию


```
git add --all							
```

добавить все файлы к отслеживанию


```
git add . 							
```

добавить всю текущую папку


```
git commit -m "Мой коммит!"					
```

сохраняем состояние файлов с комментарием (-m) "Мой коммит!"


```
git log								
```

посмотреть историю коммитов 


```
git log --oneline 
```

вывод сокращенной истории коммитов 


```
ssh -T git@github.com						
```

тестирование подключения по протоколу SSH


```
git remote add origin git@github.com:ACCOUNTNAME/REPNAME.git 	
```

подключиться к удаленному репозиторию


```
git remote -v							
```

проверить, что локальный репозиторий привязан к удаленному


```
git remote remove origin					
```

удалить подключение к удаленному репозиторию


```
git push -u origin BRANCHNAME					
```

запушить в удаленный репозиторий (github) в ветку с именем BRANCHNAME. Пример: git push -u origin main.
Флаг -u свяжет локальную ветку с одноимённой удалённой (обычно первый раз пушат так как в примере, потом просто "git push")


```
git commit --amend --no-edit					
```

Дополнить последний, уже сделанный коммит - добавить в ПОСЛЕДНИЙ коммит забытые файлы (делаем git add для файлов которые забыли добавить в 	 	
коммит, потом git commit --amend --no-edit). Точно так же можно добавить не новый файл, а дополнительные изменения в уже добавленном в коммит файле.


```
git commit --amend -m "MESSAGE"					
```

Изменить комментарий в последнем коммите на MESSAGE


```
git commit --amend				
```

Дополнить последний, уже сделанный коммит + вручную изменить комментарий в редакторе (nano, vim итп)


```
git restore --staged FILENAME	
```

Убрать файл из staging (отменить git add для файла с именем FILENAME)


```
git restore --staged .
```

«Сбросить» все файлы из staged обратно в untracked/modified


```
git restore FILENAME
```

«Откатить» изменения, которые не попали ни в staging, ни в коммит - Changes not staged for commit (modified)


```
git reset --hard COMMIT_HASH
```

«Откатить» к коммиту с хэшем = COMMIT_HASH


```
git diff
```

сравнить последнюю закоммиченную версию файла с текущей (изменённой) версией


```
git diff --staged	
```

просмотреть изменения в staged


```
git clone REP_URL						
```

клонировать удаленный репозиторий в локальный (с привязкой к удаленному)


```
git branch
```

вывести инфу о ветках


```
git branch BRANCH_NAME	
```

создань ветку с именем BRANCH_NAME


```
git checkout BRANCH_NAME
```

переключиться на ветку с именем BRANCH_NAME


