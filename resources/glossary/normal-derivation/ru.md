---
term: НОРМАЛЬНОЕ ПРОИЗВОДНОЕ
---

Процесс генерации дочерних ключей в HD-кошельках. Нормальное производное использует публичный ключ родителя в качестве входных данных для функции `HMAC-SHA512`, что позволяет генерировать дочерние публичные ключи из публичного ключа родителя и кода цепочки родителя. Процесс включает в себя конкатенацию публичного ключа родителя и индекса меньше $2^{31}$, за которым следует применение `HMAC-SHA512` с кодом цепочки родителя. Результат делится на две части: первые 256 битов добавляются к приватному ключу родителя для получения дочернего приватного ключа, в то время как оставшиеся 256 битов формируют код цепочки дочернего элемента. Этот метод гарантирует, что расширенный публичный ключ может быть использован для вывода дочерних публичных ключей. В стандартном производном нормальное производное используется на всех уровнях вывода, начиная с глубины аккаунта. В нотации путей производных нормальное производное обозначается, когда есть только индекс без апострофа `'`.