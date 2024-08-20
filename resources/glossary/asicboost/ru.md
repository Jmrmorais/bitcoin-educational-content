---
term: ASICBOOST
---

ASICBOOST - это метод алгоритмической оптимизации, изобретенный в 2016 году, предназначенный для увеличения эффективности майнинга Bitcoin примерно на 20% за счет сокращения количества вычислений, необходимых для каждой попытки хеширования заголовка. Эта техника использует особенность хеш-функции SHA256, применяемой для майнинга, которая делит данные на блоки перед их обработкой. ASICBOOST сохраняет один из этих блоков неизменным в течение множества попыток хеширования, позволяя майнеру выполнять работу по этому блоку только частично на протяжении нескольких попыток. Этот обмен данными позволяет повторно использовать результаты предыдущих вычислений, тем самым сокращая общее количество вычислений, необходимых для нахождения действительного хеша.

ASICBOOST может использоваться в двух формах: открытый ASICBOOST и скрытый ASICBOOST. Открытая форма ASICBOOST видна всем, поскольку она включает использование поля `nVersion` блока в качестве nonce и не изменяет реальный `Nonce`. Скрытая форма стремится скрыть эти модификации с помощью деревьев Меркла. Однако этот второй метод стал менее эффективным после введения SegWit из-за второго дерева Меркла, которое увеличивает количество вычислений, необходимых для его использования.

В итоге, ASICBOOST позволяет майнерам не выполнять полное хеширование SHA256 для всех попыток, поскольку часть результата остается неизменной, что ускоряет работу майнеров.