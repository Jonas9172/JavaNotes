# JavaNotes

1. 类的内部封装了成员变量、构造方法和成员方法。
   
   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/5c1e4efe-aeba-454d-9883-320a2a64038f)
   
2. 实例化是指使用已经定义好的类，创建该类对象的过程。
   
   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/c9f3217a-2a5f-4dab-9c67-332c6296c176)

3. 抽象类不能被实例化，只能被继承。抽象类可以包含非抽象方法和属性，但至少要有一个抽象方法。抽象方法是一种没有实现的方法，只有定义，需要在子类中被实现。
   -抽象类的定义：

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/209785da-5daf-4f60-827b-4914282ba6ef)

   抽象类的实现（如果一个类继承了一个抽象类，那么它必须实现父类中的所有抽象方法）（在子类中实现抽象方法时需要使用@Override注解）：

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/f81f6325-e081-4733-9bd9-623cee45813e)


4. 接口的内部主要就是封装了方法，包含抽象方法（JDK 7及以前），默认方法和静态方法（JDK 8），私有方法（JDK 9）。
   
   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/da2f4252-1c5a-4767-844c-53662ed00a5b)

5. 非抽象子类在实现接口时：
     -必须重写接口中所有抽象方法（所以，接口的抽象方法不能是 private、protected 或者 final）.
     -继承了接口的默认方法，即可以直接调用，也可以重写。
   接口中静态方法与.class 文件相关，所以只能使用接口名调用，不可以通过实现类的类名或者实现类的对象调用

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/d963a4ef-2999-4db5-8fd2-c223c675f35c)


6. 由于有了默认方法和静态方法，所以当两个默认方法或者静态方法包含一段相同的代码实现时，为了避免重复写该段代码，可以将其抽出来作为接口的私有方法。
   此外，对象的某些方法或者称为函数只想在对象的内部被使用，但不想在外部被访问到这些方法或函数，在此时也可以使用私有方法。 
 
   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/6c730bbc-2cd6-4c56-ba0b-de29f7fbea04)

7. Java 原则上只支持单一继承，但通过接口可以实现多重继承的目的。

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/baadb86f-fbce-4eb1-8a71-8c4ff222960f)

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/2734f98a-be33-4871-bd10-5c100a92ff3d)

8. 多态是指两个子类继承同一个父类，并分别重写父类中的同一个方法。可以通过继承（extends）的关系实现，也可以通过接口的形式实现。

  ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/a5f1a298-1292-4c48-871c-d91780e6f6d7)

9. 工厂模式（有多个工厂类，一个产品抽象类，工厂模式利用多态创建不同的产品对象，并使对象创建过程延迟到子类进行，不展示具体实现过程）：
   
   <img width="485" alt="屏幕截图 2024-02-20 064519" src="https://github.com/Jonas9172/JavaNotes/assets/105164575/9d7dceb5-b767-4ac9-a463-37ad27416295">

10. 抽象工厂模式（多个工厂类，多个产品抽象类）：

   ![图片](https://github.com/Jonas9172/JavaNotes/assets/105164575/2a9dcd52-b520-4237-8a7a-cbaff4654d92)





