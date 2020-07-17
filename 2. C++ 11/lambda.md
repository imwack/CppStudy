lambda表达式，可以方便的定义匿名函数
形式如下

    [capture list] (params list) mutable exception-> return type { function body }

capture list: 可以是=或&，表示{}中用到的、定义在{}外面的变量在{}中是否允许被改变。=表示不允许，&表示允许

例如

    vector<int> v{ 1,3,2,5,6 };
    //用lambda定义个cmp函数
    sort(v.begin(), v.end(), [=](int x, int y) -> bool {return x < y; });
    //用lambda定义个输出函数
    for_each(v.begin(), v.end(), [=](int i)->void {cout << i << endl; });

