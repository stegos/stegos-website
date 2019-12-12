---
author: "Владимир Лебедев"
date: 2019-06-05
linktitle: Tech Report 20190606
title: "Технический отчет, 20 мая - 31 мая"
description: "Сообщение команды разработчиков о результатах за прошлый спринт и о запланированных действиях по запуску первого тестового релиза."
metaTitle: "Технический отчет, 20 мая - 31 мая"
metaDescription: "Сообщение команды разработчиков о результатах за прошлый спринт и о запланированных действиях по запуску первого тестового релиза."
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "отчет", "технология"]
weight: 8
draft: false
---

В течение последних двух недель наша команда разработчиков тщательно дорабатывала основные функции предстоящего выпуска тестовой сети Stegos.


Сделанное за период **20 мая — 31 мая**:


## Сделано в спринте 17

- Ускорение загрузки узла и повторной синхронизации, точная настройка констант загрузки

- Служебные вознаграждения, необходимые для создания стимула для валидаторов быть в сети

- Сжатие микроблоков в макроблоки, удаление микроблоков последней \"эпохи\", перемещение их данных в один макроблок

- Оптимизация bulletproofs, проверка bulletproofs теперь составляет 10 мс (без оптимизации AVX)

- HashCash: исправление ошибок

- Разрешение проблемы \"вилки\": исправление ошибок, в том числе в механизме решения \"вилки\" для микроблоков

- UTXO Timestamp Locking, реализация блокировки конкретных выходов

- PublicPaymentUTXO: дополнительные правила проверки tx, внедрение дополнительных правил проверки транзакций для транзакций с участием публичных платежей UTXOs

- PublicPaymentUTXO: реализация поддержки использования публичных платежей UTXOs в кошельке

## Запланировано на спринт 18

- Базовая функциональность настольного приложения GUI Wallet, визуализация начальной загрузки, счетов и платежей

- Повышение безопасности Docker image

- Введение возможности устанавливать произвольную сумму комиссии за транзакцию, в целях увеличения шанса транзакции быть включенной в ближайший блок

- Сохранение истории платежей и платежных сертификатов в кошельке для поддержки их отображения в кошельке

- Использование Base58 для внешнего представления открытых ключей кошелька (адресов) для более удобного кодирования адресов

- Реализация авторизации WebSocket API, в том числе на localhost

- Поддержка возможности пользователя изменить пароль кошелька

- Стресс-тестирование задержки и потери пакетов

- Стресс-тестирование на большом количестве узлов

- Стресс-тестирование: блокчейн, консенсус, служебные вознаграждения, Slashing, ValueShuffle, тестирование других жизненно важных подсистем с использованием транзакционных нагрузок от генератора транзакций