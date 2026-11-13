# Баг-репорты (Bug Reports) – `intern-demoshopping` (Build 1.0)

В ходе функционального тестирования сборки `Build 1.0` выявлено и задокументировано **11 дефектов** с разным уровнем критичности (High: 6, Medium: 4, Low: 1). Все карточки дефектов содержат шаги воспроизведения, фактические и ожидаемые результаты.

---

## 📋 Реестр дефектов в Jira

> **Доступ:** Задачи открыты в режиме чтения (`Viewer`). Внутри каждой карточки доступны подробные описания, скриншоты/логи и связи с затронутыми User Stories.

| ID | Приоритет | Модуль / Заголовок дефекта                                                                                                         |                                                                Ссылка в Jira                                                                |
| :--- | :---: |:-----------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------:|
| **ID-10** | 🔴 High | [Регистрация] расхождение в отображении ошибок между UI и API при использовании валидного логина и пароля                          | [Открыть ID-10](https://artamkindima.atlassian.net/browse/ID-10?atlOrigin=eyJpIjoiY2FkMDRkMjU4ZmUxNGYwN2IyMTM2NGE1YjUwMmFhMDIiLCJwIjoiaiJ9) |
| **ID-11** | 🔴 High | [Регистрация] расхождение в отображении ошибок между UI и API при использовании невалидного логина                                 | [Открыть ID-11](https://artamkindima.atlassian.net/browse/ID-11?atlOrigin=eyJpIjoiN2VmNjNmNmIzZTI3NDQ0NTgzMDQ4NDgxYTJhYTQ2OWUiLCJwIjoiaiJ9) |
| **ID-12** | 🔴 High | [Регистрация] расхождение в отображении ошибок между UI и API при использовании уже зарегистрированного аккаунта                   | [Открыть ID-12](https://artamkindima.atlassian.net/browse/ID-12?atlOrigin=eyJpIjoiM2M1YmZkOWY0OTBhNDc5ZWI5N2U4Y2MwM2Y5MDQ0NmYiLCJwIjoiaiJ9) |
| **ID-13** | 🔴 High | [Авторизация] расхождение в отображении ошибок UI и API при использовании незарегистрированного логина                             |       [Открыть ID-13](https://artamkindima.atlassian.net/browse/ID-13?atlOrigin=eyJpIjoiYTEwNDU3NDZlZjFmNGJkNDg4YWExYWU4YzM4NGE1Y2MiLCJwIjoiaiJ9)                                       |
| **ID-14** | 🔴 High | [Авторизация] расхождение в отображении ошибок UI и API при использовании незарегистрированного пароля                             |         [Открыть ID-14](https://artamkindima.atlassian.net/browse/ID-14?atlOrigin=eyJpIjoiNmM0M2FiYzgwMDRhNDA0NWIwMDQ0NmQzZDhhMGIyY2UiLCJwIjoiaiJ9)                                       |
| **ID-15** | 🔴 High | [Выход из системы] страница отображает приватные данные пользователя при нажатии на кнопку "Назад" после выхода из системы         |      [Открыть ID-15](https://artamkindima.atlassian.net/browse/ID-15?atlOrigin=eyJpIjoiYjIzYTcxNmE3MGEyNDk4NDkxNWE2NzBkNjQ1MTkwMmQiLCJwIjoiaiJ9)                                       |
| **ID-16** | 🟡 Medium | [Проверка авторизации] неправильное перенаправление при нажатие на ссылку "войдите в систему" в сообщении о просьбе авторизоваться |       [Открыть ID-16](https://artamkindima.atlassian.net/browse/ID-16?atlOrigin=eyJpIjoiNDJjMjlkZDlmM2NhNGViOGFmZWY3N2ViYzEwMjVjMDAiLCJwIjoiaiJ9)                                       |
| **ID-17** | 🟡 Medium | [Карточка товара] отсутствие граничных значений для счётчика количества товаров                                                    |          [Открыть ID-17](https://artamkindima.atlassian.net/browse/ID-17?atlOrigin=eyJpIjoiZGNlMzc5NWNmYmEzNDFlZjk1M2M1NDdiYTljYjQ5NWYiLCJwIjoiaiJ9)                                       |
| **ID-18** | 🟢 Low | [Фильтрация] отсутствует уведомление об отсутствии товаров при фильтрации                                                          |        [Открыть ID-18](https://artamkindima.atlassian.net/browse/ID-18?atlOrigin=eyJpIjoiNmYzOTdlYmFkZDQwNDhiM2I5MjQ3YmU3ZGQxNjgyOGQiLCJwIjoiaiJ9)                                       |
| **ID-19** | 🟡 Medium | [Фильтрация] отсутствует валидация диапазона цен при вводе минимальной цены больше максимальной                                    |          [Открыть ID-19](https://artamkindima.atlassian.net/browse/ID-19?atlOrigin=eyJpIjoiYzk5MDM4ZTk0ZGY4NDI4YzkwYTlkYTJmNWUyNzliMTIiLCJwIjoiaiJ9)                                       |
| **ID-20** | 🟡 Medium | [Сортировка] некорректное отображение сортировки по цене возрастания и убыванию                                                    |                [Открыть ID-20](https://artamkindima.atlassian.net/browse/ID-20?atlOrigin=eyJpIjoiZTA3MzA5N2ZlN2VjNDUwNzgxYjk5ZTYzZmJkYTA0OGQiLCJwIjoiaiJ9)                                       |

---

## 🔗 Дополнительно
- **Общий фильтр всех дефектов в Jira:** [Смотреть полный список дефектов](https://artamkindima.atlassian.net/jira/software/projects/ID/list?jql=project+%3D+ID+AND+type+%3D+Bug+ORDER+BY+cf%5B10019%5D+ASC&atlOrigin=eyJpIjoiNTU5MDNkMjYzNGQ3NDNhZDljMmY2NmYwOTZhODQxMWEiLCJwIjoiaiJ9&xpis=eyJicmlkZ2UiOiJzbWFydExpbmtzIiwiaWQiOiIxNzk0NTcwOTE0Mzk2Iiwic291cmNlIjoiY29uZmx1ZW5jZSJ9)
- **Итоговый анализ влияния дефектов на релиз:** см. [Итоговый отчёт](../06_Test_Summary_Report/)