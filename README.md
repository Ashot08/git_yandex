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