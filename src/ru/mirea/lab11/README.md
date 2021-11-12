# Практическая работа №11
## Примеры реализации synchronized
```java
public class SynchExample {
    private Object obj = new Object();
    // Способ №1
    public synchronized void doSomething(){
        // логика метода, доступная для всех потоков
        synchronized (obj){
            // логика одновременно доступная только для одного потока
        }
    }
    // Способ №2
    public void swap(){
        synchronized (this){
            // логика метода
        }
    }
}

```

## Задание
Реализовать программу "конных скачек": `n` количество лошадей стартует.
Отмечается кто за кем (какой по счету) финишировал.