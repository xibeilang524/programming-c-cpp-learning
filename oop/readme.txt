类定义
========
类是C++和核心特性，通常被称为用户定义的类型。类用于指定对象的形式，包含了数据表示法和用于处理数据的方法。类中的数据和方法称为类的成员。函数在类中称为类的成员。
定义类，本质上是定义一个数据类型的蓝图。实际上并并没有定义任何数据，但它定义了类的名称意味着什么，也就是说，她定义了对象包括什么，以及可以在这个对象上执行哪些操作。
类定义是以关键字class开头，后跟类的名称。类的主体包含在一对花括号中。
类定义后必须跟着一个分号或一个声明列表。

class Box
{
	public:
	    double length;  // length of a box
	    double breadth; // Breadth of a box
	    double height;  // Height of a box
};


多态
=========
子类对父类的方法进行独立实现，就是所谓多态。多态分为两种：
* 静态多态，或者静态链接，编译时已经绑定，所谓早绑定
* 采用关键字virtual修饰的函数称为虚函数，目的是告诉编译器该函数属于
动态链接，依据调用函数的实例对象而定，所谓的后期绑定。

纯虚函数：让函数 =0 告诉编译器函数没有实现主体，为纯虚函数。

数据抽象
==========
接口与实现分离的设计模式。

抽象函数
==========
接口设计模式的策略。
抽象函数不能实例化，除非是对其虚函数进行实现的子类。
