#### 1. Иерархия Collection Framework

![](https://github.com/Primisen/interview/blob/master/pictures/collection-hierarchy.png "")
________________________________________________________________________________________________________

![](https://github.com/Primisen/interview/blob/master/pictures/map-hierarchy.png "")

#### 2. Какие должны быть выполнены условия для элемента чтобы его можно было добавить в TreeSet?
Судя по всему класс  должен имплементировать интерфейс Comparable

#### 3. `Comparable` vs `Comparator`

Вообще эти два интерфейса нужны для сравнения объектов.
Разберем их отличия. 
__`Comparable`__
Есть интерфейс `Comparable` у которого есть метод `compareTo(T o)`. Реализуя этот метод в классе мы получаем 
возможность сравнивать между собой экземпляры этого класса. Этим методом пользуются некоторые коллекции, которые хранят элементы в отсортированном виде, как я понимаю.
Правила переопределения метода `compateTo(T o)` следующие:
* если объекты равны, то возвращаем 0
* если первый объект (на котором вызывается метод) больше чем второй, то возвращаем 1
* если первый объект меньше второго, то возвращаем -1

__`Comparator`__
Этот интерфейс реализовывается отдельным классом, который будет сравнивать два объекта одного класса. У интерфейса `Comparator` есть метод 
`compare(T o1, T o2)` в котором мы должны описать алгоритм сравнения (правила переопределения такие же как у compareTo(T o)). Дальше мы создаем экземпляр
этого класса-сравнителя и закидываем в метод сортировки коллекции. 


#### 4. `Iterable` vs `Iterator`
Интерфейс `Iterable` содержит в себе единственный метод `iterator()` который возвращает `Iterator`.

#### 5. Какие возникнут сложности в использовании HashMap, если мы неправильно переопределим equals() и hashCode()?

#### 6. HashMap, когда LinkedList перерастет в TreeSet?

#### 7. Виды деревьев

#### 8. Какие преимущества и недостатки красно-черного дерева?

#### 9. Как работате HashMap? 

#### 10. Что будет, если у объектов, которые мы хотим положить в  HashMap hashCode будет постоянным (42 например)?

#### 11. HashMap, что будет если ключ будет изменяемым объектом?

#### 12. Чем отличаются LinkedList и ArrayList, временная сложность операций этих коллекций.
