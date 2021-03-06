Java 访问修饰符
===============

访问修饰符用来控制对类、变量、方法和构造方法的访问。Java 有4种访问控制符。

default
--------------

什么也不写的情况，在同一包内可见。使用对象：类、接口、变量、方法。使用默认访问修饰符声明的变量和方法，对同一个包内的类是可见的。
例外的是，接口里的变量默认声明为public static final,接口里的方法默认访问修饰符为public。

private
--------------

被声明为private的方法、变量和构造方法只能被所属类访问，并且类和接口不能声明为private。
声明为私有访问类型的变量只能通过类当中公共的getter方法被外部类访问。
private访问修饰符的使用主要用来隐藏类的实现细节和保护类的数据。

public
--------------

被声明为public的类、方法、构造方法和接口能够被任何其他类访问。
如果几个相互访问的public 类分布在不同的包中，则需要导入相应 public类所在的包。
由于类的继承性类所有的公有方法和变量都能被其子类继承。

protected
---------------

分两种情况，子类与基类在同一包中：被声明为 protected的变量、方法和构造器能被同一个包中的任何其他类访问；子类与基类不在同一包中：那么在子类中，子类实例可以访问其从基类继承而来的protected 方法，而不能访问基类实例的protected方法。protected可以修饰数据成员，构造方法，方法成员，不能修饰类（内部类除外）。并且接口及接口的成员变量和成员方法不能声明为protected。
