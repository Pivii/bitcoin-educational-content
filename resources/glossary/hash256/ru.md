---
term: HASH256

---
Криптографическая функция, используемая для различных приложений в Bitcoin. Она предполагает двойное применение функции SHA256 к входным данным. Сообщение проходит через SHA256 один раз, а результат этой операции используется в качестве входных данных для второго прохождения через SHA256. Таким образом, на выходе получается 256 бит.

$$\text{HASH256}(x) = \text{SHA256}(\text{SHA256}(x))$$