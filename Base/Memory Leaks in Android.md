
2023-03-29 09:33 Tags: #source Udemy #quest #lesson #summary

## Записи з урока:

- Memory leak - коли об'ект, який більше не використовує і не буде використовувати додаток, не видаляеться GC[[Garbage collector in android]]. Таке стаеться через те що якийсь "живий" компонент досі тримає лінк на цей об'ект, тому GC не може його видалити
- Roots - об'етки які завжди досяжні для GC і ніколи не знищюються. Тобто це об'екти які тримають інші об'екти в пам'яті
<p align="center">
  <img src="C:\Users\oleksandr.honcharuk\Documents\hard_skills\Files\GC roots.jpg" />
</p> 
- Головні Roots в Андроід додатку:
                       - Об'екти посилання на які зберігається в статичних полях
                       - Інстанси Application класу
                       - Live thrads(Active Threads) - стан потоку від виклику метода start() до закінчення методу run()
* Threads lifecycle:
  <p align="center">
  <img src="C:\Users\oleksandr.honcharuk\Documents\hard_skills\Files\Thread-Life-Cycle-in-Java.jpg" />
</p>
- ***Anonymous та Inner класи мають неявне посилання на об'екти зовнішнього класа***
- Наприклад анонімний клас Thread в середині Актівіті буду тримати посилання на обект Актівіті, тому Актівіті не може бути знищена GC поки тред знаходиться в стані Active. Те саме і для внутрішнього класу Thread
- Усі Threads мають бути своечасно завершені щоб уникнути меморі лік
---

### Zero-Links:

- [[00 Android]] [[00 Multithreading]]
---

### Links:

- https://globallogic.udemy.com/course/android-multithreading/learn/lecture/15964520#announcements
---

### Література:

- 
---

### Додаткові матеріали:

- 