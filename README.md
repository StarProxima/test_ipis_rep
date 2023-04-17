# test_ipis_rep

## Part 1

// Создаём репозиторий \
curl -H "Authorization: token YOUR_TOKEN" --data '{"name":"your_name_rep"}' https://api.github.com/user/repos

// Создаём локальный репозиторий (Инструкция на GitHub)

mkdir your_name_rep

cd your_name_rep

git init

git commit -m "Initial commit"

git branch -M main

// Связываем локальный и реп с origin \
git remote add origin https://github.com/YOUR_NICKNAME/your_name_rep.git

git push -u origin main

// Пишем в hello_world.cpp

git add .

git commit -m "Hello Word"

// Добавляем в hello_world.cpp ввод и вывод

git add .

git commit -m "Hello Word with input and output"

git push

// Проверяем коммиты на GitHub

## Part 2

git checkout -b path1

git add .

// чёт исправляем хз

git commit -m "Fix cringe"

git push
// set-upstream ...

// пулл реквест руками

// пишем комменты

git add .

git commit "Add comments"

git push

// Мерж пулл реквеста ручками, после жмём на кнопку удаления ветки

git switch main

git pull

// Проверяем, что смержилось \
git log

// Удаляем \
git branch -d patch1

## Part 3

git checkout -b path2

// code style mozilla \
clang-format --style=Mozilla hello_world.cpp

git add .

git commit -m "Format code style mozilla"

git push

// пулл реквест вручную

git switch main

// наводим суету, меняем комент, чтобы вызвать конфликт

git add .

git commit -m "Edit comment"

git push

// Чекаем, что в пулл реквесте конфикты

git switch patch2

git pull

git rebase main

// Вот тут у нас конфликты появляются, ресолвим их

git rebase --continue

// Проверям, что конфликты разрешились

// Вливаем пулл реквест в main

## Report

// Или можно создать отдельную ветку и потом смержить \
git switch main

#echo "# your_name_rep" >> README.md

// Пишем репорт

git add .

git commit -m "Add README"

git push



