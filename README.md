Общая информация
В этой задаче требуется реализоват двусвязный список из первой части задачи в виде отдельного класса.
Задача
1.	Реализуйте двусвязный список в виде класса с заданным набором методов (см. раздел “Реализация”).
2.	Напишите тестовую программу

Реализация:
  class LinkedList {
    public LinkedList();
    public LinkedList(const LinkedList other);
    //Возвращает первый элемент списка.
    public int front();
    //Возвращает последний элемент списка.
    public int  back();
    //Возвращает истину, если значение value содержится в списке.
    public bool contains(const int  value);
    //Возвращает количество вхождений значения value в список.
    public int count(int value);
    //Возвращает размер списка.
    public int size();
    //Возвращает истину, если список пуст.
    public bool empty();
    //Удаляет элемент c номером position.
    public void erase(uint posisition);
    //Удаляет элементы в интервале [begin, end).
    public void erase(uint begin, uint end);
    //Очищает список.
    public void clear();
    //Удаляет все вхождения value в список.
    public int remove(int value);
    //Удаляет последний элемент списка.
    public void pop_back();
    //Удаляет первый элемент списка.
    public void pop_front();
    //Добавляет значение value в конец списка.
    public void push_back(int value);
    //Добавляет значение value в начало списка.
    public void push_front(int value);
    //Вставляет значение value перед элементом, на который указывает before
    public void insert(uint position, int value);
  };

Так же перегрузить метод Equals, позволяющий сравнить два списка. Внутри списка ещё реализовать свойство длинны списка, доступное только для чтения для классов вне списка.
