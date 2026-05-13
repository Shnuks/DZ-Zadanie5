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
<h3>Созданная ВМ</h3>
<img width="1841" height="268" alt="изображение" src="https://github.com/user-attachments/assets/9750f4a0-c838-4e8a-bbe4-06e44592f2f7" />


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
<img width="1014" height="814" alt="изображение" src="https://github.com/user-attachments/assets/73449f29-4af3-4a5a-8040-ab8835d34a54" />
<img width="1100" height="493" alt="изображение" src="https://github.com/user-attachments/assets/d5574528-d44c-4b61-bc8f-c320e6892723" />
<h4>Появилась ошибка в доступности, сам не разобрался с чем связано</h4>
<img width="1202" height="581" alt="изображение" src="https://github.com/user-attachments/assets/61ed8c21-922a-4bd6-9a20-220da38f498a" />
<img width="863" height="908" alt="изображение" src="https://github.com/user-attachments/assets/828864c2-5ec7-40f6-b0fc-fe8db96c8281" />
<h3>При ручном разворачивании</h3>
<img width="1267" height="279" alt="изображение" src="https://github.com/user-attachments/assets/6fb669c5-705a-4d4c-b1c3-db14dc397581" />
<img width="857" height="552" alt="изображение" src="https://github.com/user-attachments/assets/59cf18be-bfa2-42a5-b776-b6dbc66ac4b6" />




<h1>Задача 6</h1>
<h3>Скачивание образа</h3>
<img width="739" height="293" alt="image" src="https://github.com/user-attachments/assets/a9f2bcbc-f104-4a03-b7f8-1de32ee1f417" />
<h3>Поиск с помощью dive</h3>
<img width="1920" height="1050" alt="image" src="https://github.com/user-attachments/assets/f9701371-bb72-4f42-a830-98aba979a3a5" />
<h3>Сохраниние бинарника на локальной вм с помощью docker save</h3>
<img width="887" height="893" alt="image" src="https://github.com/user-attachments/assets/c86a7562-7631-4851-90fa-e405d11911a4" />

<h1>Задача 6.1</h1>
<img width="1182" height="536" alt="image" src="https://github.com/user-attachments/assets/0cb004be-40d3-433e-a406-c1a400a3b73f" />








