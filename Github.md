### Работа c GitHub
___
Чтобы начать работать с GitHub необходимо сначала зарегистрироваться на GitHub. После регистрации можно приступать к ***созданию репозитория***.

### Создание репозитория
___

Чтобы создать репозиторий необходимо на главной страницы найти кнопку *"New repository"*. В следующем окне будет предложено заполнить несколько параметров.  
*"Repository name"* название вашего репозитория  
*"Description"* краткое описания вашего репозитория  
Выбрать какой будет доступ к вашему репозиторию открытый или закрытый *"Public"* или *"Private"*  
И предложено создать файл *"Readme.md"* и *".gitignore"*
Можно данные файлы не создавать, а создать их позже на локальной машине, с последующим переносом на GitHub.  
Также будет предложено создать файл *"license"*, файл описывающий, как можно или нельзя использовать ваш код. Данный файл также можно создать на локальной машине.  

### Страница первоначальными командами
___
После того, как будет создан репозиторий необходимо выполнить первоначальные команды.  
На выбор предлагается два варианта  
***…or create a new repository on the command line***
```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://example.com/example/example.git
git push -u origin main
```
***…or push an existing repository from the command line***  

```
git remote add origin https://example.com/example/example.git
git branch -M main
git push -u origin main
```
В первом варианте *создается файл*, *иницилализируется новый репозиторий*, *добавляется файл Readme.md в индекс*, *создается коммит*, *git branch -m main* данную команду можно не выполнять, так как по умолчанию основная ветка у на *master*, *добавляется новый удаленный репозиторий*, *с локальной машины отправляются на удаленный репозиторий изменения*  

Во втором варианте на локальной машине должен уже быть создан репозиторий, добавлен файл, создан коммит и тогда мы можем в ветку master на *удаленном репозитории* внести изменения.