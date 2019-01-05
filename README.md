<h1 align="center">
<br>
  <a href="https://github.com/ForWhomTheBellTolls/SiAOD"><img src="https://i.imgur.com/2kPWwMA.png" alt="Криогенный мир дискретного анализа или как сделать умное лицо на экзамене по СиАОД" width=200"></a>
  <br>
    <br>
  Криогенный мир дискретного анализа или как сделать умное лицо на экзамене по СиАОД
  <br><br>
</h1>


## Вступление

**🚀 Ведущий и самый крупный в России вуз в областях подготовки высококвалифицированных специалистов по направлениям маркетолога и продавцам обуви задумал провести экзамен по структурам и алгоритмам на богоненавистном языке Крест СС, в качестве альтернативного выжигателя мозгов данный репозиторий предлагает вам изучить все то, чему вас нигде и никогда не научат. Шутка**

**🚀 Отдельное спасибо Леонадро ЭмЭсО за возможность воспользоваться репозиторием (https://github.com/leonardomso/)**

## Оглавление
---
1. **[В чем заключаются достоинства и недостатки последовательного и связанного способов реализации динамических структур данных?](#1-в-чем-заключаются-достоинства-и-недостатки-последовательного-и-связанного-способов-реализации-динамических-структур-данных)**
2. **[Назовите принципы функционирования стека, очереди и дека?](#2-primitive-types)**
3. **[Реализуйте класс – стек с базовым набором методов на основе массива нетипированных указателей на размещенные в динамической памяти элементы](#3-value-types-and-reference-types)**
4. **[С использованием основных методов работы со стеком составьте программу копирования элементов стека в новый стек в том же порядке](#4-implicit-explicit-nominal-structuring-and-duck-typing)**
5. **[Реализуйте метод копирования элементов очереди в новую очередь.](#5--vs--vs-typeof)**
6. **[Перевод из инфиксной формы записи выражения в префиксную](#6-function-scope-block-scope-and-lexical-scope)**
7. **[Перевод инфиксной формы записи выражения в постфиксную](#7-expression-vs-statement)**
8. **[С использованием стандартного набора методов составьте программу переноса из очереди строк в новую очередь элементов начинающихся на буквы «F» или «f»](#8-iife-modules-and-namespaces)**
9. **[С использованием стандартного набора методов составьте программу записи элементов очереди в новую очередь в обратном порядке](#9-message-queue-and-event-loop)**
10. **[АТД – очередь. Ее свойства. Способы реализации](#10-settimeout-setinterval-and-requestanimationframe)**
11. **[Разработать класс «Бинарное дерево поиска». Реализовать метод вставки нового узла в дерево](#11-javascript-engines)**
12. **[АТД Дек – это очередь с двумя вершинами: правой и левой, характеристика](#12-bitwise-operators-type-arrays-and-array-buffers)**
13. **[Класс «Бинарное дерево поиска». Реализуйте метод поиска элемента в дереве](#13-dom-and-layout-trees)**
14. **[АТД Очередь с приоритетом. Ее свойства. Способы реализации](#14-factories-and-classes)**
15. **[Класс Идеально сбалансированное бинарное дерево. Реализуйте алгоритм прямого обхода дерева в глубину](#15-this-call-apply-and-bind)**
16. **[АТД Стек. Свойства. Способы реализации](#16-new-constructor-instanceof-and-instances)**
17. **[Класс Хеш-таблица. Реализация коллизий – цепное хеширование. Реализуйте метод вставки в таблицу нового узла с проверкой коэффициента нагрузки таблицы и рехеширования](#17-prototype-inheritance-and-prototype-chain)**
18. **[АТД Линейный список. Свойства. Способы реализации.](#18-objectcreate-and-objectassign)**
19. **[Класс Бинарное дерево. Реализовать метод по алгоритму симметричного обхода дерева с выводом списка вершин (номеров вершин)](#19-map-reduce-filter)**
20. **[Инфиксная и постфиксная запись выражения. Алгоритм создания постфиксной записи арифметического выражения из инфиксной. Пример создания постфиксной записи арифметического выражения (схема преобразования)](#20-pure-functions-side-effects-and-state-mutation)**
21. **[Класс Бинарное дерево поиска. Реализовать метод удаления узла с наибольшим значением, учитывая все случаи](#21-closures)**
22. **[Класс Бинарное дерево. Реализуйте метод, который определяет количество узлов в дереве](#22-high-order-functions)**
23. **[АТД сильно ветвящееся дерево. Способы реализация. Алгоритмы обхода в глубину](#23-recursion)**
24. **[Класс Стек. Реализация методов: втолкнуть узел в стек, вытолкнуть узел из стека. Использование при вычислении значения арифметического выражения, содержащего скобки](#24-collections-and-generators)**
25. **[АТД AVL дерево. Свойства. Алгоритм балансировки дерева при правом повороте](#25-promises)**
26. **[АТД – объединение списков. Реализуйте АТД на линейной связанной структуре. Даны два линейных однонаправленных списка L и М. Где L {L1,L2,…..Lki } где 0<=i<=ki; и 0<=Li<=99, а М={M0, M1,…..Mkj} где 0<=j<=kj и 100<=Mj<=199. Объедините эти списки в один список LM={L0M0,L1M1….., LiMj….} где j>=i, а Li и Mj это два значения одного элемента списка LM](#26-asyncawait)**
27. **[Ориентированный взвешенный граф. Свойства ориентированного графа. Представление в памяти. Алгоритм Дейкстры – поиск кратчайшего пути](#27-data-structures)**
28. **[Класс - циклический линейный двунаправленный список. Реализуйте метод вставки нового узла в упорядоченный список так, чтобы упорядоченность не нарушилась](#28-expensive-operation-and-big-o-notation)**
29. **[Хеш-таблица. Применение. Коллизии. Подходы к реализации коллизий](#29-algorithms)**
30. **[Класс Линейный однонаправленный список. Реализовать метод удаления узла с заданным номером из списка](#30-inheritance-polymorphism-and-code-reuse)**
31. **[АТД очередь с приоритетом. Свойства. Способы реализации. Алгоритм вставки нового элемента в очередь с приоритетом.](#31-design-patterns)**
32. **[Класс Бинарное дерево поиска. Реализация дерева на связанной структуре хранении. Реализовать метод определения высоты дерева](#32-partial-applications-currying-compose-and-pipe)**
33. **[Класс Очередь. Представление в памяти на однонаправленном списк. Реализуйте метод вычисления значения выражения, заданного в префиксной форме](#33-clean-code)**
34. **[Дерево выражений. Свойства. Алгоритм формирования префиксной записи арифметического выражения](#34-clean-code)**
35. **[AVL дерево. Свойства. Алгоритм вставки нового узла в дерево](#35-clean-code)**
36. **[Класс Стек. Реализация на однонаправленном списке. Разработайте функцию для сложения двух целых чисел большой разрядности, представляя каждое число в объекте Стек](#36-clean-code)**
37. **[Линейный список - Очередь. АТД – очередь. Реализация очереди на связанном списке. Функции операций на вставки и удаления узлов очереди](#37-clean-code)**
38. **[Класс Двунаправленный список. Разработать метод, который определяет, симметричен ли список, т.е. элементы, отстоящие от левой и правой вершин на одинаковое расстояние равны](#38-clean-code)**
39. **[Класс Граф. Реализовать на матрице смежности. Реализовать поиск кратчайшего пути от одной заданной вершины к другой, используя матрицу Флойда](#39-clean-code)**
40. **[AVL дерево. Свойства. Алгоритм двойного поворота. Пример AVL дерева для балансировки которого требуется двойной поворот](#40-clean-code)**
41. **[Дана последовательность ключей 1,2,3,4,5,6,7,8,9. Постройте бинарное дерево минимальной высоты с такими ключами](#41-clean-code)**

---

### 1. В чем заключаются достоинства и недостатки последовательного и связанного способов реализации динамических структур данных?

В памяти компьютера данные могут иметь последовательное или связанное представление. Соответственно различают структуры хранения, использующие последовательное представление данных и связанное представление данных.

При последовательном представлении данные в памяти компьютера размещаются в соседних последовательно расположенных ячейках. При этом физический порядок следования записей полностью соответствует логическому порядку, определяемому логической структурой, то есть логическая структура поддерживается физическим порядком следования данных. Совокупность записей, размещенных в последовательно расположенных ячейках памяти, называют последовательным списком.
 	
При связанном представлении в каждой записи предусматривается дополнительное поле, в котором размещается указатель (ссылка). В памяти компьютера записи располагаются в любых свободных ячейках и связываются между собой указателями, указывающими на место расположения записи, логически следующей за данной. Структуры хранения, основанные на связанном представлении данных, называют связанными списками. Если каждая запись содержит лишь один указатель, то список односвязный, при большем числе указателей - список многосвязный.
 	
Контейнерные классы предназначены для хранения данных, организованных определенным образом. Для каждого типа контейнера определены методы работы с его элементами, не зависящие от конкретного типа данных, которые хранятся в контейнере. Поэтому один и тот же вид контейнера можно использовать для хранения данных различных типов. Возможность работы с контейнерными классами реализована с помощью стандартной библиотеки шаблонов (STL Standard Template Library), в которую входят контейнерные классы, алгоритмы и итераторы. Использование STL позволяет повысить надежность программ и уменьшить сроки их реализации. 

Контейнеры можно разделить на два типа: последовательные и ассоциативные. 
 * Последовательные контейнеры обеспечивают хранение конечного количества однотипных элементов в виде непрерывной последовательности. К последовательным контейнерам относятся: векторы (vector), двусторонние очереди (deque), списки (list), а также так называемые адаптеры (варианты контейнеров): стеки (stack), очереди (queue) и очереди с приоритетами (priority_queue). Каждый вид контейнера обеспечивает свой набор действий над данными и выбор того или иного контейнера зависит от того, что именно требуется делать с данными в программе.
 * Ассоциативные контейнеры обеспечивают быстрый доступ к данным по ключу. Такие контейнеры построены на основе сбалансированных деревьев. К ассоциативным контейнерам относятся: словари (map), словари с дубликатами (multiset), множества (set), множества с дубликатами (multiset) и битовые множества (bitset).

**[:arrow_up:Оглавление](#Оглавление)**

---
