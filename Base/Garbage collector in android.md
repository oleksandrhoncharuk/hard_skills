
2023-03-24 11:35 Tags: #source Udemy #quest #lesson #summary

## Основные идеи из урока и ответы на вопросы:

- Коли ми створюємо об'єкт за допомогою new - під цей об'ект виділяеться пам'ять і він її займає.
- OutOfMemoryException - виникає коли оперативна пам'ять заповнена об'ектами які не видаляються
- Garbage Collector(GC) - системний процес який відновлює пам'ять видаляючи з неї об'екти які не використовуються. Об'ект який не використовується, у цьому випадку, - це той на якого не має активних ссилок
- Доступність об'екта:
  <p align="center">
  <img src="C:\Users\oleksandr.honcharuk\Documents\hard_skills\Files\GC.png" width="500" height="100"/>
  </p>
- Circular references - у цьому випадку об'ект 1 ссилаеться на об'ект 2, а об'ект 2 на 1. Якщо на ці об'екти більше ніхто не ссилаеться тоді GC помітить їх обох як unreachable і видалить: 
  <p align="center">
  <img src="C:\Users\oleksandr.honcharuk\Documents\hard_skills\Files\circular references.jpg" width="300" height="50"/>
  </p>

---

### Zero-Links
[[00 Multithreading]] [[00 Android]] 

---

### Links
https://globallogic.udemy.com/course/android-multithreading/learn/lecture/15858162#announcements

---

### Основная литература к уроку

- 

---

### Дополнительные материалы

- 