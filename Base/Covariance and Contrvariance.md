
2023-04-21 14:11 Tags: #source Medium #quest #lesson #summary

## Записи з урока:

- Java стандартно використовую invariance, тобто ми не можемо 
  `List<Object> obj = new ArrayList...;
  `obj.add(new String()); - отримаємо помилку компілятора`
- Для covariance треба використати `List<? extends Object>` - тоді можна буде додати об'ект строки, або будь що що розширює клас Object
- Ми говоримо що параметричний тип `T` являється covariant в generic type `M<T>`, якщо ці твердження істинні:
		                              - Клас `A` підтип класу `B`(тобто `List<B>` зможе приймати в себе об'екти `A`)
		                              -  `M<A>` підтип `M<B>`.
- Contrvariance - протилежно covariance, тобто нам треба запихнути в List класи від які розширює generic type. `List<? super Number>` - як приклад
---

### Zero-Links:

- [[00 Java]]
---

### Links:

- https://medium.com/@yuhuan/covariance-and-contravariance-in-java-6d9bfb7f6b8e
---

### Література:

- 
---

### Додаткові матеріали:

- 