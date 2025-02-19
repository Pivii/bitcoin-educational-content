---
term: P2SH-P2WPKH

---
P2SH-P2WPKH расшифровывается как *Pay to Script Hash - Pay to Witness Public Key Hash*. Это стандартная модель скриптов, используемая для создания условий расходования средств на UTXO, также известная как "вложенный SegWit".

P2SH-P2WPKH был представлен с внедрением SegWit в августе 2017 года. Этот скрипт представляет собой P2WPKH, обернутый в P2SH. Он блокирует биткоины на основе хэша публичного ключа. Отличие от классического P2WPKH заключается в том, что скрипт обернут в `redeemScript` классического P2SH.

Этот скрипт был создан во время запуска SegWit, чтобы облегчить его принятие. Он позволяет использовать этот новый стандарт даже с сервисами или кошельками, еще не совместимыми с SegWit. Это своего рода переходный скрипт к новому стандарту. На сегодняшний день использование подобных скриптов с оберткой SegWit уже неактуально, так как большинство кошельков реализовали нативный SegWit. Адреса P2SH-P2WPKH записываются с использованием кодировки `Base58Check` и всегда начинаются с `3`, как и любой другой P2SH-адрес.

> ► *`P2SH-P2WPKH` также иногда называют `P2WPKH-вложенный в-P2SH`.*