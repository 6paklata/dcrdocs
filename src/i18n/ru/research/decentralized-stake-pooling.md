# Децентрализованный пул ставок 

---

Одна из проблем, возникших в предыдущих проектах PoS, состоит в том, как осуществить пул в PoS-майнинге, аналогичну пулу в PoW-майнинге.

Decred решает эту проблему, позволяя множественные входы в транзакцию покупки тикетов и пропорционально передавая в UTXO сумму субсидии для каждого входа, одновременно передавая на новый выход открытый ключ или скрипт для этих пропорциональных вознаграждений. Затем им предоставляется субсидия, генерируя билет в недоверительном порядке, и билет может быть подписан циклическим алгоритмом до подачи в сеть. Важно отметить, что контроль за производством самого vote предоставляется другому открытому ключу или скрипту, который не может манипулировать субсидией, предоставляемой получателям. Производство голосов распределенным способом может быть достигнуто с использованием скрипта в тикете, который позволяет множественных подписантов.