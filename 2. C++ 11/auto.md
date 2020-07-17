1. 类型说明符auto,类型自动推断

        array<int, 10> arr;
        auto it = arr.begin();

2. decltype取变量类型

        array<int, 10> arr;
        decltype(arr) a;