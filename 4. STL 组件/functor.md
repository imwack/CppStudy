STL内建了一些函数对象。#include<functional>
分为:算数类函数对象,关系运算类函数对象，逻辑运算类仿函数
function是容器和算法之间的桥梁

算数类

    template<class T> T plus<T>//加法仿函数
    template<class T> T minus<T>//减法仿函数
    template<class T> T multiplies<T>//乘法仿函数
    template<class T> T divides<T>//除法仿函数
    template<class T> T modulus<T>//取模仿函数
    template<class T> T negate<T>//取反仿函数 

运算类

    template<class T> bool equal_to<T>//等于
    template<class T> bool not_equal_to<T>//不等于
    template<class T> bool greater<T>//大于
    template<class T> bool greater_equal<T>//大于等于
    template<class T> bool less<T>//小于
    template<class T> bool less_equal<T>//小于等于

逻辑类

    template<class T> bool logical_and<T>//逻辑与
    template<class T> bool logical_or<T>//逻辑或
    template<class T> bool logical_not<T>//逻辑非