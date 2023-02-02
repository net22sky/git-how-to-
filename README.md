# небольшая шпаргалка по git


## вывести список локальных веток

```bash
git branch
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