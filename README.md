# git-learn
Test

New text


New text 2
<aside>
💡 Основные команды:

</aside>

- git pull
- git push
- pull request - запрос на вливание изменений в репозиторий
- touch -создание файла
- mkdir
- cd
- echo
- 

<aside>
💡 Ключи SSH (ч/з git bash)

</aside>

- ssh-keygen -t ed25519 -b 4096 - сгенерировать ключи SSH
- ввести имя файла для хранения ключей, н-р, ssh-key-09 (появится картинка)
- скопировать ключи в папку .ssh
- перед git pull или git push выполнить идентификацию компа с помощью команд
 + eval "$(ssh-agent -s)”   
 + ssh-add ~/.ssh/ssh-key-84
