---
author: "Vladimir Lebedev"
date: 2019-06-18
linktitle: Tech Report 20190618
title: "Технический отчет, 3 июня - 17 июня"
description: "Сообщение команды разработчиков о результатах за прошлый спринт и о запланированных действиях на следующий."
metaTitle: "Технический отчет, 3 июня - 17 июня"
metaDescription: "Сообщение команды разработчиков о результатах за прошлый спринт и о запланированных действиях на следующий."
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "отчет", "технология"]
weight: 7
draft: false
---

## Сделано за Спринт 18
- Реализована базовая функциональность приложения для десктопа с графическим пользовательским интерфейсом: реализация визуализации начальной загрузки, счетов и платежей
- Создана история платежей и платежные сертификаты в кошельке, необходимые для поддержки отображения истории платежей в кошельке
- Повышена безопасность Docker image
- Введены переменные комиссии в транзакциях, установлена возможность устанавливать произвольную сумму комиссии за транзакцию, в целях увеличения шансов транзакции быть включенной в ближайший блок
- Внедрено использование Base58 для внешнего представления открытых ключей кошелька (адресов), что обеспечивает более удобное кодирование адресов
- Реализованы вебсокеты авторизации в API
- Обеспечена возможность изменения пароля кошелька самому пользователю
- Проведено стресс-тестирование на большом количестве узлов
- Разделен выход журнала и CLI: приложение CLI отделено от двоичного узла
- Ускорены подписи BLS: время проверки подписи BLS было уменьшено с 200 мс до 5 мс за подпись

## Планы на Спринт 19
- Стресс-тестирование: задержка и потеря пакетов
- Стресс-тестирование: блокчейн, консенсус, сервисные премии, обрезка (Slashing), ValueShuffle, стресс-тестирование других жизненно важных подсистем с использованием транзакционных нагрузок от генератора транзакций
