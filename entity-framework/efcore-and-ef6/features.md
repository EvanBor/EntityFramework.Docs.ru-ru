---
title: "Сравнение возможностей EF Core и EF6"
author: rowanmiller
ms.author: divega
ms.date: 10/27/2016
ms.assetid: f22f29ef-efc0-475d-b0b2-12a054f80f95
uid: efcore-and-ef6/features
ms.openlocfilehash: 3f05fbe53439826a4e1e1b188a7c03951dc109ec
ms.sourcegitcommit: b2d94cebdc32edad4fecb07e53fece66437d1b04
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2018
---
# <a name="ef-core-and-ef6-feature-by-feature-comparison"></a>Сравнительный анализ возможностей EF Core и EF6

В следующей таблице представлено сравнение возможностей, доступных в EF Core и EF6. Анализ выполняется на самом обобщенном уровне, здесь не перечисляются все доступные возможности и нет подробных сведений о всех возможных различия в реализациях каждой функции.

Столбец EF Core содержит номер версии продукта, в котором эта возможность появилась впервые.

| **Создание модели**                                  | **EF 6** | **EF Core**                           |
|:------------------------------------------------------|:---------|:--------------------------------------|
| Сопоставление базовых классов                                   | Да      | 1.0                                   |
| Конструкторы с параметрами                          |          | 2.1                                   |
| Преобразования значений свойств                            |          | 2.1                                   |
| Сопоставленные типы без ключей (типы запросов)               |          | 2.1                                   |
| Соглашения                                           | Да      | 1.0                                   |
| Соглашения об именовании                                    | Да      | 1.0 (частично)                         |
| Заметки к данным                                      | Да      | 1.0                                   |
| Текучий API                                            | Да      | 1.0                                   |
| Наследование: одна таблица на иерархию (TPH)                | Да      | 1.0                                   |
| Наследование: одна таблица на тип (TPT)                     | Да      |                                       |
| Наследование: одна таблица на конкретный класс (TPC)           | Да      |                                       |
| Теневые свойства состояния                               |          | 1.0                                   |
| Альтернативные ключи                                        |          | 1.0                                   |
| Многие ко многим без сущности соединения                      | Да      |                                       |
| Создание ключей в базе данных                              | Да      | 1.0                                   |
| Создание ключей на стороне клиента                                |          | 1.0                                   |
| Сложные и принадлежащие типы                                   | Да      | 2.0                                   |
| Пространственные данные                                          | Да      |                                       |
| Графическое представление модели                      | Да      |                                       |
| Графический редактор моделей                                | Да      |                                       |
| Формат модели: код                                    | Да      | 1.0                                   |
| Формат модели: EDMX (XML)                              | Да      |                                       |
| Создание модели из базы данных с помощью командной строки              | Да      | 1.0                                   |
| Создание модели из базы данных с помощью мастера VS                 | Да      |                                       |
| Обновление модели из базы данных                            | Partial  |                                       |
| Глобальные фильтры запросов                                  |          | 2.0                                   |
| Разбиение таблиц                                       | Да      | 2.0                                   |
| Разбиение сущностей                                      | Да      |                                       |
| Сопоставление скалярных функций базы данных                      | Плохо     | 2.0                                   |
| Сопоставление полей                                         |          | 1.1                                   |
|                                                       |          |                                       |
| **Запросы к данным**                                     | **EF6**  | **EF Core**                           |
| Запросы LINQ                                          | Да      | 1.0 (ожидается для сложных запросов) |
| Создание удобного для чтения кода SQL                                | Плохо     | 1.0                                   |
| Смешанное вычисление на клиенте и сервере                        |          | 1.0                                   |
| Преобразование оператора GroupBy                                   | Да      | 2.1                                   |
| Загрузка связанных данных: безотложная                           | Да      | 1.0                                   |
| Загрузка связанных данных: безотложная загрузка для производных типов |          | 2.1                                   |
| Загрузка связанных данных: отложенная                            | Да      | 2.1                                   |
| Загрузка связанных данных: явная                        | Да      | 1.1                                   |
| Необработанные SQL-запросы: типы сущностей                         | Да      | 1.0                                   |
| Необработанные SQL-запросы: отличные от сущностей типы (например, типы запросов)  | Да      | 2.1                                   |
| Необработанные запросы SQL: создание с помощью LINQ                  |          | 1.0                                   |
| Явным образом скомпилированные запросы                           | Плохо     | 2.0                                   |
| Язык текстовых запросов (например, Entity SQL)           | 1.0      |                                       |
|                                                       |          |                                       |
| **Сохранение данных**                                       | **EF6**  | **EF Core**                           |
| Отслеживание изменений по моментальному снимку                             | Да      | 1.0                                   |
| Отслеживание изменений по извещениям                         | Да      | 1.0                                   |
| Отслеживание изменений: прокси-серверы                              | Да      |                                       |
| Доступ к отслеживаемому состоянию                               | Да      | 1.0                                   |
| Оптимистическая блокировка                                | Да      | 1.0                                   |
| Транзакции                                          | Да      | 1.0                                   |
| Пакетная обработка инструкций                                |          | 1.0                                   |
| Сопоставление хранимых процедур                              | Да      |                                       |
| Низкоуровневые API для несвязных графов                     | Плохо     | 1.0                                   |
| Полный проход несвязных графов                         |          | 1.0 (частично)                         |
|                                                       |          |                                       |
| **Другие возможности**                                    | **EF6**  | **EF Core**                           |
| Миграции                                            | Да      | 1.0                                   |
| Интерфейсы API для создания и удаления баз данных                       | Да      | 1.0                                   |
| Начальное значение данных                                             | Да      | 2.1                                   |
| Устойчивость подключений                                 | Да      | 1.1                                   |
| Обработчики жизненного цикла (события, перехват)                | Да      |                                       |
| Простое ведение журналов (например, Database.Log)                    | Да      |                                       |
| Создание пулов DbContext                                     |          | 2.0                                   |
|                                                       |          |                                       |
| **Поставщики баз данных**                                | **EF6**  | **EF Core**                           |
| SQL Server                                            | Да      | 1.0                                   |
| MySQL                                                 | Да      | 1.0                                   |
| PostgreSQL                                            | Да      | 1.0                                   |
| Oracle                                                | Да      | 1.0 <sup>(1)</sup>                    |
| SQLite                                                | Да      | 1.0                                   |
| SQL Server Compact                                    | Да      | 1.0 <sup>(2)</sup>                    |
| DB2                                                   | Да      | 1.0                                   |
| Firebird                                              | Да      | 2.0                                   |
| Jet (Microsoft Access)                                |          | 2.0 <sup>(2)</sup>                    |
| В памяти (для тестирования)                               |          | 1.0                                   |
|                                                       |          |                                       |
| **Платформы**                                         | **EF6**  | **EF Core**                           |
| .NET framework (консоль, WinForms, WPF, ASP.NET)      | Да      | 1.0                                   |
| .NET Core (консоль, ASP.NET Core)                     |          | 1.0                                   |
| Mono и Xamarin                                        |          | 1.0 (ожидается)                     |
| UWP                                                   |          | 1.0 (ожидается)                     |

<sup>1</sup> На данный момент доступен платный поставщик. Идет разработка бесплатного официального поставщика для Oracle.
<sup>2</sup> Этот поставщик работает только в .NET Framework (не в .NET Core).
