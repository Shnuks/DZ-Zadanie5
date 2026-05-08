# Домашнее задание к занятию 5
<h2>Fork проекта находится по ссылке https://github.com/Shnuks/shvirtd-example-python.git</h2>
<h1>Задача 0</h1>
<h3>Решение</h3>
<img width="549" height="132" alt="image" src="https://github.com/user-attachments/assets/a32eb941-f54d-430a-a15b-82119f67078f" />
<h1>Задача 1</h1>
<h3>Решение</h3>
fork создан; добавлены Dockerfile.python, .dockerignore билд успешный
<h1>Задача 3</h1>
<img width="1419" height="212" alt="image" src="https://github.com/user-attachments/assets/2eaad62e-cb85-4b84-af7a-c831eeeedbf4" />
...
<img width="412" height="171" alt="image" src="https://github.com/user-attachments/assets/1a7299cb-35f9-4aa2-a9a3-d23f27424853" />

<h1>Задача 4</h1>
<pre>
#!/bin/bash

REPO_URL="https://github.com/Shnuks/shvirtd-example-python.git"
TARGET_DIR="/opt/netology"

if [ -d "$TARGET_DIR" ]; then
  echo "Обновление репозитория"
  cd $TARGET_DIR
  git pull
else
  echo "Клонирование репозитория"
  git clone $REPO_URL $TARGET_DIR
  cd $TARGET_DIR
fi

echo "Запуск проекта"
docker compose down
docker compose up -d

echo "Успешно!!!"
</pre>



<h1>Доделываю</h1>
