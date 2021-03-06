Java 数据类型
=============

基本数据类型
-------------

两大数据类型
  内置数据类型
  引用数据类型

八种基本类型。六种数字类型（四个整数型，两个浮点型），一种字符类型，还有一种布尔型。

#. byte数据类型是8位、有符号的，以二进制补码表示的整数；最小值是
   -128（-2^7）；最大值是 127（2^7-1）；默认值是 0；byte
   类型用在大型数组中节约空间，主要代替整数，因为 byte
   变量占用的空间只有 int 类型的四分之一；

#. short数据类型是 16 位、有符号的以二进制补码表示的整数,最小值是
   -32768（-2^15）；最大值是 32767（2^15 - 1）；Short 数据类型也可以像
   byte
   那样节省空间。一个short变量是int型变量所占空间的二分之一；默认值是
   0；

#. int数据类型是32位、有符号的以二进制补码表示的整数；最小值是
   -2,147,483,648（-2^31）；最大值是 2,147,483,647（2^31 -
   1）；一般地整型变量默认为 int 类型；默认值是 0 ；

#. long数据类型是 64 位、有符号的以二进制补码表示的整数；最小值是
   -9,223,372,036,854,775,808（-2^63）；最大值是
   9,223,372,036,854,775,807（2^63
   -1）；这种类型主要使用在需要比较大整数的系统上；默认值是 0L；

#. float数据类型是单精度、32位、符合IEEE 754标准的浮点数；float
   在储存大型浮点数组的时候可节省内存空间；默认值是
   0.0f；浮点数不能用来表示精确的值，如货币；

#. double数据类型是双精度、64 位、符合 IEEE 754 标准的浮点数；
   浮点数的默认类型为 double 类型；
   double类型同样不能表示精确的值，如货币； 默认值是 0.0d；

#. boolean数据类型表示一位的信息；只有两个取值：true 和
   false；这种类型只作为一种标志来记录 true/false 情况；默认值是 false；

#. char类型是一个单一的 16 位 Unicode 字符；最小值是\u0000（十进制等效值为 0）；最大值是 \uffff（即为 65535）；char 数据类型可以储存任何字符；

引用类型
-------------

引用类型指向一个对象，指向对象的变量是引用变量。这些变量在声明时被指定为一个特定的类型，比如Employee、Puppy等。变量一旦声明后，类型就不能被改变了。对象、数组都是引用数据类型。所有引用类型的默认值都是null。一个引用变量可以用来引用任何与之兼容的类型。

数据类型转换
-------------

数据类型转换必须满足如下规则

#. 不能对boolean类型进行类型转换。
#. 不能把对象类型转换成不相关类的对象。
#. 在把容量大的类型转换为容量小的类型时必须使用强制类型转换。
#. 转换过程中可能导致溢出或损失精度。
#. 浮点数到整数的转换是通过舍弃小数得到，而不是四舍五入。

强制类型转换
-------------

#.  条件是转换的数据类型必须是兼容的。

#. 格式：(type)value type是要强制类型转换后的数据类型。

隐含强制类型转换
----------------

#. 整数的默认类型是 int。

#. 小数默认是 double 类型浮点型，在定义 float 类型时必须在数字后面跟上F或者f。
