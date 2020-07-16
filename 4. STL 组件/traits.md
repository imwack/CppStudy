traits技术
STL中的迭代器将容器和算法进行联系。
迭代器是一种指针，如何获取指针的类型来适应不同的容器，使用的方法就是利用function template的参数推导机制。

迭代器所指的对象类型，称为迭代器的value type

    template<clss T>
    struct MyIter
    {
        typedef T value_type;
        T* ptr;
        MyIter(T* p=0):ptr(p)
        {

        }

        T& operator*() const {return *ptr;}
    }

    template<clss I>
    typename I::value_type //func的返回类型
    fun(I ite)
    {
        return *ite;
    }

    MyIter<int> ite(new int(8));
    count<<func(ite);

Typename
对于用于模板定义的依赖于模板参数的名称，只有在实例化的参数中存在这个类型名，或者这个名称前使用了typename关键字来修饰，编译器才会将该名称当成是类型。除了以上这两种情况，绝不会被当成是类型。

因此，如果你想直接告诉编译器T::iterator是类型而不是变量，只需用typename修饰：

几种迭代器类型
Input
Output
Forward
Bidirectional
Random Access