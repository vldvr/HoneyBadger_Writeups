# HoneyBadger CTF — Writeups

Разборы задач с **HoneyBadger CTF (Avito Tech, 2026)**.
Команда **YashaLava**, автор — [@wkiseven](https://github.com/vldvr).

Каждый разбор — не пошаговый лог «нашёл флаг», а разбор первопричины:
почему баг существует, как складывается эксплойт и как это чинится.

## Задачи

| Задача | Категория | Сложность | Что внутри |
|---|---|---|---|
| [OnMute](./OnMute.md) | Web · JavaScript | Medium | RegExp `lastIndex` desync — переиспользуемый глобальный regex ломает фильтр контента и открывает доступ к оригинальным текстам |
| [МёдХантер I](./Medhunter_I.md) | Web · Cloud | Easy | SSRF → метаданные Yandex Cloud → чтение cloud-init user-data с секретами в plaintext |

## Стек и приёмы

`SSRF` · `IMDS / cloud metadata` · `stored logic bugs` · `JS RegExp state` · `Go json.Unmarshal error reflection`
