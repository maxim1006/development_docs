#npm list package__name
посмотреть версии пакета установленного в проекте

#npm view package__name
посмотреть все версии пакета

#npm audit fix
если в проекте есть package.lock файл, то команда проверит все пакеты на секьюрити уязвимости

#npm audit 
Проверка на пакеты с vulnerability

#npm i --package-lock-only
проинсталлить только package.lock (нужно для npm audit)

#npm show
 npm view __package_name__ versions  --json //посмотреть все версии пакета

#npm config
npm config set package-lock false - удалить package.lock глобально

#npm commands
npm s имя_того_что_ищу - поиск модулей
npm i имя_модуля - инсталляция модуля, чтобы проинсталлить конкретную версию делаю так npm i имя_модуля@версия_модуля
npm -g i express - поставить модуль глобально
npm up имя_модуля - апдейт модуля всех модулей если не указывать конкретный
npm r имя_модуля - удалить модуль

# Чтобы опубликовать модуль npm
npm init (создает package.json)
npm adduser
npm publish
npm unpublish

#tilda and caret
~ - будет грузить 1.2.3 вместо 1.2.2 
^ -  1.3.2 вместо 1.2.2

#чтобы исправить ошибку гит
git config --global url."https://github.com/".insteadOf git@github.com:
git config --global url."https://".insteadOf git://

git config --system core.longpaths true

#npm repo (Чтобы посмотреть проект на гитхаб)
npm repo имя_пакета

#npm list (Посмотреть версии пакетов)
npm list --depth=0

#npm uninstall
npm uninstall имя_пакета

#Обновить npm
npm install npm@latest -g

#Посмотреть устаревшие модули
npm outdated

#Обновить все пакеты
$ npm install -g npm-check-updates
$ npm-check-updates -u
$ npm install 
ncu -a (проапдейтить package.json)
