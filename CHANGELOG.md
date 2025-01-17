# POS API 1.0 Changelog
Изменения в POS API 1.0 будут описаны в данном документе.

### 01-04-2022
### Добавлено
- Поле `onTap` в сущности 'Товар'
- Ошибки [16011, 16012, 16013, 16014, 16015, 16113, 16103, 16104, 16105]

## 10-03-2022
### Добавлено
- Описание нового типа маркированной продукции(Никотиносодержащая продукция) в `Товарах` и `Комплектах`.

## 30-09-2021
### Добавлено
- Описание новых типов маркированной продукции(Упакованная вода) в `Товарах` и `Комплектах`.

## 27-07-2021
### Добавлено
- Поле `markingSellingMode` в сущность `Точка продаж`.

## 26-07-2021
### Добавлено
 - Поля `useParentVat` и `vatEnabled` в `Товары`
 - Поле `vatEnabled` в позиции `Заказа`, `Продажи`, `Возврата`, `Предоплаты`, `Возврата предоплаты`
 - Ошибки `16010` и `17021`

## 06-05-2021
### Добавлено
 - Входящий параметр `preferredBonusToSpend` в запрос `Расчет скидок для продажи`.

## 05-05-2021
### Добавлено
- Описание новых типов маркированной продукции в `Товарах` и `Комплектах`.

## 12-04-2021
### Исправлено
 - Исправлена структура ошибки.

## 01-04-2021
### Добавлено
 - Описание эндопоинтов для создания операций на фискализацию.

## 02-03-2021
### Добавлено
 - Поле `partialDisposal` в сущность `Товары`.

## 02-02-2021
### Добавлено
- Флаг поиска покупателей во внешней системе лояльности в информации о точке продажи

## 26-11-2020
### Добавлено
 - Поля `externalOperationId` и `authCode` в объект `qrTransaction` в сущностях `Продажа`, `Возврат`, `Предоплата`, `Возврат предоплаты`.

## 12-11-2020
### Добавлено
- Поле `tobaccoMrcControlType` в сущность `Точка продаж`.

## 15-10-2020
### Добавлено
 - Описание новых типов маркированной продукции(Шины и покрышки, Альтернативаня табачная продукция) в `Товарах` и `Комплектах`.

## 28-09-2020
### Добавлено
 - Описание новых типов маркированной продукции в `Товарах` и `Комплектах`.

## 23-09-2020
### Добавлено
 - Поля `qrPayEnabled` и `qrAcquire` в сущность `Точка продаж`.
 - Поля `qrSum`, `qrTransaction` в сущности `Возврат`, `Предоплата`, `Возврат предоплаты`.
 - Поля `qrSum`, `prepaymentQrSum`, `qrTransaction` в сущность `Продажа`.
 - Поля `qrSum` и `prepaymentQrSum` в сущность `Розничные операции`.
 - Поле `paidByQr`в сущность `Заказы покупателей`.
 - Ошибки `18005`, `18006`, `19003` и `19004`.
### Изменено
 -  Текст ошибки `18000`.

## 01-09-2020
### Добавлено
 - Описание новых типов маркированной продукции в `Товарах` и `Комплектах`.

## 08-07-2020
### Добавлено
 - Поле `ppeType` (код средства идндивидуальной защиты) в сущность `Товары`.

## 26-04-2020
### Изменено
 - Формулировка об ограничении по запросу на один ip
 
## 04-03-2020
### Добавлено
- Коды маркировки в позициях возврата продажи

## 28-02-2020
### Добавлено
- новый код ошибки аутентификации 12025

## 27-01-2020
### Добавлено
- Коды маркировки в позициях розничной продажи

## 31-10-2019
### Добавлено
- Адрес электронной почты кассира в ответе на запрос информации о точке продаж

## 15-10-2019
### Добавлено
- Смена на которой была фискализирована операция с датой открытия и закрытия в ответе на запрос истории операций
- Смена на которой была фискализирована операция с датой открытия и закрытия в ответе на запрос по ID операций
- Название точки продаж в ответе на запрос по ID операций
- Тип формирования чеков в настройки точки продаж
- Создание розничных операций, которые подлежат облачной фискализации
- Работы с очередью фискализации

### Изменено
- Создание возвратов из продаж от другой точки продаж
- Обновление розничных операций теперь доступно

### Удалено
- Ошибка 12019 (Ошибка сохранения возврата: невозможно создать возврат продажи другой точки продаж)

### Исправлено
- Передача СНО в возвратах продаж и возвратах предоплат при запросе по ID