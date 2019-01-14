<h1 align="center">
<br>
  <a href="https://github.com/ForWhomTheBellTolls/SiAOD"><img src="https://i.imgur.com/2kPWwMA.png" alt="Cryogenic World of Non-Slavish Devotion by Unchained Heroes" width=300"></a>
  <br>
    <br>
  Cryogenic World of Non-Slavish Devotion by Unchained Heroes
    <br><br>
  </h1>

## Вступление

**:feelsgood: Ведущий и самый крупный в России вуз в областях подготовки высококвалифицированных специалистов по направлениям маркетолога и продавцам обуви задумал провести экзамен по структурам и алгоритмам на богоненавистном языке Крест СС, в качестве альтернативного выжигателя мозгов данный репозиторий предлагает вам изучить все то, чему вас нигде и никогда не научат.**

**🚀 Отдельное спасибо [Leonardo Maldonado](https://github.com/leonardomso/) и [Björn Fahller](https://github.com/rollbear) за возможность воспользоваться репозиториями**

**:small_orange_diamond:  [Краткий экскурс по некоторым АТД и алгоритмам](http://www.mkurnosov.net/teaching/index.php/DSA/Spring2016)**
<br>**:small_orange_diamond:  [Теоретическая основа для всех последующих реализаций деревьев](https://www.bogotobogo.com/cplusplus/binarytree.php)** 
<br>**:small_orange_diamond:  [Тыц к 22-ому](#22-класс-бинарное-дерево-реализуйте-метод-который-определяет-количество-узлов-в-дереве)**
### Оглавление
1. **[В чем заключаются достоинства и недостатки последовательного и связанного способов реализации динамических структур данных?](#1-в-чем-заключаются-достоинства-и-недостатки-последовательного-и-связанного-способов-реализации-динамических-структур-данных)**
2. **[Назовите принципы функционирования стека, очереди и дека](#2-назовите-принципы-функционирования-стека-очереди-и-дека)**
3. **[Реализуйте класс – Стек с базовым набором методов на основе массива нетипированных указателей на размещенные в динамической памяти элементы](#3-реализуйте-класс--стек-с-базовым-набором-методов-на-основе-массива-нетипированных-указателей-на-размещенные-в-динамической-памяти-элементы)**
4. **[С использованием основных методов работы со стеком составьте программу копирования элементов стека в новый стек в том же порядке](#4-с-использованием-основных-методов-работы-со-стеком-составьте-программу-копирования-элементов-стека-в-новый-стек-в-том-же-порядке)**
5. **[Реализуйте метод копирования элементов очереди в новую очередь](#5-реализуйте-метод-копирования-элементов-очереди-в-новую-очередь)**
6. **[Перевод из инфиксной формы записи выражения в префиксную](#6-перевод-из-инфиксной-формы-записи-выражения-в-префиксную)**
7. **[Перевод инфиксной формы записи выражения в постфиксную](#7-перевод-инфиксной-формы-записи-выражения-в-постфиксную)**
8. **[С использованием стандартного набора методов составьте программу переноса из очереди строк в новую очередь элементов начинающихся на буквы «F» или «f»](#8-с-использованием-стандартного-набора-методов-составьте-программу-переноса-из-очереди-строк-в-новую-очередь-элементов-начинающихся-на-буквы-f-или-f)**
9. **[С использованием стандартного набора методов составьте программу записи элементов очереди в новую очередь в обратном порядке](#9-с-использованием-стандартного-набора-методов-составьте-программу-записи-элементов-очереди-в-новую-очередь-в-обратном-порядке)**
10. **[АТД – очередь. Ее свойства. Способы реализации](#10-атд--очередь-ее-свойства-способы-реализации)**
11. **[Разработать класс «Бинарное дерево поиска». Реализовать метод вставки нового узла в дерево](#11-разработать-класс-бинарное-дерево-поиска-реализовать-метод-вставки-нового-узла-в-дерево)**
12. **[АТД Дек – это очередь с двумя вершинами: правой и левой, характеристика](#12-атд-дек--это-очередь-с-двумя-вершинами-правой-и-левой-характеристика)**
13. **[Класс «Бинарное дерево поиска». Реализуйте метод поиска элемента в дереве](#13-класс-бинарное-дерево-поиска-реализуйте-метод-поиска-элемента-в-дереве)**
14. **[АТД Очередь с приоритетом. Ее свойства. Способы реализации](#14-атд-очередь-с-приоритетом-ее-свойства-способы-реализации)**
15. **[Класс Идеально сбалансированное бинарное дерево. Реализуйте алгоритм прямого обхода дерева в глубину](#15-класс-идеально-сбалансированное-бинарное-дерево-реализуйте-алгоритм-прямого-обхода-дерева-в-глубину)**
16. **[АТД Стек. Свойства. Способы реализации](#16-атд-стек-свойства-способы-реализации)**
17. **[Класс Хеш-таблица. Реализация коллизий – цепное хеширование. Реализуйте метод вставки в таблицу нового узла с проверкой коэффициента нагрузки таблицы и рехеширования](#17-класс-хеш-таблица-реализация-коллизий--цепное-хеширование-реализуйте-метод-вставки-в-таблицу-нового-узла-с-проверкой-коэффициента-нагрузки-таблицы-и-рехеширования)**
18. **[АТД Линейный список. Свойства. Способы реализации](#18-атд-линейный-список-свойства-способы-реализации)**
19. **[Класс Бинарное дерево. Реализовать метод по алгоритму симметричного обхода дерева с выводом списка вершин (номеров вершин)](#19-класс-бинарное-дерево-реализовать-метод-по-алгоритму-симметричного-обхода-дерева-с-выводом-списка-вершин-номеров-вершин)**
20. **[<span id="20">Инфиксная и постфиксная запись выражения. Алгоритм создания постфиксной записи арифметического выражения из инфиксной. Пример создания постфиксной записи арифметического выражения (схема преобразования)</span>](#20-инфиксная-и-постфиксная-запись-выражения-алгоритм-создания-постфиксной-записи-арифметического-выражения-из-инфиксной-пример-создания-постфиксной-записи-арифметического-выражения-схема-преобразования)**
21. **[Класс Бинарное дерево поиска. Реализовать метод удаления узла с наибольшим значением, учитывая все случаи](#21-класс-бинарное-дерево-поиска-реализовать-метод-удаления-узла-с-наибольшим-значением-учитывая-все-случаи)**
22. **[Класс Бинарное дерево. Реализуйте метод, который определяет количество узлов в дереве](#22-класс-бинарное-дерево-реализуйте-метод-который-определяет-количество-узлов-в-дереве)**
23. **[АТД сильно ветвящееся дерево. Способы реализации. Алгоритмы обхода в глубину](#23-атд-сильно-ветвящееся-дерево-способы-реализации-алгоритмы-обхода-в-глубину)**
24. **[Класс Стек. Реализация методов: втолкнуть узел в стек, вытолкнуть узел из стека. Использование при вычислении значения арифметического выражения, содержащего скобки](#24-класс-стек-реализация-методов-втолкнуть-узел-в-стек-вытолкнуть-узел-из-стека-использование-при-вычислении-значения-арифметического-выражения-содержащего-скобки)**
25. **[АТД AVL дерево. Свойства. Алгоритм балансировки дерева при правом повороте](#25-атд-avl-дерево-свойства-алгоритм-балансировки-дерева-при-правом-повороте)**
26. **[АТД – объединение списков. Реализуйте АТД на линейной связанной структуре. Даны два линейных однонаправленных списка L и М. Где L {L1,L2,…..Lki } где 0<=i<=ki; и 0<=Li<=99, а М={M0, M1,…..Mkj} где 0<=j<=kj и 100<=Mj<=199. Объедините эти списки в один список LM={L0M0,L1M1….., LiMj….} где j>=i, а Li и Mj это два значения одного элемента списка LM](#26-атд--объединение-списков-реализуйте-атд-на-линейной-связанной-структуре-даны-два-линейных-однонаправленных-списка-l-и-м-где-l-l1l2lki--где-0iki-и-0li99-а-мm0-m1mkj-где-0jkj-и-100mj199-объедините-эти-списки-в-один-список-lml0m0l1m1-limj-где-ji-а-li-и-mj-это-два-значения-одного-элемента-списка-lm)**
27. **[Ориентированный взвешенный граф. Свойства ориентированного графа. Представление в памяти. Алгоритм Дейкстры – поиск кратчайшего пути](#27-ориентированный-взвешенный-граф-свойства-ориентированного-графа-представление-в-памяти-алгоритм-дейкстры--поиск-кратчайшего-пути)**
28. **[Класс - циклический линейный двунаправленный список. Реализуйте метод вставки нового узла в упорядоченный список так, чтобы упорядоченность не нарушилась](#28-класс---циклический-линейный-двунаправленный-список-реализуйте-метод-вставки-нового-узла-в-упорядоченный-список-так-чтобы-упорядоченность-не-нарушилась)**
29. **[Хеш-таблица. Применение. Коллизии. Подходы к реализации коллизий](#29-хеш-таблица-применение-коллизии-подходы-к-реализации-коллизий)**
30. **[Класс Линейный однонаправленный список. Реализовать метод удаления узла с заданным номером из списка](#30-класс-линейный-однонаправленный-список-реализовать-метод-удаления-узла-с-заданным-номером-из-списка)**
31. **[АТД очередь с приоритетом. Свойства. Способы реализации. Алгоритм вставки нового элемента в очередь с приоритетом](#31-атд-очередь-с-приоритетом-свойства-способы-реализации-алгоритм-вставки-нового-элемента-в-очередь-с-приоритетом)**
32. **[Класс Бинарное дерево поиска. Реализация дерева на связанной структуре хранении. Реализовать метод определения высоты дерева](#32-класс-бинарное-дерево-поиска-реализация-дерева-на-связанной-структуре-хранении-реализовать-метод-определения-высоты-дерева)**
33. **[Класс Очередь. Представление в памяти на однонаправленном списк. Реализуйте метод вычисления значения выражения, заданного в префиксной форме](#33-класс-очередь-представление-в-памяти-на-однонаправленном-списк-реализуйте-метод-вычисления-значения-выражения-заданного-в-префиксной-форме)**
34. **[Дерево выражений. Свойства. Алгоритм формирования префиксной записи арифметического выражения](#34-дерево-выражений-свойства-алгоритм-формирования-префиксной-записи-арифметического-выражения)**
35. **[AVL дерево. Свойства. Алгоритм вставки нового узла в дерево](#35-avl-дерево-свойства-алгоритм-вставки-нового-узла-в-дерево)**
36. **[Класс Стек. Реализация на однонаправленном списке. Разработайте функцию для сложения двух целых чисел большой разрядности, представляя каждое число в объекте Стек](#36-класс-стек-реализация-на-однонаправленном-списке-разработайте-функцию-для-сложения-двух-целых-чисел-большой-разрядности-представляя-каждое-число-в-объекте-стек)**
37. **[Линейный список - Очередь. АТД – очередь. Реализация очереди на связанном списке. Функции операций на вставки и удаления узлов очереди](#37-линейный-список---очередь-атд--очередь-реализация-очереди-на-связанном-списке-функции-операций-на-вставки-и-удаления-узлов-очереди)**
38. **[Класс Двунаправленный список. Разработать метод, который определяет, симметричен ли список, т.е. элементы, отстоящие от левой и правой вершин на одинаковое расстояние равны](#38-класс-двунаправленный-список-разработать-метод-который-определяет-симметричен-ли-список-те-элементы-отстоящие-от-левой-и-правой-вершин-на-одинаковое-расстояние-равны)**
39. **[Класс Граф. Реализовать на матрице смежности. Реализовать поиск кратчайшего пути от одной заданной вершины к другой, используя матрицу Флойда](#39-класс-граф-реализовать-на-матрице-смежности-реализовать-поиск-кратчайшего-пути-от-одной-заданной-вершины-к-другой-используя-матрицу-флойда)**
40. **[AVL дерево. Свойства. Алгоритм двойного поворота. Пример AVL дерева для балансировки которого требуется двойной поворот](#40-avl-дерево-свойства-алгоритм-двойного-поворота-пример-avl-дерева-для-балансировки-которого-требуется-двойной-поворот)**
41. **[Дана последовательность ключей 1,2,3,4,5,6,7,8,9. Постройте бинарное дерево минимальной высоты с такими ключами](#41-дана-последовательность-ключей-123456789-постройте-бинарное-дерево-минимальной-высоты-с-такими-ключами)**

---

### 1. В чем заключаются достоинства и недостатки последовательного и связанного способов реализации динамических структур данных?
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>
В памяти компьютера данные могут иметь последовательное или связанное представление. Соответственно различают структуры хранения, использующие последовательное представление данных и связанное представление данных.

При последовательном представлении данные в памяти компьютера размещаются в соседних последовательно расположенных ячейках. При этом физический порядок следования записей полностью соответствует логическому порядку, определяемому логической структурой, то есть логическая структура поддерживается физическим порядком следования данных. Совокупность записей, размещенных в последовательно расположенных ячейках памяти, называют последовательным списком.
 	
При связанном представлении в каждой записи предусматривается дополнительное поле, в котором размещается указатель (ссылка). В памяти компьютера записи располагаются в любых свободных ячейках и связываются между собой указателями, указывающими на место расположения записи, логически следующей за данной. Структуры хранения, основанные на связанном представлении данных, называют связанными списками. Если каждая запись содержит лишь один указатель, то список односвязный, при большем числе указателей - список многосвязный.
 	
Контейнерные классы предназначены для хранения данных, организованных определенным образом. Для каждого типа контейнера определены методы работы с его элементами, не зависящие от конкретного типа данных, которые хранятся в контейнере. Поэтому один и тот же вид контейнера можно использовать для хранения данных различных типов. Возможность работы с контейнерными классами реализована с помощью стандартной библиотеки шаблонов (STL Standard Template Library), в которую входят контейнерные классы, алгоритмы и итераторы. Использование STL позволяет повысить надежность программ и уменьшить сроки их реализации. 

Контейнеры можно разделить на два типа: последовательные и ассоциативные. 
 * *Последовательные контейнеры* обеспечивают хранение конечного количества однотипных элементов в виде непрерывной последовательности. К последовательным контейнерам относятся: векторы (vector), двусторонние очереди (deque), списки (list), а также так называемые адаптеры (варианты контейнеров): стеки (stack), очереди (queue) и очереди с приоритетами (priority_queue). Каждый вид контейнера обеспечивает свой набор действий над данными и выбор того или иного контейнера зависит от того, что именно требуется делать с данными в программе.
 * *Ассоциативные контейнеры* обеспечивают быстрый доступ к данным по ключу. Такие контейнеры построены на основе сбалансированных деревьев. К ассоциативным контейнерам относятся: словари (map), словари с дубликатами (multiset), множества (set), множества с дубликатами (multiset) и битовые множества (bitset).
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 2. Назовите принципы функционирования стека, очереди и дека
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>

* *Двусторонняя очередь (дек)* – последовательный контейнер, поддерживающий доступ к произвольным элементам и обеспечивает вставку и удаление из обоих концов очереди за постоянное время. Операции с элементами внутри очереди занимают время, пропорциональное количеству перемещаемых элементов. Доступ к элементам очереди осуществляется за постоянное время (оно несколько больше, чем для вектора).
* *Список* – последовательный контейнер, обеспечивающий вставку и удаление элементов за постоянное время. Не предоставляет произвольный доступ к своим элементам. Операции с элементами внутри списка (вставка элемента, удаление элемента) занимают постоянное время. 
* *Стек* – последовательный контейнер, обеспечивающий вставку элемента в вершину стека и удаление элемента из вершины стека. 
* *Очередь* – последовательный контейнер, обеспечивающий добавление элементов в конец очереди и извлечение элементов с начала очереди. 
* *Очередь с приоритетом* – структура, реализованная при помощи очереди на основе контейнера, допускающего произвольный доступ к элементам (например, вектора или двусторонней очереди). Первым параметром при описании очереди с приоритетами является тип ключа, вторым последовательный контейнер, третьим – функция определения приоритета. STL определяется в следующих заголовочных файлах: algorithm, deque, functional, iterator, list, map, memory, numeric, queue, set, stack, utility, vector.

</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 3. Реализуйте класс – Стек с базовым набором методов на основе массива нетипированных указателей на размещенные в динамической памяти элементы
<details> 
  <summary> 
	  <strong>[pointed_Stack.cpp]</strong>
  </summary>

```c++
template <typename T>
class Stack
{
private:
    T *stackPointer;                  // Указатель на стек
    const int size;                   // Максимальное количество элементов в стеке
    int top;                          // Номер текущего элемента стека
public:
    Stack(int = 10);                  // По умолчанию размер стека равен 10 элементам
    Stack(const Stack<T> &);          // Конструктор копирования
    ~Stack();                         // Жеструктор
 
    inline void push(const T & );     // Поместить элемент в вершину стека
    inline T pop();                   // Удалить элемент из вершины стека и вернуть его
    inline void printStack();         // Вывод стека на экран
    inline const T &Peek(int ) const; // N-й элемент от вершины стека
    inline int getStackSize() const;  // Получить размер стека
    inline T *getPointer() const;         // Получить указатель на стек
    inline int getTop() const;        // Получить номер текущего элемента в стеке
};
 
// Реализация методов шаблона класса STack
 
// Конструктор Стека
template <typename T>
Stack<T>::Stack(int maxSize) :
    size(maxSize) // Инициализация константы
{
    stackPointer = new T[size]; // Выделить память под стек
    top = 0; // Инициализируем текущий элемент нулем;
}
 
// Конструктор копирования
template <typename T>
Stack<T>::Stack(const Stack<T> & otherStack) :
    size(otherStack.getStackSize()) // Инициализация константы
{
    stackPointer = new T[size]; // Выделить память под новый стек
    top = otherStack.getTop();
 
    for(int ix = 0; ix < top; ix++)
        stackPointer[ix] = otherStack.getPointer()[ix];
}
 
// Функция деструктора Стека
template <typename T>
Stack<T>::~Stack()
{
    delete [] stackPointer; // Удаляем стек
}
 
// Функция добавления элемента в стек
template <typename T>
inline void Stack<T>::push(const T &value)
{
    // Проверяем размер стека
    assert(top < size); // Номер текущего элемента должен быть меньше размера стека
    stackPointer[top++] = value; // Помещаем элемент в стек
}
 
// Функция удаления элемента из стека
template <typename T>
inline T Stack<T>::pop()
{
    // Проверяем размер стека
    assert(top > 0); // Номер текущего элемента должен быть больше 0
    return stackPointer[--top]; // Удаляем элемент из стека
}
 
// Функция возвращает n-й элемент, в коде это chosenElement от вершины стека
template <class T>
inline const T &Stack<T>::Peek(int chosenElement) const
{
  assert(chosenElement <= top);
  return stackPointer[top - chosenElement]; // Вернуть n-й элемент стека
}
 
// Вывод стека на экран
template <typename T>
inline void Stack<T>::printStack()
{
    for (int ix = top - 1; ix >= 0; ix--)
        cout << "|" << setw(4) << stackPointer[ix] << endl;
}
 
// Вернуть размер стека
template <typename T>
inline int Stack<T>::getStackSize() const
{
    return size;
}
 
// Вернуть указатель на стек (для конструктора копирования)
template <typename T>
inline T *Stack<T>::getPointer() const
{
    return stackPointer;
}
 
// Вернуть размер стека
template <typename T>
inline int Stack<T>::getTop() const
{
    return top;
}
```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 4. С использованием основных методов работы со стеком составьте программу копирования элементов стека в новый стек в том же порядке
<details> 
  <summary> 
	  <strong>[copyStack.cpp]</strong>
  </summary>
	
```c++
#include <iostream>
#include <string>
 
class firstStack{
private:
    int firstStackTop;
    int firstStackArray[3];
public:
    firstStack(){
        firstStackTop = -1;
    }
    void set(int value){
        firstStackArray[++firstStackTop] = value;
    }
 
    int get(){
        return firstStackArray[firstStackTop--];
    }
};
 
class secondStack{
private:
    int secondStackTop;
    int secondStackArray[3];
public:
    secondStack(){
        secondStackTop = -1;
    }
 
    void set (firstStack* S){
        secondStackArray[++secondStackTop] = S -> get();
    }
 
    void display(){
        std::cout << secondStackArray[secondStackTop--] << std::endl;
    }
};
 
 
int main(){
    SetConsoleCP (1251);
    SetConsoleOutputCP (1251);
 
    firstStack from;
    from.set(34);
    from.set (54);
    from.set (23);
 
    secondStack to; to.set (&from);
    to.set (&from);
    to.set (&from);
 
    to.display();
    to.display();
    to.display();
 
 
    system ("pause");
    return NULL;
};
```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

--- 

### 5. Реализуйте метод копирования элементов очереди в новую очередь
<details> 
  <summary> 
    <strong>[swapQueue.cpp]</strong>
  </summary>
<summary> 
    <strong><em>pop()</em></strong>
  </summary>

```c++
// pop() removes front element of the queue and reduces size of the queue by one.
#include <iostream>
#include <queue>

using namespace std;

int main(void) {
   queue<int> q;

   for (int i = 0; i < 5; ++i)
      q.emplace(i + 1);

   cout << "Contents of queue" << endl;
   while (!q.empty()) {
      cout << q.front() << endl;
      q.pop();
   }

   return 0;
}
```
<summary> 
    <strong><em>front()</em></strong>
  </summary>

```c++
//front() returns a reference to the first element of the queue. 
//This element will be removed after performing pop operation on queue.
#include <iostream>
#include <queue>

using namespace std;

int main(void) {
   queue<int> q;

   for (int i = 0; i < 5; ++i)
      q.emplace(i + 1);

   cout << "First element of queue = " << q.front() << endl;

   return 0;
}
```
<summary> 
    <strong><em>empty()</em></strong>
  </summary>

```c++
//empty() tests whether queue is empty or not. 
//Queue of zero size is considered as empty queue.
#include <iostream>
#include <queue>

using namespace std;

int main(void) {
   queue<int> q;

   if (q.empty())
      cout << "Queue is empty." << endl;

   q.push(10);

   if (!q.empty())
      cout << "Queue is not empty." << endl;

   return 0;
}
```
<summary> 
    <strong><em>swap()</em></strong>
  </summary>

```c++
// swap() exchanges the contents of two queues.
#include <iostream>
#include <queue>
#include <list>

using namespace std;

int main(void) {
   auto mainArray = {1, 2, 3, 4, 5};
   queue<int> queueOne(mainArray);
   queue<int> queueTwo(queueOne);

   cout << "Contents of queueOne" << endl;
   while (!queueOne.empty()) {
      cout << queueOne.front() << endl;
      queueOne.pop();
   }
   
   cout << endl;

   cout << "Contents of queueTwo" << endl;
   while (!queueTwo.empty()) {
      cout << queueTwo.front() << endl;
      queueTwo.pop();
   }

   return 0;
}
```
Результат:
```
Contents of queueOne: 1 2 3 4 5
Contents of queueTwo: 1 2 3 4 5
```
</details>

[Источник](http://www.tutorialspoint.com/cpp_standard_library/cpp_queue_swap_queue.htm)

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 6. Перевод из инфиксной формы записи выражения в префиксную
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>

***В инфиксной записи*** операция разделяет два операнда, в постфиксной – операция следует за двумя операндами, в префиксной – операция предшествует двум операндам. Например:

| ***Инфиксная запись*** | ***Постфиксная запись*** | ***Префиксная запись*** |
| ------------- |:------------------:| -----:|
| A+B    | AB+   | +AB |
| A+B–C    | AB+C– | +A–BC |
| A*B+C  | AB*C+| +*ABC |
| A+B*C   | ABC*+ |   +A*BC |
| (A+B)*C  | AB+C* |  *+ABC |

***Перевод из инфиксной формы записи выражения в префиксную***
<br>Инфиксное выражение сканируется справа налево, и префиксная строка строится также справа налево. Алгоритм преобразования такой же, как и при преобразовании в постфиксную форму, только открывающие скобки меняются на закрывающие и, наоборот, при определении приоритета операции «<=» изменяется на «<», чтобы равноприоритетные операции выполнялись слева направо.

***Вычисление значения выражения по его префиксной записи***
<br>Алгоритм вычисления полностью совпадает с алгоритмом вычисления по постфиксной записи, но префиксная строка сканируется справа налево.

</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 7. Перевод инфиксной формы записи выражения в постфиксную
<details> 
  <summary> 
	  <strong>[postfix_to_infix.cpp]</strong>
  </summary>

```c++
#include <string.h>
#include <stdio.h>
#include <stdlib.h>

// <--Структуры данных-->
enum optype {power = 3, devide = 2, multiply = 2, minus = 1, plus = 1, null=0}; // приоритеты операций

struct stack {
	char val[100]; // непосредственно значение элемента
	optype type; // приоритет операции, необходим для правильного расставления  скобок
	stack * next;
} *head;

// <--Функции работы со стеком-->
void push(char[], optype);
void push(stack *);
stack * pop();
// <--Функция выполняющая наш алгоритм-->
void fromRPN(char *, char *); // (RPN) Reverse polish notation

int main() {
	char infix[100], postfix[100]; // входная и выходная строка
	gets(infix);
	fromRPN(infix, postfix);
	printf("%s\n", postfix);
	system("PAUSE");
	return 0;
}

void push(stack *t) {
	t->next = head;
	head = t;
}

void push(char str[], optype type) {
	stack *t;
	t = new stack;
	strcpy(t->val, str);
	t->type = type;
	t->next = head;
	head = t;
}

stack * pop() {
	stack *t;
	if(head == NULL) return NULL;
	t = head;
	head = t->next;
	return t;
}

void fromRPN(char * input, char * output) {
	char c, temp[100];
	int p_temp=0;
	stack *h1, *h2; // переменные для хранения первых двух элементов стека
	optype type;
	head = NULL;
	while(*input) { // пока есть символы строке
		c = (*input);
		if(c>='0' && c<='9' || c=='.') { //если текущий символ часть числа
			temp[p_temp++] = c; //то добавляем его во временную строку
			temp[p_temp] = '\0';
		} else if(c==' ') {
			if(p_temp!=0) {
				push(temp, null); // добавляем число в стек
				p_temp=0; }
			temp[0] = '\0'; // опустошаем временную строку
		} else if(c=='+' || c=='-'|| c=='*' || c=='/' || c=='^') { //если читаем знак операции
			h1 = pop(); // выталкиваем первый элемент
			h2 = pop(); // выталкиваем второй элемент
                        // находим приоритет операции
			if(c=='+') type = plus;
			else if(c=='-') type = minus;
			else if(c=='*') type = multiply;
			else if(c=='/') type = devide;
			else if(c=='^') type = power;
			if(h2->type!=null && h2->type<type) { // если приоритет для 1-го элемента меньше
				temp[0]='('; temp[1] = '\0'; // берем выражение в скобки
				h2->val[strlen(h2->val)+2] = '\0';
				h2->val[strlen(h2->val)+1] = c; // приписываем знак операции
				h2->val[strlen(h2->val)] = ')';
			} else {
				h2->val[strlen(h2->val)+1] = '\0';
				h2->val[strlen(h2->val)] = c;
			}
			strcat(temp, h2->val);
			if(h1->type!=null && h1->type<type) {  // если приоритет для 2-го элемента меньше
				strcat(temp, "(");
				h1->val[strlen(h1->val)+1] = '\0';
				h1->val[strlen(h1->val)] = ')'; // берем выражение в скобки
			}
			strcat(temp, h1->val);
			strcpy(h2->val, temp); // что бы не выделять память под новый элемент, копируем полученное выражение во второй элемент
			delete h1; // удаляем первый элемент
			h2->type = type; // устанавливаем новый приоритет операции
			push(h2); // добавляем новый элемент в стек
		}
		input++;
	}
	strcpy(output, (pop())->val); // копируем выражение из вершины стека в строку результата
}
```
</details/>
<details> 
  <summary> 
	  <strong>[infix_to_postfix.cpp]</strong>
  </summary>

```c++
/**
 *  Given an infix expression, convert it to postfix. Consider usual operator precedence.
 *  Consider only following operands in your arsenal.
 *  +, -, * , /, ^(power)
 *  Operands are only alphabets --> 'a '-->'z' and 'A'-->'Z'
 *  Another assumption is operand is a single char.
 */

#include <iostream>
#include <stack.h>
#include <string>

// all utility and main functions declared first
/**
 * isOperator- Determines if input char is operator
 * @param  c - char
 * @return   - true or false
 */
bool isOperator( char c );

/**
 * isOperand Determines if input char is operand
 * @param  c - char
 * @return   true or false.
 */
bool isOperand( char c );


/**
 * getOperatorWeight returns an integer weight of the operator
 * @param  c  - An operator
 * @return   Weight of operator , larger is more precedence
 */
int getOperatorWeight(char c);


/**
 * isRightAssociative -Determines if operator is right associative.
 * @param  c operator
 * @return   returns true if operator is right associative
 *
 * Associativity only comes to picture when both operators have same weight
 * Example ^ is right associative ( ^ represents power of)
 * 5 ^ 4 ^ 3 ^ 2  = 5 ^ ( 4 ^ ( 3 ^ 2 ) )
 * where as  7 − 4 + 2 (7 − 4) + 2 = 5 or 7 − (4 + 2) = 1
 */
bool isRightAssociative(char c);

/**
 * [hasHigherPrecedence] compare op1 and op2 based on precedence
 * @param  op1 operaror 1
 * @param  op2 operator 2
 * @return     return true if precedence(op1) > precedence(op2), else false
 */
bool hasHigherPrecedence(char op1, char op2);

/**
 * [infixToPostfix - converts infix expr to postfix expr
 * @param  expression - infix expre
 * @return            postfix expr
 */
std::string infixToPostfix( std::string expression );


//check if c is an operator
bool isOperator( char c )
{
  if ( c == '+' || c == '-' || c == '*' || c == '/' || c == '^') {
    return true;
  }
  return false;
}

//check if c is a valid operand defined in comments.
bool isOperand( char c )
{
  if ( c >= 'a' && c <= 'z' ) return true;
  if ( c >= 'A' && c <= 'Z' ) return true;
  return false;
}

//returns precedence weight of the char c.
// more weight higher precedence.
int getOperatorWeight( char c )
{
  int weight;
  switch(c) {
    case '+':
    case '-':
      weight = 1;
      break;
    case '*':
    case '/':
      weight = 2;
      break;
    case '^':
      weight = 3;
      break;
    default:
      weight = -1;
  }
  return weight;
}


// is operator right associative?
bool isRightAssociative( char op )
{
  if ( op == '^') return true;
  return false;
}

bool hasHigherPrecedence( char op1, char op2 )
{
  // get weight of the operators
  int w1 = getOperatorWeight(op1);
  int w2 = getOperatorWeight(op2);

  // If both operators weigh same, return true if operators are
  // left associative, return false if right associative.
  if ( w1 == w2 ) {
    if ( isRightAssociative(op1) ) {
      return false;
    }
    return true;
  }
  return w1 > w2 ? true : false;
}

// final function to convert infix to postix operator.

std::string infixToPostFix(std::string expr)
{
  bool errorDetected = false;
  algo::Stack<char> operatorStack;
  std::string postFixExpr = "";

  //scanning input infix expr left to right char by char
  for ( char c : expr ) {

    // char is delimiter, continue
    if ( c == ',' || c == ' ') {
      continue;
    }

    //if character is an operand
    else if ( isOperand(c) ) {
      postFixExpr += c;
    }

    //if character is operator
    else if ( isOperator(c) ) {
      //if stack is not empty pop the stack back and compare precedence.
      //if higher precedence perform operation.
      while ( !operatorStack.empty() &&  operatorStack.top() != '(' &&
              hasHigherPrecedence(operatorStack.top(), c) ) {
          postFixExpr += operatorStack.top();
          operatorStack.pop();
      }
      operatorStack.push(c);
    }

    else if( c == '(' ) {
      operatorStack.push(c);
    }

    else if( c == ')' ) {
      while( !operatorStack.empty() && operatorStack.top() != '(' ) {
        postFixExpr += operatorStack.top();
        operatorStack.pop();
      }
      operatorStack.pop();
    }

    else {
      std::cout << " ERROR An invalid operator/operand detected\n";
      errorDetected = true;
      break;
    }
  }
  if (errorDetected) {
    return "INVALID EXPR!";
  }

  while( !operatorStack.empty() ) {
    postFixExpr += operatorStack.top();
    operatorStack.pop();
  }
  return postFixExpr;
}


int main()
{
  std::string expr;
  std::cout << "Provide an expression such that :"
            << "1. Expression shoule be parenthesis valid.\n"
            << "2. Operators should contain +, -, /, *, ^\n"
            << "3. Operands should contain A-Z or a-z \n"
            << "Your expression is :";
  std::getline(std::cin, expr);
  std::cout << "Corresponding postfix expression of the express - "
            << expr
            << " is :" << infixToPostFix(expr) << std::endl;
  return 0;
}

```
</details> 
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>

***Перевод из инфиксной формы записи выражения в постфиксную (польскую)*** <br>Инфиксное выражение сканируется слева направо, и в зависимости от вида очередного элемента выражения выполняется одно из следующих действий:

| ***Элемент выражения*** | ***Действие*** |
| ------------- |:------------------:| 
| Открывающая скобка | Вталкивание элемента в стек |
| Операнд | Запись элемента в постфиксную строку | 
|Закрывающая скобка  |Выталкивание элементов из стека до первой открывающей скобки и запись их в постфиксную строку, затем выталкивание самой открывающей скобки без записи ее в постфиксную строку. Если перед выполнением этой операции стек оказался пустым, значит, для данной закрывающей скобки не было парной открывающей, т.е. возникла исключительная ситуация |
| Операция  | Если стек не пуст, и приоритет операции ниже (<=), чем у верхней операции в стеке, то выталкивание элементов из стека до операции с меньшим приоритетом или до опустошения стека и запись их в постфиксную строку; в противном случае стек не изменяется. Затем вталкивание операции в стек |   

После просмотра выражения выталкиваются из стека и записываются в постфиксную строку все оставшиеся в стеке операции.
<br><br>
***Вычисление значения выражения по его постфиксной записи***
<br>Постфиксное выражение сканируется слева направо и обрабатывается следующим образом:

| ***Элемент выражения*** | ***Действие*** |
| ------------- |:------------------:| 
| Операнд  | Вталкивание элемента в стек |
| Операция | Выталкивание из стека двух элементов, выполнение операции с ними, запись результата в стек, если стек не пуст |

</details>

&emsp;&ensp;**[infix_to_postfix.cpp](https://github.com/mandliya/algorithms_and_data_structures/blob/master/stack_problems/infix_to_postfix.cpp)**

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 8. С использованием стандартного набора методов составьте программу переноса из очереди строк в новую очередь элементов начинающихся на буквы «F» или «f»

<details> 
  <summary> 
    <strong>[Черновик]</strong>
  </summary>

```c++
//Создать массив строк, отсортировать его по нужным символам F и f, результат сортировки перезаписать в новый массив, 
//который бы  передавался как основной для копирования из одной очереди в другую.
typedef std::vector<std::string> StringArray;
 
// Заполнение массива строк.
void FillArray(StringArray& array)
{
  StringArray strings;
  strings.push_back("Fsffsf");
  strings.push_back("sfasdfa");
  strings.push_back("324fsfd");
  strings.push_back("F2422d");
  strings.push_back("aadf");
  array.swap(strings);
}
 
// Проверка символа. Если он "плохой" возвращаем true.
bool IsSymbolBad(char symbol)
{
  return !isalpha(symbol);
}
 
// Проверка строки на наличие плохи символов.
bool HasBadSymbol(const std::string& str)
{
  // Поиск "плохого" символа в строке.
  std::string::const_iterator pos = std::find_if(str.begin(), str.end(), &IsSymbolBad);
 
  // Если "плохой" символ найден, возвращаем true.
  return pos != str.end();
}
 
// Обработка массива строк согласно заданию.
void ProcessArray(StringArray& array)
{
  // Удаление строк у которых есть "плохие" символы.
  StringArray::iterator newEnd = std::remove_if(array.begin(), array.end(), &HasBadSymbol);
  array.erase(newEnd, array.end());
 
  // Сортировка массива строк по алфавиту.
  std::sort(array.begin(), array.end());
}
 
int main()
{
  StringArray array;
  FillArray(array);
  PrintArray("Before processing:", array);
  ProcessArray(array);
  PrintArray("After processing:", array);
  return 0;
}

```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 9. С использованием стандартного набора методов составьте программу записи элементов очереди в новую очередь в обратном порядке

```c++
// Копирование рассмотрено в методе swap() Вопрос №5
// C++ code for reversing a queue 
#include <bits/stdc++.h> 
using namespace std; 
  
// Utility function to print the queue 
void printQueue(queue<long long int> Queue) 
{ 
    while (!Queue.empty()) { 
        cout << Queue.front() << " "; 
        Queue.pop(); 
    } 
} 
  
// Recursive function to reverse the queue 
void reverseQueue(queue<long long int>& q) 
{ 
    // Base case 
    if (q.empty()) 
        return; 
  
    // Dequeue current item (from front)   
    long long int data = q.front(); 
    q.pop(); 
  
    // Reverse remaining queue   
    reverseQueue(q); 
  
    // Enqueue current item (to rear)   
    q.push(data); 
} 
  
// Driver code 
int main() 
{ 
    queue<long long int> Queue; 
    Queue.push(56); 
    Queue.push(27); 
    Queue.push(30); 
    Queue.push(45); 
    Queue.push(85); 
    Queue.push(92); 
    Queue.push(58); 
    Queue.push(80); 
    Queue.push(90); 
    Queue.push(100); 
    reverseQueue(Queue); 
    printQueue(Queue); 
} 

```
```
Результат: 100 90 80 58 92 85 45 30 27 56 
```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 10. АТД – очередь. Ее свойства. Способы реализации
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>
	
***О́чередь*** — абстрактный тип данных с дисциплиной доступа к элементам «первый пришёл — первый вышел» (FIFO, англ. first in, first out). Добавление элемента (принято обозначать словом enqueue — поставить в очередь) возможно лишь в конец очереди, выборка — только из начала очереди (что принято называть словом dequeue — убрать из очереди), при этом выбранный элемент из очереди удаляется.

***Операции над очередью***
<br>Над очередью q (от англ. queue – очередь) могут быть выполнены следующие операции:
* Включение нового элемента v в конец очереди – Insert(q,v);
* Исключение элемента из начала очереди – Remove(q) и возвращение его значения;
* Выработка признака «очередь пуста» – Empty(q);
* Считывание первого элемента без его удаления – HeadValue(q);
* Считывание последнего элемента очереди – RearValue(q);
* Определение числа элементов очереди Size(q);
* Очистка очереди – Clear(q).

Первые три операции над очередью являются основными. Операции Empty, Size, и Clear для очереди аналогичны соответствующим операциям для стека.

</details>
<details> 
  <summary> 
	  <strong>Рисунок</strong>
  </summary>
<a href="https://github.com/ForWhomTheBellTolls/SiAOD"><img src="https://i.imgur.com/K9KPK2H.png"></a>	
</details>

<details> 
  <summary> 
	  <strong>[Queue]</strong>
  </summary>

```c++
#ifndef QUEUE_H
#define QUEUE_H

#include <exception>

namespace algo {
    const int defaultQueueCapacity = 500;

    template <typename T>
        class Queue {
            public:
                Queue( int capacity = defaultQueueCapacity )
                    : _capacity { capacity }, _count { 0 },
                      _head { 0 }, _tail { -1 }, _elements { new T[_capacity] }
                { 
                }

                bool empty() const
                {
                    return ( _count == 0 );
                }

                int count() const
                {
                    return _count;
                }

                int capacity() const
                {
                    return _capacity;
                }

                void pop()
                {
                    if (empty())
                    {
                        return;
                    }
                    else { 
                        --_count;
                        ++_head;
                        if ( _head == _capacity ) {
                            _head = 0;
                        }
                    }
                }

                bool push( const T & obj )
                {
                    if ( _count == _capacity )
                    {
                        return false;
                    }
                    else {
                        ++_count;
                        ++_tail;
                        if ( _tail == _capacity )
                        {
                            _tail = 0;
                        }
                        _elements[_tail]  = obj;
                        return true;
                    }
                }

                const T & front() const
                {
                    if ( empty() ) throw empty_queue_exception;
                    return _elements[_head];
                }

            private:
                class EmptyQueueException : public std::exception {
                    virtual const char * what() const throw()
                    {
                        return "Queue is empty";
                    }
                } empty_queue_exception;

                int _capacity;
                int _count;
                int _head;
                int _tail;

                T * _elements;

                Queue( const Queue & );
                Queue & operator= ( const Queue & );

        }; //end of class queue

} //end of namespace algo

#endif //end of QUEUE_H
```
</details> 

&emsp;&ensp;**[Еще код на C++](https://codelessons.ru/cplusplus/ochered-queue-v-c-realizaciya-i-chto-eto-voobshhe-takoe.html)**<br>
&emsp;&ensp;**[Queue.h](https://github.com/mandliya/algorithms_and_data_structures/blob/master/include/queue.h)**

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 11. Разработать класс «Бинарное дерево поиска». Реализовать метод вставки нового узла в дерево
<details> 
  <summary> 
    <strong>[insertTreeNode.cpp]</strong>
  </summary>

Insert Node [insertTreeNode()]
<br>Insertion begins as a search would begin; if the root is not equal to the value, we search the left or right subtrees as before. Eventually, we will reach an external node and add the value as its right or left child, depending on the node's value.<br>In other words, we examine the root and recursively insert the new node to the left subtree if the new value is less than the root, or the right subtree if the new value is greater than or equal to the root. Ω(logn) operations
```c++
struct Tree
{
  char data;
  Tree *left;
  Tree *right;  
  Tree *parent;  
};

struct Tree* insertTreeNode(struct Tree *node, int data)
{
  static Tree *p;
  Tree *retNode;

  //if(node != NULL) p = node;

  if(node == NULL)  {
      retNode = newTreeNode(data);
      retNode->parent = p;
      return retNode;
  }
  if(data <= node->data ) { 
      p = node;
      node->left = insertTreeNode(node->left,data);
  } 
  else {
      p = node;
      node->right = insertTreeNode(node->right,data);
  } 
  return node;
}
```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 12. АТД Дек – это очередь с двумя вершинами: правой и левой, характеристика
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>

*Дек* — структура данных, представляющая из себя список элементов, в которой добавление новых элементов и удаление существующих производится с обоих концов. Эта структура поддерживает как FIFO, так и LIFO, поэтому на ней можно реализовать как стек, так и очередь. В первом случае нужно использовать только методы головы или хвоста, во втором — методы push и pop двух разных концов. Дек можно воспринимать как двустороннюю очередь.
* **empty** — проверка на наличие элементов,
* **pushBack** (запись в конец) — операция вставки нового элемента в конец,
* **popBack** (снятие с конца) — операция удаления конечного элемента,
* **pushFront** (запись в начало) — операция вставки нового элемента в начало,
* **popFront** (снятие с начала) — операция удаления начального элемента.

</details>
<details> 
  <summary> 
    <strong>[Простая реализаци]</strong>
  </summary>

В данной реализации изначально **head=n−1** и **tail=n−1**. Ключевые поля: 
* **array[0…2×n−1]** — массив, с помощью которого реализуется дек, способный вместить не более n элементов,
* **head** — индекс головы дека,
* **tail** — индекс хвоста.

Дек состоит из элементов **array[head…tail−1]**. Если происходит максимум **n** добавлений, то массив длины **2×n** может вместить в себя все добавленные элементы.

```c++
boolean empty():
  return head == tail
  
function pushBack(x : T):
  array[tail++] = x
  
T popBack():
  if (empty()) 
    return error "underflow" 
  return array[--tail]
  
function pushFront(x : T):
  array[--head] = x
  
T popFront():
  if (empty()) 
    return error "underflow" 
  return array[head++]
```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 13. Класс «Бинарное дерево поиска». Реализуйте метод поиска элемента в дереве
<details> 
  <summary> 
    <strong>[Поиск элемента]</strong>
  </summary>
	
Для поиска элемента в бинарном дереве поиска можно воспользоваться следующей функцией, которая принимает в качестве параметров корень дерева и искомый ключ. Для каждого узла функция сравнивает значение его ключа с искомым ключом. Если ключи одинаковы, то функция возвращает текущий узел, в противном случае функция вызывается рекурсивно для левого или правого поддерева. Узлы, которые посещает функция образуют нисходящий путь от корня, так что время ее работы **O(h)** , где **h** — высота дерева. 

  ```c++
  Node search(x : Node, k : T):
   if x == null or k == x.key
      return x
   if k < x.key
      return search(x.left, k)
   else
      return search(x.right, k)
   ```
  </details> 
 <details>
  <summary> 
      <strong>[Рис. Поиск элемента 4]</strong>
  </summary>
 <a href="https://github.com/ForWhomTheBellTolls/SiAOD"><img src="https://i.imgur.com/i37O5wZ.png" width=266"></a>
</details>
<details>
  <summary> 
    <strong>[Поиск минимума и максимума]</strong>
  </summary>
	
Чтобы найти минимальный элемент в бинарном дереве поиска, необходимо просто следовать указателям **left** от корня дерева, пока не встретится значение **null**. Если у вершины есть левое поддерево, то по свойству бинарного дерева поиска в нем хранятся все элементы с меньшим ключом. Если его нет, значит эта вершина и есть минимальная. Аналогично ищется и максимальный элемент. Для этого нужно следовать правым указателям. 

```c++
  Node minimum(x : Node):
  if x.left == null
     return x
  return minimum(x.left)
  
  Node maximum(x : Node):
  if x.right == null
     return x
  return maximum(x.right)
```
Данные функции принимают корень поддерева, и возвращают минимальный (максимальный) элемент в поддереве. Обе процедуры выполняются за   время **O(h)**. 
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 14. АТД Очередь с приоритетом. Ее свойства. Способы реализации
<details> 
  <summary> 
	  <strong>[prio_queue_by_binary_heap]</strong>
  </summary>
 
 ```c++
class pri_queue
{
public:
  prio_queue(Compare const& comp = Compare());
  
  using value type = Prio;
  using payload_type = Value;
  
  void                           push(Prio p, Value v);
  std::pair<Prio const&, Value&> top() const noexcept;
  void                           pop();
  void                           reschedule_top(Prio);
  bool                           empty() const noexcept;
  std::size_t                    size() const noexcept();
};
 ```
</details> 
<details> 
  <summary> 
    [prio_queue_by_static_stl_array]
  </summary>
  
  ```c++
#include <iostream>
#include <algorithm>
#include <cassert>
 
 
template<typename Type, std::size_t Size>
class min_priority_queue {
 
public:
   min_priority_queue() : index(0) {}   
 
   void push(Type const& value) {
      assert(index < Size);
      container[index] = value;
      std::push_heap(&container[0], &container[0] + ++index, std::greater<int>());
   }
   
   void pop() {
      assert(index > 0);
      std::pop_heap(&container[0], &container[0] + index--, std::greater<int>());
   }
   
   Type & top() {
      assert(index > 0);
      return container[0];
   }
   
   Type const& top() const {
      assert(index > 0);
      return container[0];
   }
 
private:
   Type         container[Size];
   std::size_t  index;
};
 
 
int main() {
   min_priority_queue<int, 10> queue;
   
   queue.push(1);
   std::cout << queue.top() << std::endl;
   queue.push(2);
   std::cout << queue.top() << std::endl;
   queue.pop();
   std::cout << queue.top() << std::endl;
   queue.push(-1);
   std::cout << queue.top() << std::endl;
   queue.push(-3);
   std::cout << queue.top() << std::endl;
   queue.pop();
   std::cout << queue.top() << std::endl;
   queue.push(6);
   std::cout << queue.top() << std::endl;
}
  ```
</details> 

&emsp;&ensp;**[prio_queue_by_binary_heap](https://github.com/rollbear/prio_queue/blob/master/README.md)**

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 15. Класс Идеально сбалансированное бинарное дерево. Реализуйте алгоритм прямого обхода дерева в глубину

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 16. АТД Стек. Свойства. Способы реализации

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```
***[Теория](http://www.mkurnosov.net/teaching/uploads/DSA/dsa-lecture4.pdf)***

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 17. Класс Хеш-таблица. Реализация коллизий – цепное хеширование. Реализуйте метод вставки в таблицу нового узла с проверкой коэффициента нагрузки таблицы и рехеширования

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 18. АТД Линейный список. Свойства. Способы реализации
<details> 
  <summary> 
	  <strong>[linked_list.cpp]</strong>
  </summary>

```c++
#include <iostream>
using namespace std;

class LinkedList{
    // Struct inside the class LinkedList
    // This is one node which is not needed by the caller. It is just
    // for internal work.
    struct Node {
        int x;
        Node *next;
    };

// public member
public:
    // constructor
    LinkedList(){
        head = NULL; // set head to NULL
    }

    // destructor
    ~LinkedList(){
        Node *next = head;

        while(next) {              // iterate over all elements
            Node *deleteMe = next;
            next = next->next;     // save pointer to the next element
            delete deleteMe;       // delete the current entry
        }
    }

    // This prepends a new value at the beginning of the list
    void addValue(int val){
        Node *n = new Node();   // create new Node
        n->x = val;             // set value
        n->next = head;         // make the node point to the next node.
                                //  If the list is empty, this is NULL, so the end of the list --> OK
        head = n;               // last but not least, make the head point at the new node.
    }

    // returns the first element in the list and deletes the Node.
    // caution, no error-checking here!
    int popValue(){
        Node *n = head;
        int ret = n->x;

        head = head->next;
        delete n;
        return ret;
    }

// private member
private:
    Node *head; // this is the private member variable. It is just a pointer to the first Node
};

int main() {
    LinkedList list;

    list.addValue(5);
    list.addValue(10);
    list.addValue(20);

    cout << list.popValue() << endl;
    cout << list.popValue() << endl;
    cout << list.popValue() << endl;
    // because there is no error checking in popValue(), the following
    // is undefined behavior. Probably the program will crash, because
    // there are no more values in the list.
    // cout << list.popValue() << endl;
    return 0;
}
```
</details>
<details> 
  <summary> 
	  <strong>Теория</strong>
  </summary>

Линейный спи́сок — базовая динамическая структура данных в информатике, состоящая из узлов, каждый из которых содержит как собственно данные, так и одну или две ссылки («связки») на следующий и/или предыдущий узел списка. Принципиальным преимуществом перед массивом является структурная гибкость: порядок элементов связного списка может не совпадать с порядком расположения элементов данных в памяти компьютера, а порядок обхода списка всегда явно задаётся его внутренними связями.

Линейный список представляет последовательность из n>0 узлов x[1], x[2], ... ,x[n], важнейшей структурной особенностью которой является такое расположение элементов списка один относительно другого, как будто они находятся на одной линии. Иначе говоря, в такой структуре следует соблюдать условие: если n>0 и x[1] является первым узлом, а x[n] – последним, то k-тый узел x[k] следует за x[k-1] узлом и перед x[k+1] узлом для любого k лежащего в промежутке от 1 до n.

С линейными списками могут выполняться `следующие операции:`
* Получение доступа к x[k] элементу списка для проверки и/или изменения содержания его полей
* Вставка нового узла сразу до или после x[k] узла
* Удаление x[k] узла 
* Разбиение линейного списка на два и более списка.
* Создание копии линейного списка
* Определение количества узлов с списке
* Сортировка узлов в порядке возрастания значений в определенных полях этих узлов
* Поиск узла с заданным значением некоторого поля

Линейные списки, в которых операции *вставки (вставка нового узла сразу до или после x[k] узла списка)*, *удаления* и *операции доступа к значению (получение доступа к x[k] элементу списка для проверки и/или изменения содержания его полей)* чаще всего выполняются в первом и последнем узле получили специальное название: 
* *Стек* – линейный список, в котором операции вставки и удаления (и как правило доступа к данным) выполняются только на одном из концов списка; 
* *Очередь* (односторонняя очередь) – линейный список, в котором все операции вставки выполняются на одном конце списка, а все операции удаления (и доступа, как правило) – на другом; 
* *Дек* (двухсторонняя очередь) – линейный список, в котором все операции вставки, удаления и доступа выполняются с обоих концов. Различают дек с ограниченным вводом и ограниченным выводом, в котором операция удаления и вставки элементов соответственно выполняется только на одном из концов.

Под связными списками понимается набор элементов, причем каждый из них является часть узла *Node*, который также содержит ссылку *Link*.

```c++

struct Node{Item item; Node *next;};
typedef Node* Link;

```
Соответственно узлы в связном списке ссылаются на узлы и поэтому связный список называется самоссылочным. Простые линейные списки можно рассматривать как последовательность , в которой принято одно из следующих соглашений для ссылки последнего узла, а именно:
* Пустая (NULL) ссылка, не указывает ни на какой узел
* Ссылка, которая указывает на фиктивный узел, который не содержит элемента
* Ссылка, которая указывает на первый узел, делает список циклическим

В каждом случае отслеживание ссылок от первого элемента до последнего формирует последовательность расположения элементов. При программировании связных списков как только возникает необходимость использовать новый узел в списке для него необходимо резервировать память.
<br><br>При объявлении переменной типа *Node* для нее резервируется память во время компиляции. 
<br><br>Однако часто приходится организовывать вычисления, связанные с резервирование памяти во время выполнения посредством вызовов системных операторов управления памятью.

</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 19. Класс Бинарное дерево. Реализовать метод по алгоритму симметричного обхода дерева с выводом списка вершин (номеров вершин)

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```
**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 20. Инфиксная и постфиксная запись выражения. Алгоритм создания постфиксной записи арифметического выражения из инфиксной. Пример создания постфиксной записи арифметического выражения (схема преобразования)

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 21. Класс Бинарное дерево поиска. Реализовать метод удаления узла с наибольшим значением, учитывая все случаи

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 22. Класс Бинарное дерево. Реализуйте метод, который определяет количество узлов в дереве

**[Теоретическая основа для всех последующих деревьев](https://www.bogotobogo.com/cplusplus/binarytree.php)**

**[:u6e80:Вернуться к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 23. АТД сильно ветвящееся дерево. Способы реализации. Алгоритмы обхода в глубину

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 24. Класс Стек. Реализация методов: втолкнуть узел в стек, вытолкнуть узел из стека. Использование при вычислении значения арифметического выражения, содержащего скобки

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 25. АТД AVL дерево. Свойства. Алгоритм балансировки дерева при правом повороте

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 26. АТД – объединение списков. Реализуйте АТД на линейной связанной структуре. Даны два линейных однонаправленных списка L и М. Где L {L1,L2,…..Lki } где 0<=i<=ki; и 0<=Li<=99, а М={M0, M1,…..Mkj} где 0<=j<=kj и 100<=Mj<=199. Объедините эти списки в один список LM={L0M0,L1M1….., LiMj….} где j>=i, а Li и Mj это два значения одного элемента списка LM

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 27. Ориентированный взвешенный граф. Свойства ориентированного графа. Представление в памяти. Алгоритм Дейкстры – поиск кратчайшего пути

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 28. Класс - циклический линейный двунаправленный список. Реализуйте метод вставки нового узла в упорядоченный список так, чтобы упорядоченность не нарушилась

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 29. Хеш-таблица. Применение. Коллизии. Подходы к реализации коллизий

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 30. Класс Линейный однонаправленный список. Реализовать метод удаления узла с заданным номером из списка

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 31. АТД очередь с приоритетом. Свойства. Способы реализации. Алгоритм вставки нового элемента в очередь с приоритетом
<details> 
  <summary> 
	  <strong>[Теория]</strong>
  </summary>

***Очередь с приоритетами (англ. priority queue)*** — абстрактный контейнер, похожий на обычную очередь, но имеющий ряд особенностей:
* Каждому элементу очереди с приоритетами сопоставлено некоторое значение, именуемое приоритетом этого элемента. Приоритеты допускают сравнение друг с другом;
* Функция извлечения из очереди с приоритетами возвращает тот элемент, приоритет которого является максимальным.

Учащийся, выполняющий домашнее задание по нескольким предметам, может вводить различные показатели, определяющие порядок выполнения: от более любимых предметов к менее любимым, от менее сложных к более сложным, и так далее. Пожарная бригада планирует выезды сообразно с категорией сложности возгорания. Операционная система компьютера выделяет аппаратные ресурсы в первую очередь приложениям, запущенным с приоритетом реального времени, и лишь затем — остальным приложениям. Эти примеры позволяют пояснить назначение и принципы функционирования очередей с приоритетами.

На практике интерфейс очереди с приоритетом нередко расширяют другими операциями:
* Вернуть минимальный элемент без удаления из очереди
* Изменить приоритет произвольного элемента
* Удалить произвольный элемент
* Слить две очереди в одну

В индексированных очередях с приоритетом возможно обращение к элементам по индексу. Такие очереди могут быть использованы, например, для слияния нескольких отсортированных последовательностей (multiway merge).
Могут также рассматриваться очереди с приоритетом с двусторонним доступом (англ. double-ended priority queue, DEPQ), в которых есть операции доступа как к минимальному, так и к максимальному элементу.

**Очередь с приоритетами может быть реализована на основе различных структур данных**
<br>Простейшие (и не очень эффективные) реализации могут использовать неупорядоченный или упорядоченный ***Массив***, ***Связный список***, подходящие для небольших очередей. При этом вычисления могут быть как «ленивыми» (тяжесть вычислений переносится на извлечение элемента), так и ранними (eager), когда вставка элемента сложнее его извлечения. 

</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 32. Класс Бинарное дерево поиска. Реализация дерева на связанной структуре хранении. Реализовать метод определения высоты дерева
<details> 
  <summary> 
    <strong>[Depth.cpp]</strong>
  </summary>

Maximum/Minimum Depth [(maxDepth()/minDepth()] <br>The number of nodes along the longest/shortest path from the root node down to the farthest leaf node. <br>The maxDepth of the empty tree is 0.

```c++
struct Tree
{
  char data;
  Tree *left;
  Tree *right;  
  Tree *parent;  
};

int maxDepth(struct Tree *node)
{
  if(node == NULL || (node->left == NULL && node->right == NULL)) 
            return 0;

  int leftDepth = maxDepth(node->left);
  int rightDepth = maxDepth(node->right);

  return leftDepth > rightDepth ? 
        leftDepth + 1 : rightDepth + 1;
}

int minDepth(struct Tree *node)
{
  if(node == NULL || (node->left == NULL && node->right == NULL)) 
            return 0;

  int leftDepth = minDepth(node->left);
  int rightDepth = minDepth(node->right);

  return leftDepth < rightDepth ? 
        leftDepth + 1 : rightDepth + 1;
}
```
</details>

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 33. Класс Очередь. Представление в памяти на однонаправленном списк. Реализуйте метод вычисления значения выражения, заданного в префиксной форме

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 34. Дерево выражений. Свойства. Алгоритм формирования префиксной записи арифметического выражения

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 35. AVL дерево. Свойства. Алгоритм вставки нового узла в дерево

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 36. Класс Стек. Реализация на однонаправленном списке. Разработайте функцию для сложения двух целых чисел большой разрядности, представляя каждое число в объекте Стек

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 37. Линейный список - Очередь. АТД – очередь. Реализация очереди на связанном списке. Функции операций на вставки и удаления узлов очереди

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 38. Класс Двунаправленный список. Разработать метод, который определяет, симметричен ли список, т.е. элементы, отстоящие от левой и правой вершин на одинаковое расстояние равны

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 39. Класс Граф. Реализовать на матрице смежности. Реализовать поиск кратчайшего пути от одной заданной вершины к другой, используя матрицу Флойда

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 40. AVL дерево. Свойства. Алгоритм двойного поворота. Пример AVL дерева для балансировки которого требуется двойной поворот

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---

### 41. Дана последовательность ключей 1,2,3,4,5,6,7,8,9. Постройте бинарное дерево минимальной высоты с такими ключами

```html
  _________                     .__           ___________              __   
 /   _____/____    _____ ______ |  |   ____   \__    ___/___ ___  ____/  |_ 
 \_____  \\__  \  /     \\____ \|  | _/ __ \    |    |_/ __ \\  \/  /\   __\
 /        \/ __ \|  Y Y  \  |_> >  |_\  ___/    |    |\  ___/ >    <  |  |  
/_______  (____  /__|_|  /   __/|____/\___  >   |____| \___  >__/\_ \ |__|  
        \/     \/      \/|__|             \/               \/      \/       

```

**[:u6e80:к Началу](#Оглавление)**
<br>**[:u7121:к Середине](#20)**

---
