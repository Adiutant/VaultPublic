# VaultPublic
## Этот проект в статусе alpha pre-release. 
Это значит, что его можно запустить без dev-окружения
Технологический стек -  Qt5 C++ Kotlin?
## Менеджер паролей.
Этот проект представляет собой менеджер паролей, главной фичей которого является настройка шифрования и безопасности. Кроме того, файл паролей хранится на облаке пользователя (Яндекс Диск), а не на сервере разработчика, что позволяет деверсифицировать риски.
## Использование
Выбор удаленного хранилища.

![image](https://github.com/Adiutant/VaultPublic/assets/17684112/c5b020bc-7dd5-4469-828b-a061a39c65be)

Подключение удаленного хранилища с помощью авторизации в бразузере.

![image](https://github.com/Adiutant/VaultPublic/assets/17684112/4ea250eb-9423-4939-81ca-4d78659891ff)

После создания мастер-пароля, можно добавлять аккаунты, которые будут сохранены.
Программа сворачивается в трей и при выборе аккаунта из трея, пароль попадает в буфер обмена. Из трея можно закрыть хранилище.
## Tech
Программа использует продвинутые способы шифрования. Шифрование паролей производится с помощью AES-256, используя мульти-инициализирующие векторы. Хэширование мастер-пароля производится совместным использованием scrypt и SHA-256.
OAuth2 ключи к Yandex тоже шифруются дополнительным паролем.
## Todo
- [x] Выполнить рефакторинг
- [x] Сделать сборку для linux и дебианизировать ее
- [ ] Адаптировать идею проекта под андроид-реализацию
- [ ] Добавить настройку шифрования под несколько алгоритмов
