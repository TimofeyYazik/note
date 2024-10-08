Вот таблица с основными алгоритмами и их асимптотическими характеристиками (в лучшем, среднем и худшем случаях):

| Алгоритм                                        | Лучший случай    | Средний случай   | Худший случай    |
| ----------------------------------------------- | ---------------- | ---------------- | ---------------- |
| Сортировка                                      |                  |                  |                  |
| Быстрая сортировка                              | O(n log n)       | O(n log n)       | O(n²)            |
| Пирамидальная сортировка                        | O(n log n)       | O(n log n)       | O(n log n)       |
| Сортировка слиянием                             | O(n log n)       | O(n log n)       | O(n log n)       |
| Поразрядная сортировка                          | O(nk)            | O(nk)            | O(nk)            |
| Поиск                                           |                  |                  |                  |
| Линейный поиск                                  | O(1)             | O(n)             | O(n)             |
| Бинарный поиск                                  | O(1)             | O(log n)         | O(log n)         |
| Алгоритмы на графах                             |                  |                  |                  |
| Поиск в ширину (BFS)                            | O(V + E)         | O(V + E)         | O(V + E)         |
| Поиск в глубину (DFS)                           | O(V + E)         | O(V + E)         | O(V + E)         |
| Алгоритм Дейкстры                               | O(V + E log V)   | O(V + E log V)   | O(V + E log V)   |
| Алгоритм Флойда-Уоршелла                        | O(V³)            | O(V³)            | O(V³)            |
| Алгоритм Беллмана-Форда                         | O(VE)            | O(VE)            | O(VE)            |
| Динамическое программирование                   |                  |                  |                  |
| Алгоритм Кадане (максимальная сумма подмассива) | O(n)             | O(n)             | O(n)             |
| Задача о рюкзаке (0/1)                          | O(nW)            | O(nW)            | O(nW)            |
| Разное                                          |                  |                  |                  |
| Алгоритм Кнута-Морриса-Пратта (поиск подстроки) | O(n)             | O(n)             | O(n)             |
| Алгоритм Рабина-Карпа (поиск подстроки)         | O(n + m)         | O(n + m)         | O(nm)            |
| Быстрое возведение в степень                    | O(log n)         | O(log n)         | O(log n)         |
| Алгоритм Евклида (НОД)                          | O(log min(a, b)) | O(log min(a, b)) | O(log min(a, b)) |

**Примечания**:

- n - размер входных данных (например, длина массива или количество вершин в графе).
- V - количество вершин в графе.
- E - количество ребер в графе.
- k - количество разрядов в числе (для поразрядной сортировки).
- W - максимальная емкость рюкзака (для задачи о рюкзаке).
- m - размер подстроки (для алгоритмов поиска подстроки).

Эта таблица поможет понять временную сложность основных алгоритмов и выбрать подходящий алгоритм для решения конкретной задачи.