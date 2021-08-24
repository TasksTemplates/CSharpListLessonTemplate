Общая информация
В этой задаче требуется реализоват двусвязный список из первой части задачи в виде отдельного класса.
Задача
1.	Реализуйте двусвязный список в виде класса с заданным набором методов (см. раздел “Реализация”).
2.	Напишите тестовую программу

Реализация:
```cs  
class LinkedList 
{
    public LinkedList();
    public LinkedList(LinkedList other);
    //Возвращает первый элемент списка.
    public int Front();
    //Возвращает последний элемент списка.
    public int Back();
    //Возвращает истину, если значение value содержится в списке.
    public bool Contains(int value);
    //Возвращает количество вхождений значения value в список.
    public int Count(int value);
    //Возвращает размер списка.
    public int Size();
    //Возвращает истину, если список пуст.
    public bool Empty();
    //Удаляет элемент c номером position.
    public void Erase(uint posisition);
    //Удаляет элементы в интервале [begin, end).
    public void Erase(uint begin, uint end);
    //Очищает список.
    public void Clear();
    //Удаляет все вхождения value в список.
    public int Remove(int value);
    //Удаляет последний элемент списка.
    public void PopBack();
    //Удаляет первый элемент списка.
    public void PopFront();
    //Добавляет значение value в конец списка.
    public void PushBack(int value);
    //Добавляет значение value в начало списка.
    public void PushFront(int value);
    //Вставляет значение value перед элементом, на который указывает before
    public void Insert(uint position, int value);
};
```

Так же перегрузить метод Equals, позволяющий сравнить два списка. Внутри списка ещё реализовать свойство длинны списка, доступное только для чтения для классов вне списка.
