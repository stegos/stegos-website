---
author: "Владимир Лебедев"
date: 2019-05-07
linktitle: Testnet 6 Release 20190507
title: "Тестовая сеть, релиз 6"
description: "Шестой релиз тестовой сети блокчейна Stegos."
metaTitle: "test"
metaDescription: "test"
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "отчет", "технология"]
weight: 7
draft: false
---

Примечания к релизу 6 тестовой сети Stegos

Stegos создает передовые технологии, которые защищают ваши секреты от посторонних глаз, чтобы вы чувствовали себя в безопасности.

Это шестой тестовый выпуск блокчейна Stegos. Изменения произведенные после [Testnet 5] (https://github.com/stegos/stegos/releases/tag/v0.5):

 - Добавлен вызов HashCash в протокол PubSub для ограничения атак типа "отказ в обслуживании"
 - Реализована упрощенная повторная ставка для отслеживания онлайн-статуса валидаторов
 - Реализовано восстановление кошелька с использованием фразы восстановления из 24 слов
 - Реализована защита кошелька паролем и шифрование ключей, хранящихся на диске
 - Обеспечено разделение 1 STG на 1 000 000 microSTG
 - Ограничено количество UTXO в транзакциях и блоках


Критическое изменение:

Выпуск тестовой сети в 6 релизе не полностью совместим с выпуском 5 релиза. Пожалуйста, сбросьте локальную базу данных, если вы обновляете предыдущую версию:

rm -rf database/


Изучите план проекта для получения дополнительной информации: https://github.com/stegos/stegos/wiki/project-plan#sprint15 .

Пожалуйста, присоединяйтесь к нам в Telegram, чтобы получить тестовые токены и дайте нам обратную связь: https://t.me/stegos4privacy .


Установка узла тестовой сети

64-разрядная версия Linux:

curl -L https://github.com/stegos/stegos/releases/download/v0.6/stegos-linux-x64 -o stegos
chmod a+x stegos
./stegos


macOS 64-bit:

curl -L https://github.com/stegos/stegos/releases/download/v0.6/stegos-macos-x64 -o stegos
chmod a+x stegos
./stegos

Сразу после запуска узел будет печатать много информационных сообщений с отладочной информацией относительно начальной загрузки вашего узла. Нажмите Enter, чтобы получить stegos. Для получения справки введите команду help в командной строке.
