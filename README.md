# небольшая шпаргалка по git

##  создать новый проект

```bash
git init             # создать новый проект в текущей директории
git init folder-name # создать новый проект в указанной директории
```
## вывести список локальных веток

```bash
git branch
```
## Список удаленных веток (remote) 

```bash
git branch -r
```
## Список всех веток

```bash
git branch -a
```

## Cписок удаленных репозиториев

```bash
git remote -v

```


## Как переключиться на ветку в Git

```bash
git checkout master

```

## Как создать ветку на основе текушей 

```bash
git checkout -b ＜new-branch＞

git checkout -b ＜new-branch＞ ＜existing-branch＞


```

## добавить все изменения

```
git add .

```

## Закоммитить 

```
git commit -m " "

```

##  Добавить ветку в удалённый репозиторий

```
git push -u origin удалённая ветка

```

## спрятать изменения 

```
git stash

git stash save ""

git stash list

git stash show

git stash apply

git stash pop

git stash branch new-name

git stash drop

git stash clear

```

## Копирование коммита (перенос коммитов)

```
git cherry-pick 5589877          # скопировать на активную ветку изменения из указанного коммита, закоммитить эти изменения
git cherry-pick master~2..master # скопировать на активную ветку изменения из master (2 последних коммита)
git cherry-pick -n 5589877       # скопировать на активную ветку изменения из указанного коммита, но НЕ КОММИТИТЬ (подразумевается, что мы сами потом закоммитим)
git cherry-pick master..feature  # скопировать на активную ветку изменения из всех коммитов ветки feature с момента её расхождения с master (похоже на слияние веток, но это копирование изменений, а не слияние), закоммитить эти изменения; это может вызвать конфликт
git cherry-pick --abort    # прервать конфликтный перенос коммитов
git cherry-pick --continue # продолжить конфликтный перенос коммитов (сработает только после решения конфликта)
```

## Удалить ветку

```
git branch -d  local_branch_name
```
