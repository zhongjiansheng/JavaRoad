[TOC]

## 一、流

流是一种数据格式，基于流可以实现免费的并行处理，并且可以做到代码的简单和易理解。

行为参数化：方法中的具体方法取决于传递的参数，从而实现方法的多样性，减少代码的重复率。

通过使用 **Lambda** 来进行参数化模式：

```java
List<Apple> result = filterApples(inventory, (Apple apple) -> "red".equals(apple.getColors()));
```

