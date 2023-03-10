# Выявление факторов, влияющих на возврат заемщиками кредита в срок

[Ссылка на проект](https://nbviewer.org/github/anapon-DA/projects/blob/main/Factors%20Affecting%20Loan%20Repayment%20Performance/loan-repayment-factors.ipynb) :point_left:

Проект выполнен с применением морфологического анализатора русского языка (библиотека PyMystem3). Использована лемматизация.

Для кредитного отдела банка необходимо выяснить, влияет ли семейное положение и количество детей клиента на факт погашения кредита в срок. Входные данные от банка — статистика о платёжеспособности клиентов.

Результаты исследования нужны для построения модели кредитного скоринга.

Для анализа предоставлена таблица с информацией о клиентах.

**Описание данных (содержание столбцов таблицы)**

- `children` — количество детей в семье;
- `days_employed` — общий трудовой стаж в днях;
- `dob_years` — возраст клиента в годах;
- `education` — уровень образования клиента;
- `education_id` — идентификатор уровня образования;
- `family_status` — семейное положение;
- `family_status_id` — идентификатор семейного положения;
- `gender` — пол клиента;
- `income_type` — тип занятости;
- `debt` — имел ли задолженность по возврату кредитов;
- `total_income` — ежемесячный доход;
- `purpose` — цель получения кредита.

| [Рендер проекта на `nbviewer`](https://nbviewer.org/github/anapon-DA/projects/blob/main/Factors%20Affecting%20Loan%20Repayment%20Performance/loan-repayment-factors.ipynb) | [Проект на `github`](https://github.com/anapon-DA/projects/blob/main/Factors%20Affecting%20Loan%20Repayment%20Performance/loan-repayment-factors.ipynb) |
| --- | --- |
| **корректный переход по внутренним ссылкам в оглавлении проекта** | статичный вариант |

# Выводы

В ходе анализа были изучены, обработаны и категоризированы данные, что в итоге дало возможность найти взаимосвязи между возвратом кредита в срок и наличием детей, семейным положением, уровнем дохода, целями кредита:

- заемщики, у которых нет детей, возвращают кредит в срок чаще на 1.5 процентных пункта, чем те, у кого есть хотя бы один ребенок;

- реже всего кредит возвращают в срок клиенты, которые никогда не состояли в официально зарегистрированном браке, клиенты со средним доходом и те, кто брал кредит на автомобиль и на оплату образовательных услуг.

Кроме того, благодаря категоризации, возможен дальнейший поиск взаимосвязей (например, связь с образованием, типом занятости), которые можно использовать для построения моделей.

# Статус проекта

:white_check_mark: Завершен

# Инструменты

`Pandas`
`PyMystem3`
`Python`
