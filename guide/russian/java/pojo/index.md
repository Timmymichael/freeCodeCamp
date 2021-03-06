---
title: POJO
localeTitle: POJO
---
## POJO

POJO означает «Обычный объект Java Java». Это отличается от _обычных_ объектов _Javascript_ . Обычный простой Java-объект относится к парадигме объектно-ориентированного программирования (ООП), которая используется на языке программирования Java. Модель [ООП](https://en.wikipedia.org/wiki/Object-oriented_programming) рассматривает данные как «объекты». Каждый «объект» является экземпляром «класса», который представляет архетип или шаблон, из которого все объекты наследуют свои свойства и атрибуты.

Поэтому POJO просто является Java-объектом. Однако он также должен удовлетворять следующим дополнительным критериям:

1.  он не должен распространять предустановленные Java-классы;

```java
public class Foo extends javax.servlet.http.HttpServlet { 
 ...// body ... 
 } 
```

2.  он не должен реализовывать предустановленные интерфейсы;

```java
public class Bar implements javax.ejb.EntityBean { 
  ...  // body 
 } 
```

3.  он не должен содержать предустановленные аннотации.

```java
@javax.persistence.Entity public class Baz { 
  ... // body ... 
 } 
```

Поэтому объект Java квалифицируется как POJO только тогда, когда он свободен от указанных выше изменений. Отсюда следует, что POJO не «связан никакими ограничениями», кроме тех, которые предписаны официальной спецификацией языка Java.

#### Дополнительная информация:

[Википедия - POJO](https://en.wikipedia.org/wiki/Plain_old_Java_object)