# Python OOP (Object-Oriented Programming) bo'yicha test savollari
---

## 1-VARIANT

**1.** Class nima?
```python
class Student:
    pass
```
A) O'zgaruvchi  
B) Funksiya  
C) Ob'yektlar uchun shablon  
D) Modul

**2.** Quyidagi kod natijasi nima?
```python
class Car:
    def __init__(self, model):
        self.model = model

car1 = Car("Toyota")
print(car1.model)
```
A) Car  
B) Toyota  
C) model  
D) Error

**3.** `__init__` metodi nima uchun ishlatiladi?
A) Ob'yektni o'chirish  
B) Ob'yektni yaratish va boshlang'ich qiymatlar berish  
C) Ob'yektni nusxalash  
D) Ob'yektni print qilish

**4.** `self` kalit so'zi nimani bildiradi?
A) Global o'zgaruvchi  
B) Joriy ob'yektga havola  
C) Class nomi  
D) Funksiya parametri

**5.** Quyidagi kod natijasi nima?
```python
class Person:
    count = 0
    def __init__(self, name):
        self.name = name
        Person.count += 1

p1 = Person("Ali")
p2 = Person("Vali")
print(Person.count)
```
A) 0  
B) 1  
C) 2  
D) Error

**6.** Instance variable va class variable farqi nima?
A) Farqi yo'q  
B) Instance - har bir ob'yektga tegishli, Class - barcha ob'yektlarga umumiy  
C) Instance - classga tegishli, Class - ob'yektga tegishli  
D) Ikkalasi ham bir xil

**7.** Quyidagi kod natijasi nima?
```python
class Animal:
    def speak(self):
        return "Sound"

class Dog(Animal):
    pass

d = Dog()
print(d.speak())
```
A) Error  
B) Sound  
C) Dog  
D) None

**8.** Inheritance (meros olish) nima?
A) Yangi class yaratish  
B) Bir classning xususiyatlarini boshqa class olishi  
C) Ob'yekt yaratish  
D) Metodlarni o'chirish

**9.** Quyidagi kod natijasi nima?
```python
class A:
    def __init__(self):
        self.x = 10

class B(A):
    def __init__(self):
        super().__init__()
        self.y = 20

b = B()
print(b.x + b.y)
```
A) 10  
B) 20  
C) 30  
D) Error

**10.** `super()` funksiyasi nima qiladi?
A) Ob'yektni o'chiradi  
B) Parent classga murojaat qiladi  
C) Yangi class yaratadi  
D) Metodlarni yashiradi

**11.** Quyidagi kod natijasi nima?
```python
class Math:
    @staticmethod
    def add(a, b):
        return a + b

print(Math.add(5, 3))
```
A) 8  
B) 53  
C) Error  
D) None

**12.** Static method nima?
A) Instance kerak bo'lgan metod  
B) Class yoki instance kerak bo'lmagan metod  
C) Faqat private metod  
D) Constructor metod

**13.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.__name = name
    
    def get_name(self):
        return self.__name

p = Person("John")
print(p.get_name())
```
A) Error  
B) John  
C) __name  
D) None

**14.** `__name` (double underscore) nimani bildiradi?
A) Public attribute  
B) Protected attribute  
C) Private attribute  
D) Static attribute

**15.** Quyidagi kod natijasi nima?
```python
class Rectangle:
    def __init__(self, w, h):
        self.width = w
        self.height = h
    
    def area(self):
        return self.width * self.height

r = Rectangle(5, 4)
print(r.area())
```
A) 9  
B) 20  
C) 5  
D) 4

**16.** Method overriding nima?
A) Metodlarni o'chirish  
B) Child classda parent metodini qayta yozish  
C) Bir nechta metod yaratish  
D) Metodlarni nusxalash

**17.** Quyidagi kod natijasi nima?
```python
class Animal:
    def sound(self):
        return "Some sound"

class Cat(Animal):
    def sound(self):
        return "Meow"

c = Cat()
print(c.sound())
```
A) Some sound  
B) Meow  
C) Error  
D) None

**18.** Quyidagi kod natijasi nima?
```python
class Counter:
    def __init__(self):
        self.count = 0
    
    def increment(self):
        self.count += 1
        return self.count

c = Counter()
c.increment()
c.increment()
print(c.count)
```
A) 0  
B) 1  
C) 2  
D) 3

**19.** Encapsulation nima?
A) Ma'lumotlarni yashirish va himoya qilish  
B) Klasslarni birlashtirish  
C) Ob'yektlarni nusxalash  
D) Metodlarni o'chirish

**20.** Quyidagi kod natijasi nima?
```python
class Book:
    def __init__(self, title, price):
        self.title = title
        self.price = price

b1 = Book("Python", 100)
b2 = Book("Java", 150)
print(b1.price + b2.price)
```
A) 100  
B) 150  
C) 250  
D) Error

**21.** Class method qanday aniqlanadi?
A) `@staticmethod`  
B) `@classmethod`  
C) `@method`  
D) `def method()`

**22.** Quyidagi kod natijasi nima?
```python
class Student:
    school = "MIT"
    
    @classmethod
    def change_school(cls, new_school):
        cls.school = new_school

Student.change_school("Harvard")
print(Student.school)
```
A) MIT  
B) Harvard  
C) Error  
D) None

**23.** Polymorphism nima?
A) Ko'p shakllilik  
B) Bitta shakl  
C) Klasslarni o'chirish  
D) Ob'yektlarni yaratish

**24.** Quyidagi kod natijasi nima?
```python
class Shape:
    def area(self):
        pass

class Square(Shape):
    def __init__(self, side):
        self.side = side
    
    def area(self):
        return self.side ** 2

s = Square(4)
print(s.area())
```
A) 4  
B) 8  
C) 16  
D) Error

**25.** `__str__` metodi nima uchun ishlatiladi?
A) Ob'yektni string ko'rinishida qaytarish  
B) Ob'yektni o'chirish  
C) Ob'yektni yaratish  
D) Ob'yektni nusxalash

**26.** Quyidagi kod natijasi nima?
```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __str__(self):
        return f"({self.x}, {self.y})"

p = Point(3, 4)
print(p)
```
A) Point  
B) (3, 4)  
C) Error  
D) <Point object>

**27.** Multiple inheritance nima?
A) Bir classdan meros olish  
B) Bir nechta classdan meros olish  
C) Ob'yekt yaratish  
D) Metodlarni o'chirish

**28.** Quyidagi kod natijasi nima?
```python
class A:
    x = 10

class B:
    y = 20

class C(A, B):
    pass

c = C()
print(c.x + c.y)
```
A) 10  
B) 20  
C) 30  
D) Error

**29.** `__init__` metodisiz class yaratsa bo'ladimi?
A) Yo'q, har doim kerak  
B) Ha, bo'ladi  
C) Faqat inheritance bilan  
D) Faqat static method bilan

**30.** Quyidagi kod natijasi nima?
```python
class Car:
    wheels = 4

c1 = Car()
c2 = Car()
Car.wheels = 6
print(c1.wheels + c2.wheels)
```
A) 8  
B) 10  
C) 12  
D) Error

**31.** Property decorator nima uchun ishlatiladi?
A) Metodlarni attribut kabi ishlatish  
B) Klasslarni yaratish  
C) Ob'yektlarni o'chirish  
D) Static metodlar yaratish

**32.** Quyidagi kod natijasi nima?
```python
class Circle:
    def __init__(self, radius):
        self._radius = radius
    
    @property
    def radius(self):
        return self._radius

c = Circle(5)
print(c.radius)
```
A) Error  
B) 5  
C) _radius  
D) None

**33.** Abstract class nima?
A) To'liq tayyor class  
B) Instance yaratib bo'lmaydigan, faqat meros beruvchi class  
C) Oddiy class  
D) Static class

**34.** Quyidagi kod natijasi nima?
```python
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary

e1 = Employee("Ali", 1000)
e2 = Employee("Vali", 1500)
print(e1.salary < e2.salary)
```
A) True  
B) False  
C) Error  
D) None

**35.** `__repr__` va `__str__` farqi nima?
A) Farqi yo'q  
B) `__repr__` - debugging uchun, `__str__` - foydalanuvchi uchun  
C) `__str__` - debugging uchun, `__repr__` - foydalanuvchi uchun  
D) Ikkalasi ham bir xil

**36.** Quyidagi kod natijasi nima?
```python
class Box:
    def __init__(self, length):
        self.length = length
    
    def __add__(self, other):
        return self.length + other.length

b1 = Box(10)
b2 = Box(20)
print(b1 + b2)
```
A) Error  
B) 30  
C) Box  
D) None

**37.** Operator overloading nima?
A) Operatorlarning o'zini o'zgartirish  
B) Operatorlarga yangi ma'no berish  
C) Operatorlarni o'chirish  
D) Yangi operator yaratish

**38.** Quyidagi kod natijasi nima?
```python
class Number:
    def __init__(self, value):
        self.value = value
    
    def __eq__(self, other):
        return self.value == other.value

n1 = Number(5)
n2 = Number(5)
print(n1 == n2)
```
A) True  
B) False  
C) Error  
D) None

**39.** Composition nima?
A) Klasslarni birlashtirish  
B) Bir ob'yekt ichida boshqa ob'yekt yaratish  
C) Meros olish  
D) Metodlarni nusxalash

**40.** Quyidagi kod natijasi nima?
```python
class Engine:
    def __init__(self, power):
        self.power = power

class Car:
    def __init__(self, model, power):
        self.model = model
        self.engine = Engine(power)

c = Car("Toyota", 150)
print(c.engine.power)
```
A) Toyota  
B) 150  
C) Engine  
D) Error

**41.** Class ichida class yaratsa bo'ladimi?
A) Yo'q  
B) Ha  
C) Faqat inheritance bilan  
D) Faqat static bilan

**42.** Quyidagi kod natijasi nima?
```python
class Outer:
    class Inner:
        def __init__(self, value):
            self.value = value

i = Outer.Inner(100)
print(i.value)
```
A) Outer  
B) Inner  
C) 100  
D) Error

**43.** `hasattr()` funksiyasi nima qiladi?
A) Ob'yektni o'chiradi  
B) Ob'yektda attribut bor-yo'qligini tekshiradi  
C) Attribut qo'shadi  
D) Attribut o'chiradi

**44.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.name = name

p = Person("Ali")
print(hasattr(p, "name"))
```
A) True  
B) False  
C) Ali  
D) Error

**45.** `getattr()` funksiyasi nima qiladi?
A) Attributni o'chiradi  
B) Attribut qiymatini oladi  
C) Attribut qo'shadi  
D) Ob'yektni yaratadi

**46.** Quyidagi kod natijasi nima?
```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

s = Student("John", 20)
print(getattr(s, "age"))
```
A) Student  
B) John  
C) 20  
D) Error

**47.** `isinstance()` funksiyasi nima uchun ishlatiladi?
A) Ob'yekt yaratish  
B) Ob'yekt ma'lum classga tegishli yoki yo'qligini tekshirish  
C) Class yaratish  
D) Metodlarni tekshirish

**48.** Quyidagi kod natijasi nima?
```python
class Animal:
    pass

class Dog(Animal):
    pass

d = Dog()
print(isinstance(d, Animal))
```
A) True  
B) False  
C) Dog  
D) Error

**49.** `__len__` metodi nima qiladi?
A) Ob'yektni o'chiradi  
B) `len()` funksiyasi uchun qaytariladigan qiymatni belgilaydi  
C) Ob'yekt yaratadi  
D) String qaytaradi

**50.** Quyidagi kod natijasi nima?
```python
class MyList:
    def __init__(self, items):
        self.items = items
    
    def __len__(self):
        return len(self.items)

ml = MyList([1, 2, 3, 4, 5])
print(len(ml))
```
A) MyList  
B) [1, 2, 3, 4, 5]  
C) 5  
D) Error

---

## 2-VARIANT

**1.** Quyidagi kod natijasi nima?
```python
class Phone:
    def __init__(self, brand):
        self.brand = brand

p = Phone("Samsung")
print(p.brand)
```
A) Phone  
B) Samsung  
C) brand  
D) Error

**2.** Class attribute va instance attribute farqi nima?
A) Farqi yo'q  
B) Class - barcha ob'yektlarga, Instance - har biriga alohida  
C) Instance - barcha ob'yektlarga, Class - har biriga alohida  
D) Ikkalasi ham bir xil

**3.** Quyidagi kod natijasi nima?
```python
class Counter:
    total = 0
    def __init__(self):
        Counter.total += 1

c1 = Counter()
c2 = Counter()
c3 = Counter()
print(Counter.total)
```
A) 0  
B) 1  
C) 2  
D) 3

**4.** Quyidagi kod natijasi nima?
```python
class Vehicle:
    def move(self):
        return "Moving"

class Bike(Vehicle):
    def move(self):
        return "Riding"

b = Bike()
print(b.move())
```
A) Moving  
B) Riding  
C) Vehicle  
D) Error

**5.** Method overriding qachon sodir bo'ladi?
A) Bir xil nomli metodlar bir classda  
B) Child class parent class metodini qayta yozganda  
C) Metodlarni o'chirganda  
D) Yangi class yaratganda

**6.** Quyidagi kod natijasi nima?
```python
class A:
    def __init__(self):
        self.x = 5

class B(A):
    def __init__(self):
        super().__init__()
        self.x = 10

b = B()
print(b.x)
```
A) 5  
B) 10  
C) 15  
D) Error

**7.** `super()` ni qachon ishlatamiz?
A) Ob'yekt yaratganda  
B) Parent class metodlarini chaqirganda  
C) Klassni o'chirganda  
D) Metodlarni yaratganda

**8.** Quyidagi kod natijasi nima?
```python
class Calculator:
    @staticmethod
    def multiply(a, b):
        return a * b

print(Calculator.multiply(4, 5))
```
A) 9  
B) 20  
C) 45  
D) Error

**9.** Static method va instance method farqi nima?
A) Farqi yo'q  
B) Static - self kerak emas, Instance - self kerak  
C) Static - self kerak, Instance - self kerak emas  
D) Ikkalasi ham bir xil

**10.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self._name = name
    
    @property
    def name(self):
        return self._name

p = Person("Ali")
print(p.name)
```
A) _name  
B) Ali  
C) Error  
D) None

**11.** `@property` decorator nima qiladi?
A) Metodlarni static qiladi  
B) Metodlarni attribut kabi ishlatish imkonini beradi  
C) Klasslarni yaratadi  
D) Ob'yektlarni o'chiradi

**12.** Quyidagi kod natijasi nima?
```python
class Square:
    def __init__(self, side):
        self.side = side
    
    def perimeter(self):
        return 4 * self.side

s = Square(5)
print(s.perimeter())
```
A) 5  
B) 10  
C) 20  
D) 25

**13.** Private attribute qanday yaratiladi?
A) `name`  
B) `_name`  
C) `__name`  
D) `name_`

**14.** Quyidagi kod natijasi nima?
```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance
    
    def get_balance(self):
        return self.__balance

acc = BankAccount(1000)
print(acc.get_balance())
```
A) Error  
B) 1000  
C) __balance  
D) None

**15.** Encapsulation nimani ta'minlaydi?
A) Ma'lumotlarni himoya qilish  
B) Klasslarni birlashtirish  
C) Ob'yektlarni yaratish  
D) Metodlarni o'chirish

**16.** Quyidagi kod natijasi nima?
```python
class Product:
    def __init__(self, name, price):
        self.name = name
        self.price = price

p1 = Product("Book", 50)
p2 = Product("Pen", 10)
print(p1.price - p2.price)
```
A) 40  
B) 50  
C) 60  
D) Error

**17.** Class method qanday aniqlanadi?
A) Oddiy metod kabi  
B) `@classmethod` decorator bilan  
C) `@staticmethod` decorator bilan  
D) `@method` decorator bilan

**18.** Quyidagi kod natijasi nima?
```python
class Student:
    count = 0
    
    @classmethod
    def increment(cls):
        cls.count += 1

Student.increment()
Student.increment()
print(Student.count)
```
A) 0  
B) 1  
C) 2  
D) Error

**19.** Quyidagi kod natijasi nima?
```python
class Triangle:
    def __init__(self, base, height):
        self.base = base
        self.height = height
    
    def area(self):
        return 0.5 * self.base * self.height

t = Triangle(10, 6)
print(t.area())
```
A) 16  
B) 30  
C) 60  
D) 30.0

**20.** Polymorphism qanday amalga oshiriladi?
A) Bir xil nomli metodlar turli classlarda  
B) Bir xil classda bir xil metodlar  
C) Turli nomdagi metodlar  
D) Static metodlar orqali

**21.** Quyidagi kod natijasi nima?
```python
class Animal:
    def sound(self):
        return "Sound"

class Dog(Animal):
    def sound(self):
        return "Bark"

class Cat(Animal):
    def sound(self):
        return "Meow"

animals = [Dog(), Cat()]
for a in animals:
    print(a.sound(), end=" ")
```
A) Sound Sound  
B) Bark Meow  
C) Dog Cat  
D) Error

**22.** `__str__` metodini qachon chaqiriladi?
A) Ob'yekt yaratilganda  
B) `print()` yoki `str()` ishlatilganda  
C) Ob'yekt o'chirilganda  
D) Metod chaqirilganda

**23.** Quyidagi kod natijasi nima?
```python
class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = author
    
    def __str__(self):
        return f"{self.title} by {self.author}"

b = Book("Python", "Guido")
print(b)
```
A) Book  
B) Python by Guido  
C) Error  
D) <Book object>

**24.** Multiple inheritance qanday amalga oshiriladi?
A) `class C(A, B):`  
B) `class C extends A, B:`  
C) `class C inherits A, B:`  
D) `class C: A, B`

**25.** Quyidagi kod natijasi nima?
```python
class X:
    a = 5

class Y:
    b = 10

class Z(X, Y):
    c = 15

z = Z()
print(z.a + z.b + z.c)
```
A) 15  
B) 20  
C) 30  
D) Error

**26.** Quyidagi kod natijasi nima?
```python
class Temperature:
    def __init__(self, celsius):
        self.celsius = celsius
    
    @property
    def fahrenheit(self):
        return (self.celsius * 9/5) + 32

t = Temperature(0)
print(t.fahrenheit)
```
A) 0  
B) 32  
C) 32.0  
D) Error

**27.** Property setter qanday yaratiladi?
A) `@property.setter`  
B) `@setter`  
C) `@set`  
D) Yaratib bo'lmaydi

**28.** Quyidagi kod natijasi nima?
```python
class Circle:
    def __init__(self, radius):
        self._radius = radius
    
    @property
    def radius(self):
        return self._radius
    
    @radius.setter
    def radius(self, value):
        if value > 0:
            self._radius = value

c = Circle(5)
c.radius = 10
print(c.radius)
```
A) 5  
B) 10  
C) Error  
D) None

**29.** Operator overloading uchun qaysi metodlar ishlatiladi?
A) `__add__`, `__sub__`, `__mul__`  
B) `add()`, `sub()`, `mul()`  
C) `+`, `-`, `*`  
D) `@operator`

**30.** Quyidagi kod natijasi nima?
```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __add__(self, other):
        return Vector(self.x + other.x, self.y + other.y)

v1 = Vector(1, 2)
v2 = Vector(3, 4)
v3 = v1 + v2
print(v3.x, v3.y)
```
A) 1 2  
B) 3 4  
C) 4 6  
D) Error

**31.** `__eq__` metodi nima uchun ishlatiladi?
A) Qo'shish operatori  
B) Tenglik operatori  
C) Ayirish operatori  
D) Ko'paytirish operatori

**32.** Quyidagi kod natijasi nima?
```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __eq__(self, other):
        return self.x == other.x and self.y == other.y

p1 = Point(3, 4)
p2 = Point(3, 4)
print(p1 == p2)
```
A) True  
B) False  
C) Error  
D) None

**33.** Composition nima?
A) Meros olish  
B) Bir ob'yekt ichida boshqa ob'yekt yaratish  
C) Klasslarni birlashtirish  
D) Metodlarni qayta yozish

**34.** Quyidagi kod natijasi nima?
```python
class CPU:
    def __init__(self, cores):
        self.cores = cores

class Computer:
    def __init__(self, cpu_cores):
        self.cpu = CPU(cpu_cores)

c = Computer(8)
print(c.cpu.cores)
```
A) CPU  
B) Computer  
C) 8  
D) Error

**35.** `isinstance()` funksiyasi nima qaytaradi?
A) Class nomi  
B) True yoki False  
C) Ob'yekt  
D) None

**36.** Quyidagi kod natijasi nima?
```python
class Shape:
    pass

class Circle(Shape):
    pass

c = Circle()
print(isinstance(c, Shape))
```
A) True  
B) False  
C) Circle  
D) Error

**37.** `issubclass()` funksiyasi nima tekshiradi?
A) Ob'yekt class ga tegishli yoki yo'qligini  
B) Bir class boshqa classdan meros olgan yoki yo'qligini  
C) Metodlarni  
D) Attributlarni

**38.** Quyidagi kod natijasi nima?
```python
class Animal:
    pass

class Dog(Animal):
    pass

print(issubclass(Dog, Animal))
```
A) True  
B) False  
C) Dog  
D) Error

**39.** `hasattr()`, `getattr()`, `setattr()` nima qiladi?
A) Ob'yektlarni yaratadi  
B) Attributlar bilan ishlash funksiyalari  
C) Metodlarni chaqiradi  
D) Klasslarni yaratadi

**40.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.name = name

p = Person("Ali")
setattr(p, "age", 25)
print(getattr(p, "age"))
```
A) Ali  
B) 25  
C) Error  
D) None

**41.** `delattr()` funksiyasi nima qiladi?
A) Attribut qo'shadi  
B) Attributni o'chiradi  
C) Attributni o'zgartiradi  
D) Attributni tekshiradi

**42.** Quyidagi kod natijasi nima?
```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

s = Student("John", 20)
delattr(s, "age")
print(hasattr(s, "age"))
```
A) True  
B) False  
C) 20  
D) Error

**43.** `__len__` metodi qachon chaqiriladi?
A) Ob'yekt yaratilganda  
B) `len()` funksiyasi ishlatilganda  
C) `print()` ishlatilganda  
D) Ob'yekt o'chirilganda

**44.** Quyidagi kod natijasi nima?
```python
class Stack:
    def __init__(self):
        self.items = []
    
    def __len__(self):
        return len(self.items)
    
    def push(self, item):
        self.items.append(item)

s = Stack()
s.push(10)
s.push(20)
print(len(s))
```
A) 0  
B) 1  
C) 2  
D) Error

**45.** `__repr__` metodi nima uchun ishlatiladi?
A) Foydalanuvchi uchun string  
B) Developer uchun string (debugging)  
C) Ob'yektni o'chirish  
D) Ob'yektni yaratish

**46.** Quyidagi kod natijasi nima?
```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def __repr__(self):
        return f"Point({self.x}, {self.y})"

p = Point(5, 10)
print(repr(p))
```
A) Point  
B) Point(5, 10)  
C) (5, 10)  
D) Error

**47.** Class ichida class (nested class) yaratsa bo'ladimi?
A) Yo'q  
B) Ha  
C) Faqat static bilan  
D) Faqat inheritance bilan

**48.** Quyidagi kod natijasi nima?
```python
class University:
    class Department:
        def __init__(self, name):
            self.name = name

d = University.Department("CS")
print(d.name)
```
A) University  
B) Department  
C) CS  
D) Error

**49.** `__call__` metodi nimani amalga oshiradi?
A) Ob'yektni funksiya kabi chaqirish  
B) Ob'yektni yaratish  
C) Ob'yektni o'chirish  
D) Metodlarni chaqirish

**50.** Quyidagi kod natijasi nima?
```python
class Multiplier:
    def __init__(self, factor):
        self.factor = factor
    
    def __call__(self, x):
        return x * self.factor

m = Multiplier(5)
print(m(10))
```
A) 5  
B) 10  
C) 50  
D) Error

---

## 3-VARIANT

**1.** Quyidagi kod natijasi nima?
```python
class Laptop:
    def __init__(self, brand, ram):
        self.brand = brand
        self.ram = ram

l = Laptop("Dell", 16)
print(l.ram)
```
A) Dell  
B) 16  
C) Laptop  
D) Error

**2.** Quyidagi kod natijasi nima?
```python
class Database:
    connections = 0
    
    def __init__(self):
        Database.connections += 1

d1 = Database()
d2 = Database()
print(Database.connections)
```
A) 0  
B) 1  
C) 2  
D) Error

**3.** Inheritance nima uchun ishlatiladi?
A) Kod takrorlashni kamaytirish  
B) Klasslarni o'chirish  
C) Ob'yektlarni yaratish  
D) Metodlarni yashirish

**4.** Quyidagi kod natijasi nima?
```python
class Parent:
    def greet(self):
        return "Hello from Parent"

class Child(Parent):
    pass

c = Child()
print(c.greet())
```
A) Error  
B) Hello from Parent  
C) Hello from Child  
D) None

**5.** Quyidagi kod natijasi nima?
```python
class A:
    def __init__(self):
        self.value = 100

class B(A):
    def __init__(self):
        super().__init__()
        self.value += 50

b = B()
print(b.value)
```
A) 50  
B) 100  
C) 150  
D) Error

**6.** `super()` funksiyasini ishlatmasak nima bo'ladi?
A) Parent class `__init__` chaqirilmaydi  
B) Xato beradi  
C) Hech narsa  
D) Child class ishlamaydi

**7.** Quyidagi kod natijasi nima?
```python
class Math:
    @staticmethod
    def power(x, n):
        return x ** n

print(Math.power(2, 3))
```
A) 5  
B) 6  
C) 8  
D) Error

**8.** Static method qachon ishlatiladi?
A) Instance bilan bog'liq bo'lmagan amallar uchun  
B) Har doim  
C) Faqat inheritance bilan  
D) Ob'yekt yaratganda

**9.** Quyidagi kod natijasi nima?
```python
class Employee:
    company = "ABC Corp"
    
    @classmethod
    def get_company(cls):
        return cls.company

print(Employee.get_company())
```
A) Employee  
B) ABC Corp  
C) Error  
D) None

**10.** Class method va static method farqi nima?
A) Farqi yo'q  
B) Class method `cls` oladi, static method hech narsa olmaydi  
C) Static method `cls` oladi, class method olmaydi  
D) Ikkalasi ham bir xil

**11.** Quyidagi kod natijasi nima?
```python
class Rectangle:
    def __init__(self, width, height):
        self._width = width
        self._height = height
    
    @property
    def area(self):
        return self._width * self._height

r = Rectangle(5, 10)
print(r.area)
```
A) 15  
B) 50  
C) Error  
D) None

**12.** Property nima uchun ishlatiladi?
A) Metodlarni attribut kabi chaqirish  
B) Static metod yaratish  
C) Klasslarni yaratish  
D) Ob'yektlarni o'chirish

**13.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.__name = name
    
    def get_name(self):
        return self.__name
    
    def set_name(self, name):
        self.__name = name

p = Person("Ali")
p.set_name("Vali")
print(p.get_name())
```
A) Ali  
B) Vali  
C) Error  
D) None

**14.** Private attribute ga to'g'ridan-to'g'ri murojaat qilsak nima bo'ladi?
A) Xato beradi  
B) Ishlaydi  
C) Name mangling bo'ladi  
D) None qaytaradi

**15.** Quyidagi kod natijasi nima?
```python
class Item:
    def __init__(self, name, price, quantity):
        self.name = name
        self.price = price
        self.quantity = quantity
    
    def total(self):
        return self.price * self.quantity

i = Item("Book", 50, 3)
print(i.total())
```
A) 50  
B) 53  
C) 150  
D) Error

**16.** Quyidagi kod natijasi nima?
```python
class Shape:
    def draw(self):
        return "Drawing shape"

class Circle(Shape):
    def draw(self):
        return "Drawing circle"

c = Circle()
print(c.draw())
```
A) Drawing shape  
B) Drawing circle  
C) Error  
D) None

**17.** Method overriding polymorphism ga misol bo'la oladimi?
A) Yo'q  
B) Ha  
C) Faqat static metodda  
D) Faqat class metodda

**18.** Quyidagi kod natijasi nima?
```python
class Account:
    def __init__(self, balance):
        self.balance = balance
    
    def deposit(self, amount):
        self.balance += amount
        return self.balance

acc = Account(100)
acc.deposit(50)
print(acc.balance)
```
A) 100  
B) 50  
C) 150  
D) Error

**19.** `__str__` va `__repr__` farqi nimada?
A) Farqi yo'q  
B) `__str__` - user friendly, `__repr__` - developer friendly  
C) `__repr__` - user friendly, `__str__` - developer friendly  
D) Ikkalasi ham bir xil

**20.** Quyidagi kod natijasi nima?
```python
class Student:
    def __init__(self, name, grade):
        self.name = name
        self.grade = grade
    
    def __str__(self):
        return f"{self.name}: {self.grade}"
    
    def __repr__(self):
        return f"Student('{self.name}', {self.grade})"

s = Student("Ali", 90)
print(str(s))
```
A) Student('Ali', 90)  
B) Ali: 90  
C) Ali  
D) Error

**21.** Multiple inheritance da MRO nima?
A) Method Resolution Order  
B) Multiple Resolution Object  
C) Method Return Order  
D) Multiple Return Object

**22.** Quyidagi kod natijasi nima?
```python
class A:
    x = 1

class B:
    x = 2

class C(A, B):
    pass

c = C()
print(c.x)
```
A) 1  
B) 2  
C) 3  
D) Error

**23.** Quyidagi kod natijasi nima?
```python
class Distance:
    def __init__(self, meters):
        self.meters = meters
    
    def __add__(self, other):
        return Distance(self.meters + other.meters)

d1 = Distance(100)
d2 = Distance(200)
d3 = d1 + d2
print(d3.meters)
```
A) 100  
B) 200  
C) 300  
D) Error

**24.** Operator overloading uchun nechta maxsus metod bor?
A) 5 ta  
B) 10 ta  
C) 20+ ta  
D) Cheklanmagan

**25.** Quyidagi kod natijasi nima?
```python
class Number:
    def __init__(self, value):
        self.value = value
    
    def __lt__(self, other):
        return self.value < other.value

n1 = Number(5)
n2 = Number(10)
print(n1 < n2)
```
A) True  
B) False  
C) Error  
D) None

**26.** `__lt__`, `__le__`, `__gt__`, `__ge__` metodlari nima uchun?
A) Arifmetik operatorlar  
B) Taqqoslash operatorlari  
C) Mantiqiy operatorlar  
D) String operatorlar

**27.** Quyidagi kod natijasi nima?
```python
class Battery:
    def __init__(self, capacity):
        self.capacity = capacity

class Phone:
    def __init__(self, model, battery_capacity):
        self.model = model
        self.battery = Battery(battery_capacity)

p = Phone("iPhone", 3000)
print(p.battery.capacity)
```
A) iPhone  
B) 3000  
C) Battery  
D) Error

**28.** Composition va Inheritance farqi nima?
A) Farqi yo'q  
B) Composition - "has-a", Inheritance - "is-a" munosabat  
C) Composition - "is-a", Inheritance - "has-a" munosabat  
D) Ikkalasi ham bir xil

**29.** Quyidagi kod natijasi nima?
```python
class Animal:
    pass

class Dog(Animal):
    pass

d = Dog()
print(isinstance(d, Dog) and isinstance(d, Animal))
```
A) True  
B) False  
C) Error  
D) None

**30.** `type()` va `isinstance()` farqi nima?
A) Farqi yo'q  
B) `type()` - aniq class, `isinstance()` - class va parent classlar  
C) `isinstance()` - aniq class, `type()` - barcha classlar  
D) Ikkalasi ham bir xil

**31.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p = Person("Ali", 25)
print(hasattr(p, "name") and hasattr(p, "age"))
```
A) True  
B) False  
C) Error  
D) None

**32.** Quyidagi kod natijasi nima?
```python
class Car:
    def __init__(self, brand):
        self.brand = brand

c = Car("Toyota")
setattr(c, "model", "Camry")
print(c.model)
```
A) Toyota  
B) Camry  
C) Error  
D) None

**33.** `__getitem__` metodi nima uchun ishlatiladi?
A) Ob'yektni index orqali olish  
B) Ob'yektni yaratish  
C) Ob'yektni o'chirish  
D) Ob'yektni print qilish

**34.** Quyidagi kod natijasi nima?
```python
class MyList:
    def __init__(self):
        self.items = [1, 2, 3, 4, 5]
    
    def __getitem__(self, index):
        return self.items[index]

ml = MyList()
print(ml[2])
```
A) 1  
B) 2  
C) 3  
D) Error

**35.** `__setitem__` metodi nima qiladi?
A) Index orqali qiymat o'rnatish  
B) Ob'yekt yaratish  
C) Ob'yekt o'chirish  
D) Ob'yekt nusxalash

**36.** Quyidagi kod natijasi nima?
```python
class Dictionary:
    def __init__(self):
        self.data = {}
    
    def __setitem__(self, key, value):
        self.data[key] = value
    
    def __getitem__(self, key):
        return self.data[key]

d = Dictionary()
d["name"] = "Ali"
print(d["name"])
```
A) Dictionary  
B) Ali  
C) name  
D) Error

**37.** `__contains__` metodi nima uchun ishlatiladi?
A) `in` operatori uchun  
B) `not` operatori uchun  
C) `and` operatori uchun  
D) `or` operatori uchun

**38.** Quyidagi kod natijasi nima?
```python
class NumberSet:
    def __init__(self, numbers):
        self.numbers = numbers
    
    def __contains__(self, item):
        return item in self.numbers

ns = NumberSet([1, 2, 3, 4, 5])
print(3 in ns)
```
A) True  
B) False  
C) Error  
D) None

**39.** `__iter__` va `__next__` metodlari nima uchun?
A) Ob'yektni iterable qilish  
B) Ob'yektni yaratish  
C) Ob'yektni o'chirish  
D) Ob'yektni print qilish

**40.** Quyidagi kod natijasi nima?
```python
class Counter:
    def __init__(self, start, end):
        self.current = start
        self.end = end
    
    def __iter__(self):
        return self
    
    def __next__(self):
        if self.current >= self.end:
            raise StopIteration
        self.current += 1
        return self.current - 1

c = Counter(1, 4)
print(list(c))
```
A) [1, 2, 3]  
B) [1, 2, 3, 4]  
C) [0, 1, 2, 3]  
D) Error

**41.** Abstract method nima?
A) To'liq metod  
B) Faqat signature bo'lgan, implementation yo'q metod  
C) Static metod  
D) Class metod

**42.** Quyidagi kod to'g'ri ishlash uchun nima kerak?
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    
    # Nima kerak?
```
A) `__init__` metodi  
B) `area()` metodini implement qilish  
C) `__str__` metodi  
D) Hech narsa

**43.** Duck typing nima?
A) Ob'yektning turi emas, xatti-harakati muhim  
B) Faqat ma'lum turlar bilan ishlash  
C) Type checking  
D) Class checking

**44.** Quyidagi kod ishlash uchun ob'yekt qanday bo'lishi kerak?
```python
def make_sound(animal):
    print(animal.sound())

# animal da nima bo'lishi kerak?
```
A) Animal classdan bo'lishi kerak  
B) `sound()` metodi bo'lishi kifoya  
C) Dog classdan bo'lishi kerak  
D) Parent class kerak

**45.** Context manager nima?
A) `with` statement bilan ishlaydigan ob'yekt  
B) Oddiy class  
C) Static class  
D) Abstract class

**46.** Context manager uchun qaysi metodlar kerak?
A) `__init__` va `__del__`  
B) `__enter__` va `__exit__`  
C) `__start__` va `__stop__`  
D) `__open__` va `__close__`

**47.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.name = name
    
    def __del__(self):
        print(f"{self.name} deleted")

p = Person("Ali")
del p
```
A) Hech narsa  
B) Ali deleted  
C) Error  
D) None

**48.** `__del__` metodi qachon chaqiriladi?
A) Ob'yekt yaratilganda  
B) Ob'yekt o'chirilganda  
C) Metod chaqirilganda  
D) Print qilinganda

**49.** Singleton pattern nima?
A) Bir classdan faqat bitta ob'yekt yaratish  
B) Ko'p ob'yekt yaratish  
C) Ob'yektlarni nusxalash  
D) Klasslarni birlashtirish

**50.** Quyidagi kod natijasi nima?
```python
class Calculator:
    def __init__(self, value):
        self.value = value
    
    def __call__(self, x):
        return self.value + x

calc = Calculator(10)
print(calc(5))
```
A) 10  
B) 5  
C) 15  
D) Error

---

## 4-VARIANT

**1.** Quyidagi kod natijasi nima?
```python
class Monitor:
    def __init__(self, size, resolution):
        self.size = size
        self.resolution = resolution

m = Monitor(24, "1920x1080")
print(m.size)
```
A) Monitor  
B) 24  
C) 1920x1080  
D) Error

**2.** Class variable va instance variable qachon ishlatiladi?
A) Class - barcha ob'yektlar uchun umumiy, Instance - har biriga alohida  
B) Farqi yo'q  
C) Instance - umumiy, Class - alohida  
D) Ikkalasi ham bir xil

**3.** Quyidagi kod natijasi nima?
```python
class Server:
    active_connections = 0
    
    def __init__(self):
        Server.active_connections += 1
    
    def __del__(self):
        Server.active_connections -= 1

s1 = Server()
s2 = Server()
print(Server.active_connections)
```
A) 0  
B) 1  
C) 2  
D) Error

**4.** Quyidagi kod natijasi nima?
```python
class Device:
    def turn_on(self):
        return "Device on"

class TV(Device):
    def turn_on(self):
        return "TV on"

tv = TV()
print(tv.turn_on())
```
A) Device on  
B) TV on  
C) Error  
D) None

**5.** Child class parent classning barcha metodlariga kirish huquqiga egami?
A) Yo'q  
B) Ha, public va protected metodlarga  
C) Faqat public metodlarga  
D) Faqat protected metodlarga

**6.** Quyidagi kod natijasi nima?
```python
class Base:
    def __init__(self):
        self.x = 10

class Derived(Base):
    def __init__(self):
        super().__init__()
        self.y = 20
    
    def sum(self):
        return self.x + self.y

d = Derived()
print(d.sum())
```
A) 10  
B) 20  
C) 30  
D) Error

**7.** `super()` ishlatmasdan ham parent classni chaqirsa bo'ladimi?
A) Yo'q  
B) Ha, `ParentClass.__init__(self)` orqali  
C) Faqat Python 2 da  
D) Hech qachon

**8.** Quyidagi kod natijasi nima?
```python
class Utils:
    @staticmethod
    def divide(a, b):
        return a / b if b != 0 else "Error"

print(Utils.divide(10, 2))
```
A) 2  
B) 5  
C) 5.0  
D) Error

**9.** Static method instance yaratmasdan chaqirilishi mumkinmi?
A) Yo'q  
B) Ha  
C) Faqat inheritance bilan  
D) Faqat composition bilan

**10.** Quyidagi kod natijasi nima?
```python
class Company:
    name = "TechCorp"
    
    @classmethod
    def set_name(cls, new_name):
        cls.name = new_name
    
    @classmethod
    def get_name(cls):
        return cls.name

Company.set_name("CodeCorp")
print(Company.get_name())
```
A) TechCorp  
B) CodeCorp  
C) Error  
D) None

**11.** Class method `cls` parametri nimani bildiradi?
A) Instance  
B) Classning o'zini  
C) Parent class  
D) Metod nomi

**12.** Quyidagi kod natijasi nima?
```python
class Box:
    def __init__(self, length, width, height):
        self.length = length
        self.width = width
        self.height = height
    
    @property
    def volume(self):
        return self.length * self.width * self.height

b = Box(2, 3, 4)
print(b.volume)
```
A) 9  
B) 24  
C) Error  
D) None

**13.** Property setter va getter nima uchun ishlatiladi?
A) Attributlarga nazoratli kirish  
B) Metodlarni yashirish  
C) Klasslarni yaratish  
D) Ob'yektlarni o'chirish

**14.** Quyidagi kod natijasi nima?
```python
class User:
    def __init__(self, username):
        self.__username = username
    
    @property
    def username(self):
        return self.__username
    
    @username.setter
    def username(self, value):
        if len(value) >= 3:
            self.__username = value

u = User("ab")
u.username = "admin"
print(u.username)
```
A) ab  
B) admin  
C) Error  
D) None

**15.** Quyidagi kod natijasi nima?
```python
class Order:
    def __init__(self, items):
        self.items = items
    
    def total_items(self):
        return len(self.items)

o = Order(["item1", "item2", "item3"])
print(o.total_items())
```
A) 1  
B) 2  
C) 3  
D) Error

**16.** Polymorphism qaysi holatlarda ko'rinadi?
A) Method overriding  
B) Operator overloading  
C) Duck typing  
D) Barchasi to'g'ri

**17.** Quyidagi kod natijasi nima?
```python
def process(obj):
    return obj.calculate()

class A:
    def calculate(self):
        return 10

class B:
    def calculate(self):
        return 20

print(process(A()) + process(B()))
```
A) 10  
B) 20  
C) 30  
D) Error

**18.** `__str__` metodini yozmasak `print()` nima chiqaradi?
A) Error  
B) Ob'yektning xotira manzili  
C) Class nomi  
D) None

**19.** Quyidagi kod natijasi nima?
```python
class Product:
    def __init__(self, name, price):
        self.name = name
        self.price = price
    
    def __str__(self):
        return f"{self.name}: ${self.price}"

p = Product("Laptop", 1000)
print(p)
```
A) Product  
B) Laptop: $1000  
C) Error  
D) <Product object>

**20.** `__repr__` metodini yozmasak `repr()` nima qaytaradi?
A) Error  
B) Default representation  
C) None  
D) Class nomi

**21.** Quyidagi kod natijasi nima?
```python
class X:
    value = 5

class Y:
    value = 10

class Z(Y, X):
    pass

z = Z()
print(z.value)
```
A) 5  
B) 10  
C) 15  
D) Error

**22.** MRO (Method Resolution Order) qanday aniqlanadi?
A) C3 linearization algoritmi  
B) Random  
C) Alfabetik tartib  
D) Yaratilish tartibi

**23.** Quyidagi kod natijasi nima?
```python
class Time:
    def __init__(self, hours, minutes):
        self.hours = hours
        self.minutes = minutes
    
    def __add__(self, other):
        total_minutes = (self.hours * 60 + self.minutes) + (other.hours * 60 + other.minutes)
        return Time(total_minutes // 60, total_minutes % 60)

t1 = Time(1, 30)
t2 = Time(2, 45)
t3 = t1 + t2
print(t3.hours, t3.minutes)
```
A) 3 75  
B) 4 15  
C) 4 75  
D) Error

**24.** `__sub__`, `__mul__`, `__truediv__` metodlari qaysi operatorlar uchun?
A) +, -, *  
B) -, *, /  
C) +, *, /  
D) -, /, *

**25.** Quyidagi kod natijasi nima?
```python
class Fraction:
    def __init__(self, numerator, denominator):
        self.num = numerator
        self.den = denominator
    
    def __eq__(self, other):
        return self.num * other.den == self.den * other.num

f1 = Fraction(1, 2)
f2 = Fraction(2, 4)
print(f1 == f2)
```
A) True  
B) False  
C) Error  
D) None

**26.** `__ne__`, `__gt__`, `__ge__` metodlari nima uchun?
A) !=, >, >=  
B) ==, <, <=  
C) +, -, *  
D) and, or, not

**27.** Quyidagi kod natijasi nima?
```python
class Address:
    def __init__(self, city, street):
        self.city = city
        self.street = street

class Person:
    def __init__(self, name, city, street):
        self.name = name
        self.address = Address(city, street)

p = Person("Ali", "Tashkent", "Amir Temur")
print(p.address.city)
```
A) Ali  
B) Tashkent  
C) Amir Temur  
D) Error

**28.** Composition qachon inheritance dan yaxshiroq?
A) "has-a" munosabatda  
B) "is-a" munosabatda  
C) Har doim  
D) Hech qachon

**29.** Quyidagi kod natijasi nima?
```python
class Shape:
    pass

class Rectangle(Shape):
    pass

r = Rectangle()
print(isinstance(r, Rectangle) and isinstance(r, Shape))
```
A) True  
B) False  
C) Error  
D) None

**30.** Quyidagi kod natijasi nima?
```python
class Animal:
    pass

class Dog(Animal):
    pass

print(issubclass(Dog, Animal))
```
A) True  
B) False  
C) Error  
D) None

**31.** Quyidagi kod natijasi nima?
```python
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

c = Car("Toyota", "Camry")
print(hasattr(c, "brand") and hasattr(c, "model") and hasattr(c, "year"))
```
A) True  
B) False  
C) Error  
D) None

**32.** `getattr()` funksiyasiga default qiymat bersa bo'ladimi?
A) Yo'q  
B) Ha, uchinchi parametr sifatida  
C) Faqat None  
D) Faqat string

**33.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.name = name

p = Person("Ali")
print(getattr(p, "age", 25))
```
A) Ali  
B) 25  
C) Error  
D) None

**34.** `__getitem__` va `__setitem__` metodlari qaysi operatorlar uchun?
A) `[]` operatori  
B) `.` operatori  
C) `()` operatori  
D) `{}` operatori

**35.** Quyidagi kod natijasi nima?
```python
class Matrix:
    def __init__(self):
        self.data = [[1, 2], [3, 4]]
    
    def __getitem__(self, index):
        return self.data[index]

m = Matrix()
print(m[1][0])
```
A) 1  
B) 2  
C) 3  
D) 4

**36.** Quyidagi kod natijasi nima?
```python
class Bag:
    def __init__(self):
        self.items = ["apple", "banana", "cherry"]
    
    def __contains__(self, item):
        return item in self.items

b = Bag()
print("banana" in b)
```
A) True  
B) False  
C) Error  
D) None

**37.** Iterator protocol nimadan iborat?
A) `__iter__` va `__next__`  
B) `__start__` va `__stop__`  
C) `__begin__` va `__end__`  
D) `__first__` va `__last__`

**38.** Quyidagi kod natijasi nima?
```python
class Countdown:
    def __init__(self, start):
        self.current = start
    
    def __iter__(self):
        return self
    
    def __next__(self):
        if self.current <= 0:
            raise StopIteration
        self.current -= 1
        return self.current + 1

c = Countdown(3)
print(list(c))
```
A) [3, 2, 1]  
B) [3, 2, 1, 0]  
C) [2, 1, 0]  
D) Error

**39.** Generator va Iterator farqi nima?
A) Generator - `yield` ishlatadi, Iterator - class  
B) Farqi yo'q  
C) Generator - class, Iterator - function  
D) Ikkalasi ham bir xil

**40.** Abstract Base Class qanday yaratiladi?
A) `from abc import ABC`  
B) Oddiy class  
C) Static class  
D) `from abstract import Base`

**41.** Quyidagi kod xato beradimi?
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

s = Shape()
```
A) Yo'q  
B) Ha, abstract classdan instance yaratib bo'lmaydi  
C) Faqat Python 2 da  
D) Faqat method bo'lmasa

**42.** Abstract method child classda implement qilinmasa nima bo'ladi?
A) Hech narsa  
B) Xato beradi  
C) Ishlaydi  
D) Warning beradi

**43.** Quyidagi kod natijasi nima?
```python
class Person:
    count = 0
    
    def __init__(self, name):
        self.name = name
        Person.count += 1
    
    def __del__(self):
        Person.count -= 1

p1 = Person("Ali")
p2 = Person("Vali")
del p1
print(Person.count)
```
A) 0  
B) 1  
C) 2  
D) Error

**44.** Garbage collection qachon `__del__` ni chaqiradi?
A) Darhol  
B) Ob'yektga hech qanday havola qolmaganda  
C) Dastur tugaganda  
D) Hech qachon

**45.** Metaclass nima?
A) Klasslarni yaratuvchi class  
B) Oddiy class  
C) Abstract class  
D) Static class

**46.** `__new__` va `__init__` farqi nima?
A) `__new__` - ob'yekt yaratadi, `__init__` - initsializatsiya qiladi  
B) Farqi yo'q  
C) `__init__` - ob'yekt yaratadi, `__new__` - initsializatsiya qiladi  
D) Ikkalasi ham bir xil

**47.** Quyidagi kod natijasi nima?
```python
class Singleton:
    _instance = None
    
    def __new__(cls):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
        return cls._instance

s1 = Singleton()
s2 = Singleton()
print(s1 is s2)
```
A) True  
B) False  
C) Error  
D) None

**48.** `is` va `==` operatorlari farqi nima?
A) `is` - xotira manzili, `==` - qiymat  
B) Farqi yo'q  
C) `==` - xotira manzili, `is` - qiymat  
D) Ikkalasi ham bir xil

**49.** Quyidagi kod natijasi nima?
```python
class Adder:
    def __init__(self, n):
        self.n = n
    
    def __call__(self, x):
        return self.n + x

add5 = Adder(5)
print(add5(10))
```
A) 5  
B) 10  
C) 15  
D) Error

**50.** Callable ob'yekt nima?
A) Funksiya kabi chaqirilishi mumkin bo'lgan ob'yekt  
B) Oddiy ob'yekt  
C) Class  
D) Metod

---

## 5-VARIANT

**1.** Quyidagi kod natijasi nima?
```python
class Smartphone:
    def __init__(self, brand, model, price):
        self.brand = brand
        self.model = model
        self.price = price

phone = Smartphone("Apple", "iPhone 13", 999)
print(phone.brand)
```
A) Smartphone  
B) Apple  
C) iPhone 13  
D) 999

**2.** Instance variable qachon yaratiladi?
A) Class yaratilganda  
B) `__init__` metodida  
C) Metod chaqirilganda  
D) Import qilinganda

**3.** Quyidagi kod natijasi nima?
```python
class Logger:
    log_count = 0
    
    @classmethod
    def log(cls, message):
        cls.log_count += 1
        return f"Log #{cls.log_count}: {message}"

print(Logger.log("Error"))
print(Logger.log("Warning"))
print(Logger.log_count)
```
A) 1  
B) 2  
C) 3  
D) Error

**4.** Quyidagi kod natijasi nima?
```python
class Appliance:
    def operate(self):
        return "Operating"

class WashingMachine(Appliance):
    def operate(self):
        return "Washing"

wm = WashingMachine()
print(wm.operate())
```
A) Operating  
B) Washing  
C) Error  
D) None

**5.** Inheritance ning asosiy maqsadi nima?
A) Kodni qayta ishlatish  
B) Ob'yektlarni o'chirish  
C) Metodlarni yashirish  
D) Klasslarni birlashtirish

**6.** Quyidagi kod natijasi nima?
```python
class Vehicle:
    def __init__(self, brand):
        self.brand = brand

class Car(Vehicle):
    def __init__(self, brand, model):
        super().__init__(brand)
        self.model = model

c = Car("Toyota", "Corolla")
print(c.brand + " " + c.model)
```
A) Toyota  
B) Corolla  
C) Toyota Corolla  
D) Error

**7.** `super().__init__()` chaqirilmasa nima bo'ladi?
A) Parent class `__init__` ishlamaydi  
B) Xato beradi  
C) Hech narsa  
D) Child class ishlamaydi

**8.** Quyidagi kod natijasi nima?
```python
class Converter:
    @staticmethod
    def celsius_to_fahrenheit(c):
        return (c * 9/5) + 32

print(Converter.celsius_to_fahrenheit(100))
```
A) 100  
B) 212  
C) 212.0  
D) Error

**9.** Static method `self` parametriga ega bo'ladimi?
A) Ha  
B) Yo'q  
C) Ba'zida  
D) Faqat Python 3 da

**10.** Quyidagi kod natijasi nima?
```python
class Database:
    connection_string = "localhost:5432"
    
    @classmethod
    def connect(cls):
        return f"Connecting to {cls.connection_string}"

print(Database.connect())
```
A) Database  
B) Connecting to localhost:5432  
C) localhost:5432  
D) Error

**11.** `@classmethod` va `@staticmethod` farqi nima?
A) `@classmethod` - `cls` oladi, `@staticmethod` - hech narsa olmaydi  
B) Farqi yo'q  
C) `@staticmethod` - `cls` oladi  
D) Ikkalasi ham bir xil

**12.** Quyidagi kod natijasi nima?
```python
class Cylinder:
    def __init__(self, radius, height):
        self.radius = radius
        self.height = height
    
    @property
    def volume(self):
        return 3.14 * self.radius ** 2 * self.height

cyl = Cylinder(5, 10)
print(int(cyl.volume))
```
A) 15  
B) 50  
C) 785  
D) Error

**13.** Property ga qiymat o'rnatish uchun nima kerak?
A) `@property` yetadi  
B) `@property.setter` decorator  
C) `@setter` decorator  
D) O'rnatib bo'lmaydi

**14.** Quyidagi kod natijasi nima?
```python
class Temperature:
    def __init__(self):
        self._celsius = 0
    
    @property
    def celsius(self):
        return self._celsius
    
    @celsius.setter
    def celsius(self, value):
        if value >= -273:
            self._celsius = value

t = Temperature()
t.celsius = -300
print(t.celsius)
```
A) -300  
B) 0  
C) Error  
D) -273

**15.** Quyidagi kod natijasi nima?
```python
class ShoppingCart:
    def __init__(self):
        self.items = []
    
    def add_item(self, item):
        self.items.append(item)
    
    def total_items(self):
        return len(self.items)

cart = ShoppingCart()
cart.add_item("Book")
cart.add_item("Pen")
cart.add_item("Notebook")
print(cart.total_items())
```
A) 1  
B) 2  
C) 3  
D) Error

**16.** Polymorphism ning qaysi turi mavjud?
A) Compile-time polymorphism  
B) Runtime polymorphism  
C) Ad-hoc polymorphism  
D) Barchasi

**17.** Quyidagi kod natijasi nima?
```python
class Shape:
    def perimeter(self):
        pass

class Square(Shape):
    def __init__(self, side):
        self.side = side
    
    def perimeter(self):
        return 4 * self.side

class Triangle(Shape):
    def __init__(self, a, b, c):
        self.a, self.b, self.c = a, b, c
    
    def perimeter(self):
        return self.a + self.b + self.c

shapes = [Square(5), Triangle(3, 4, 5)]
total = sum([s.perimeter() for s in shapes])
print(total)
```
A) 20  
B) 12  
C) 32  
D) Error

**18.** `__str__` metodi qanday string qaytarishi kerak?
A) Foydalanuvchi uchun tushunarli  
B) Debugging uchun  
C) Xotira manzili  
D) Class nomi

**19.** Quyidagi kod natijasi nima?
```python
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary
    
    def __str__(self):
        return f"{self.name}: ${self.salary}"
    
    def __repr__(self):
        return f"Employee('{self.name}', {self.salary})"

e = Employee("John", 5000)
print(repr(e))
```
A) John: $5000  
B) Employee('John', 5000)  
C) Employee  
D) Error

**20.** `print()` avval qaysi metodga murojaat qiladi?
A) `__repr__`  
B) `__str__`  
C) `__init__`  
D) `__call__`

**21.** Quyidagi kod natijasi nima?
```python
class A:
    def method(self):
        return "A"

class B(A):
    def method(self):
        return "B"

class C(A):
    def method(self):
        return "C"

class D(B, C):
    pass

d = D()
print(d.method())
```
A) A  
B) B  
C) C  
D) Error

**22.** Diamond problem nima?
A) Multiple inheritance da nom to'qnashuvi  
B) Oddiy muammo  
C) Inheritance yo'q  
D) Class yaratish muammosi

**23.** Quyidagi kod natijasi nima?
```python
class Money:
    def __init__(self, amount):
        self.amount = amount
    
    def __add__(self, other):
        return Money(self.amount + other.amount)
    
    def __str__(self):
        return f"${self.amount}"

m1 = Money(100)
m2 = Money(50)
m3 = m1 + m2
print(m3)
```
A) 150  
B) $150  
C) Money  
D) Error

**24.** Qaysi metodlar operator overloading uchun ishlatiladi?
A) `__add__`, `__sub__`, `__mul__`, `__truediv__`  
B) `add()`, `sub()`, `mul()`, `div()`  
C) `+`, `-`, `*`, `/`  
D) Hech biri

**25.** Quyidagi kod natijasi nima?
```python
class List:
    def __init__(self, items):
        self.items = items
    
    def __eq__(self, other):
        return self.items == other.items
    
    def __len__(self):
        return len(self.items)

l1 = List([1, 2, 3])
l2 = List([1, 2, 3])
print(l1 == l2 and len(l1) == 3)
```
A) True  
B) False  
C) Error  
D) None

**26.** `__hash__` metodi nima uchun ishlatiladi?
A) Ob'yektni dictionary key sifatida ishlatish  
B) Ob'yektni yaratish  
C) Ob'yektni o'chirish  
D) Ob'yektni print qilish

**27.** Quyidagi kod natijasi nima?
```python
class Wheel:
    def __init__(self, size):
        self.size = size

class Engine:
    def __init__(self, power):
        self.power = power

class Car:
    def __init__(self, wheel_size, engine_power):
        self.wheels = [Wheel(wheel_size) for _ in range(4)]
        self.engine = Engine(engine_power)

car = Car(18, 200)
print(len(car.wheels))
```
A) 1  
B) 2  
C) 4  
D) Error

**28.** Aggregation va Composition farqi nima?
A) Aggregation - "weak has-a", Composition - "strong has-a"  
B) Farqi yo'q  
C) Aggregation kuchliroq  
D) Ikkalasi ham bir xil

**29.** Quyidagi kod natijasi nima?
```python
class Base:
    pass

class Derived(Base):
    pass

d = Derived()
print(type(d) == Derived)
```
A) True  
B) False  
C) Error  
D) None

**30.** `type(obj)` va `isinstance(obj, Class)` farqi nima?
A) `type()` - aniq class, `isinstance()` - class hierarchy  
B) Farqi yo'q  
C) `isinstance()` tezroq  
D) Ikkalasi ham bir xil

**31.** Quyidagi kod natijasi nima?
```python
class Book:
    def __init__(self, title, author, pages):
        self.title = title
        self.author = author
        self.pages = pages

b = Book("Python", "Guido", 300)
attrs = ["title", "author", "pages", "price"]
count = sum([hasattr(b, attr) for attr in attrs])
print(count)
```
A) 1  
B) 2  
C) 3  
D) 4

**32.** `setattr()` orqali yangi attribut qo'shsa bo'ladimi?
A) Yo'q  
B) Ha  
C) Faqat `__init__` da  
D) Faqat property orqali

**33.** Quyidagi kod natijasi nima?
```python
class Config:
    def __init__(self):
        self.settings = {}
    
    def __setitem__(self, key, value):
        self.settings[key] = value
    
    def __getitem__(self, key):
        return self.settings.get(key, "Not found")

config = Config()
config["debug"] = True
config["port"] = 8080
print(config["debug"], config["port"])
```
A) True 8080  
B) Not found Not found  
C) Error  
D) None

**34.** `__delitem__` metodi nima qiladi?
A) `del obj[key]` operatori uchun  
B) Ob'yektni o'chiradi  
C) Metodlarni o'chiradi  
D) Klassni o'chiradi

**35.** Quyidagi kod natijasi nima?
```python
class Range:
    def __init__(self, start, end):
        self.start = start
        self.end = end
    
    def __contains__(self, value):
        return self.start <= value <= self.end

r = Range(10, 20)
print(15 in r and 25 not in r)
```
A) True  
B) False  
C) Error  
D) None

**36.** `in` operatori qaysi metodni chaqiradi?
A) `__in__`  
B) `__contains__`  
C) `__has__`  
D) `__check__`

**37.** Quyidagi kod natijasi nima?
```python
class Fibonacci:
    def __init__(self, n):
        self.n = n
        self.a, self.b = 0, 1
        self.count = 0
    
    def __iter__(self):
        return self
    
    def __next__(self):
        if self.count >= self.n:
            raise StopIteration
        self.count += 1
        self.a, self.b = self.b, self.a + self.b
        return self.a

fib = Fibonacci(5)
print(list(fib))
```
A) [0, 1, 1, 2, 3]  
B) [1, 1, 2, 3, 5]  
C) [1, 2, 3, 5, 8]  
D) Error

**38.** Generator expression va generator function farqi nima?
A) Expression - `()` ichida, Function - `yield` bilan  
B) Farqi yo'q  
C) Expression tezroq  
D) Function yaxshiroq

**39.** Quyidagi kod to'g'rimi?
```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self):
        pass

class Dog(Animal):
    def sound(self):
        return "Bark"

d = Dog()
```
A) Yo'q, xato  
B) Ha, to'g'ri  
C) Faqat Python 2 da  
D) Faqat method bo'lmasa

**40.** Abstract method da implementation bo'lsa bo'ladimi?
A) Yo'q  
B) Ha, lekin child classda qayta yozilishi kerak  
C) Faqat Python 3 da  
D) Hech qachon

**41.** Quyidagi kod natijasi nima?
```python
class Person:
    def __init__(self, name):
        self.name = name
    
    def __del__(self):
        print(f"Deleting {self.name}")

p1 = Person("Ali")
p2 = p1
del p1
print("After del p1")
```
A) Deleting Ali, After del p1  
B) After del p1, Deleting Ali  
C) After del p1  
D) Error

**45.** Circular reference muammosi nima?
A) Ikki ob'yekt bir-biriga havola qilganda  
B) Oddiy muammo  
C) Klasslar orasidagi muammo  
D) Metodlar orasidagi muammo

**43.** Dataclass nima?
A) `@dataclass` decorator bilan soddalashtirilgan class  
B) Oddiy class  
C) Abstract class  
D) Static class

**44.** Quyidagi kod natijasi nima?
```python
from dataclasses import dataclass

@dataclass
class Point:
    x: int
    y: int

p1 = Point(3, 4)
p2 = Point(3, 4)
print(p1 == p2)
```
A) True  
B) False  
C) Error  
D) None

**45.** Named tuple va dataclass farqi nima?
A) Dataclass mutable, Named tuple immutable  
B) Farqi yo'q  
C) Named tuple tezroq  
D) Ikkalasi ham bir xil

**46.** Quyidagi kod natijasi nima?
```python
class Singleton:
    _instance = None
    _initialized = False
    
    def __new__(cls):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
        return cls._instance
    
    def __init__(self):
        if not Singleton._initialized:
            self.value = 0
            Singleton._initialized = True

s1 = Singleton()
s1.value = 10
s2 = Singleton()
print(s2.value)
```
A) 0  
B) 10  
C) Error  
D) None

**47.** Factory pattern nima?
A) Ob'yekt yaratish uchun interfeys  
B) Oddiy pattern  
C) Singleton pattern  
D) Iterator pattern

**48.** Quyidagi kod natijasi nima?
```python
class Operation:
    def execute(self):
        pass

class Addition(Operation):
    def __init__(self, a, b):
        self.a, self.b = a, b
    
    def execute(self):
        return self.a + self.b

class Multiplication(Operation):
    def __init__(self, a, b):
        self.a, self.b = a, b
    
    def execute(self):
        return self.a * self.b

ops = [Addition(5, 3), Multiplication(4, 2)]
result = sum([op.execute() for op in ops])
print(result)
```
A) 8  
B) 16  
C) 24  
D) Error

**49.** Quyidagi kod natijasi nima?
```python
class Doubler:
    def __call__(self, x):
        return x * 2

double = Doubler()
result = double(5) + double(10)
print(result)
```
A) 15  
B) 20  
C) 30  
D) Error

**50.** Decorator pattern OOP da qanday amalga oshiriladi?
A) Wrapper class orqali  
B) Oddiy class orqali  
C) Static class orqali  
D) Abstract class orqali

---

# JAVOBLAR KALITI

## 1-VARIANT
1. C  2. B  3. B  4. B  5. C  6. B  7. B  8. B  9. C  10. B
11. A  12. B  13. B  14. C  15. B  16. B  17. B  18. C  19. A  20. C
21. B  22. B  23. A  24. C  25. A  26. B  27. B  28. C  29. B  30. C
31. A  32. B  33. B  34. A  35. B  36. B  37. B  38. A  39. B  40. B
41. B  42. C  43. B  44. A  45. B  46. C  47. B  48. A  49. B  50. C

## 2-VARIANT
1. B  2. B  3. D  4. B  5. B  6. B  7. B  8. B  9. B  10. B
11. B  12. C  13. C  14. B  15. A  16. A  17. B  18. C  19. D  20. A
21. B  22. B  23. B  24. A  25. C  26. C  27. A  28. B  29. A  30. C
31. B  32. A  33. B  34. C  35. B  36. A  37. B  38. A  39. B  40. B
41. B  42. B  43. B  44. C  45. B  46. B  47. B  48. C  49. A  50. C

## 3-VARIANT
1. B  2. C  3. A  4. B  5. C  6. A  7. C  8. A  9. B  10. B
11. B  12. A  13. B  14. A  15. C  16. B  17. B  18. C  19. B  20. B
21. A  22. A  23. C  24. C  25. A  26. B  27. B  28. B  29. A  30. B
31. A  32. B  33. A  34. C  35. A  36. B  37. A  38. A  39. A  40. A
41. B  42. B  43. A  44. B  45. A  46. B  47. B  48. B  49. A  50. C

## 4-VARIANT
1. B  2. A  3. C  4. B  5. B  6. C  7. B  8. C  9. B  10. B
11. B  12. B  13. A  14. B  15. C  16. D  17. C  18. B  19. B  20. B
21. B  22. A  23. B  24. B  25. A  26. A  27. B  28. A  29. A  30. A
31. B  32. B  33. B  34. A  35. C  36. A  37. A  38. A  39. A  40. A
41. B  42. B  43. B  44. B  45. A  46. A  47. A  48. A  49. A  50. A

## 5-VARIANT
1. B  2. B  3. C  4. B  5. A  6. C  7. A  8. C  9. B  10. B
11. A  12. C  13. B  14. B  15. C  16. D  17. C  18. A  19. B  20. B
21. B  22. A  23. B  24. A  25. A  26. A  27. C  28. A  29. A  30. A
31. C  32. B  33. A  34. A  35. A  36. B  37. B  38. A  39. B  
