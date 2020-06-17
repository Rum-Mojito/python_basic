# fit9136 review
## 概述
以下部分为个人的理解，因为9136为全新的课程，但是和之前的9133很相似，所以根据以往经验这次将复习的内容（知识点）整理为3个部分，每个部分有不同的级别要求（概念理解，可以看懂代码，能写代码），会在后面的知识点部分给大家说明

## 第一部分 ---- python 基础

-------------------------------------


### partA. 衡量自己是否合格的标准
最最最最最重要的就是能够自己写代码，组织逻辑写出代码！！！！！！
代码题不会很难

最低要求：总的来说能够达到写出assignment2的水平（不包含load_person和load_patient这两个函数，assignment1没有参考性，这里不讨论）

（D及D以上在课堂上会讨论，开始只讨论最起码能过的要求，后面会说到什么样的分数大概对应什么样的掌握程度）

=====================================
### partB. 知识总结

1. 抽象（要求：概念理解）

    抽象简单来说是指把现实的问题转换成代码思想，这里举个例子，比如我们在做模拟传染病的时候。我们会把病人抽象成一个类，每一天的模拟抽象为一个循环等等。这是一个非常high level的概念

2. 基础数据类型/数据结构（要求：能写代码）

    - 把数据结构的概念大概能用英语总结一下

    - 数据存储方式，变量，变量名

    - 非集合数据类型
        - int (example: 5)
        - float (example: 5.0)

    - 集合数据类型
        - string (example: '5' or "5" or '5555' or "5555")
            - 常用方法！str.split(); str.count();str.join(a_list)
        - list (example: [5] or [5555])
            - 创建：a_list = [] or a_list = list() or a_list = [1, ‘two’, 3.0, ‘4’] or a_list = [1] * 6
            - 添加：a_list.append(new_item) or a_list.insert(index,new_item)
            - 取值：直接用下标/索引：a_list[1]
            - 修改：a_list[1] = 5
            - 删除：a_list.pop(index), a_list.remove(item)
            - 排序：a_list.sort(), a_list.reverse(), sorted(a_list)
        - tuple (example: (5) or (5555))
            - 和list类似，但是区别是不可修改
            - 特殊用法：x, y = a_tuple
        - set (example: {5} or {5555})
            - 创建：a_set=set()，a_set = {“one”, 2}，a_set = set([1,2,2,3])这里属于类型转换
            - 添加：a_set.add('c')
            - 删除：a_set.remove(item), a_set.discard(item), a_set.pop(index), item.clear()
            - 特殊的操作：Union，Intersection，Difference，Symmetric difference (xor)
        - dictionary (example {'no1':5, 'no2':5555})
            - 创建：a_dict={}；a_dict = {“one”:1, “two”:2}；a_dict = dict([(‘a’,1),(‘b’,1)])
            - 添加： a_dict[new_key] = new_value
            - 删除： del a_dict[a_key]；del（a_dict[a_key]）
            - 常用方法：a_dict.keys(), a_dict.items()
        - 索引，切片，range()，in，+，

    - 可变数据类型（mutable） -- list, set, dictionary 

    - 不可变数据类型 （unmutable）-- int,float,string,tuple

    - 无序数据类型 （unordered）-- set（且不重复 no Duplicate）,dictionary

3. 运算
    - 数学运算（+,-,*,/,**,//）
    - 关系运算 (>,>=,==,<=,<)
    - 逻辑运算 (and,not,or)

4. 基础语句
    - program
    - module
    - statement
    - expression
    
5. 流程控制（要求：能写代码）
    - Indentation

        指的是前面的空格（4个）或tab，表示着归属关系，这里不止是流程控制语句需要用到，函数，类等都需要用到，大家理解即可

    - 条件语句
        - if-elif-else

    - 循环语句(loop)
        - while
        - for
        - 循环里的break

            break的作用是立刻跳出当前循环，如果是嵌套循环的话，跳出的只是当前层的循环而不能跳出父循环
        - 循环里的continue

            continue的作用是立刻回到循环的开头，重新执行这次循环，如果在for循环里，当前是第二轮循环，如果执行到里continue，则会立刻执行第三轮循环。 如果在while循环里
        - range() 

6. 函数（要求：能写代码）
    - 函数的定义(define function)
        - 函数头（head）
        - 参数 (parameter or argument)
        - 返回值 (return)
    - 函数的调用(method call)

    - print()
        - print(end='')
    - return 和 print() 的区别
    - 主函数(main function)
    - 强制转换(内置函数(default function))

        把数据作为参数传入，如果可以转换的话会转换成相应的数据类型
        - int()
        - float()
        - string()
        - list()
        - tuple()
        - set()
        - dict()
        如int('10') 和 10 是一样的
        但是如果int('b') 程序就会崩掉，报错
    - I/O
     

7. 面向对象（要求：能写代码）

    这个可以做的练习是强烈推荐大家自己把stack和queue这两种数据结构自己写一遍代码，跑一跑。这个往年类似科目有考过，主要内容在week5，大家要有能力自己把ass2写出来的话，这里不用太担心。可以看一下我第五周的平时班

    - 类（class）
    - 方法（method）
        - Accessors/getter
        - Mutators/setter
        - 特殊方法（SPECIAL OPERATORS）
            - `__add__(self, other) -> self + other`
            - `__sub__(self, other) -> self - other`
            - `__eq__(self, other) -> self == other`
            - `__lt__(self, other) -> self < other`
            - `__len__(self) -> len(self)`
            - `__str__(self) -> print(self)`
    - 构造器（constructor）
    - 属性
    - 对象（object）
    - 范围（scoping），生命周期（lifetime），全局变量，局部变量
    - 继承
    - is和==的区别

8. Libraies(要求：能写代码)
    
    Libraies说白了就是别人写好的东西，我们下载了python，默认会加载一些python开发者们写好的东西（代码），比如上面讲到的各种数据类型等基础的东西。还有一部分东西被下载下来了，但是没有加载，因为有的时候并不会用到，所以大家需要用的时候主动加载它们即可，它们就是默认的standard libiaries

    那么如何加载呢？我们这里说加载，其实更像是一种导入，把别人已经写好的东西导入我们的文件里，语法为 import 包名，比如 import math 或 from math import *, *意思为导入所有内容， 我们当然也可以有选择性的导入 

    当然还有一些别人写好的，但是我们没有下载下来的东西（功能代码），这种常常称为External libraries， 常见的有 numpy（基础数据分析的数据结构和部分数学方法）, pandas（表格）, SciPy（数学方法）, Matplotlib(可视化)

    我们也可以导入自己写好的代码，

    要求细节：
    1. 大家需要会import和会简单的使用Matplotlib，因为ass2用到了，可能会考
    2. ppt那些例题看一下，代码要能看懂


9. Testing（要求：看懂代码）
    - 不同的测试类型和规模
    - debug 方法 print()和assert

10. Error和Exception（要求：看懂代码）
    大家要能区分这三种错误
    - Syntax errors
    - Run-time errors
    - Logic errors
    - try-except-else-finally

-------------------------------------
## 第二部分 ---- 数据结构

数据结构这个部分相对比较复杂，最起码最起码最起码大家要理解思想，其次要会一些简单的数据结构代码

1. 默认数据结构-上面已经讨论过了

2. Stack(要求：会写代码)
    - 特点：LIFO (Last-In-First-Out)
    - 操作（方法）：push, pop, peek
    - 注意：单指针top，但是实际python代码不涉及这个top指针(HD+要求)

3. Queue(要求：会写代码)
    - 特点：FIFO (First-In-First-Out)
    - 操作（方法）：Enqueue, dequeue, append, serve, peek
    - 注意：双指针H 和 R， 实际python代码不涉及这两个指针(HD+要求)

4. Tree(要求：概念理解)
    - root, leaf, parent, child nodes
    - Tree search: BFS, DFS

5. Binary search tree (要求：概念理解) - BST
    - 特点：
        1. Nodes in left subtree < the root
        2. Nodes in right subtree > the root.
        3. The left and right subtree each must also be a BST
    - 必须会构建二叉搜索树
    - Tree imbalance

6. Heap（要求：概念理解）
    - 特点：the top element is the smallest of all elements for min-heap, or biggest for max-heap
    - 必须会构建二叉堆，添加和删除，这些操作需要会通过list形式展示

--------------------------------------
## 第三部分 算法

算法的实现常常要依赖于数据结构，算法的话，大概率会考验大家的理解能力。代码会考验一些简单的排序和查询算法。

1. 时间复杂度（要求：概念理解）

    时间复杂度简单来说就是代码总共执行了多少行，我们通过大O表示法表示

    - 时间复杂度比较:

        O(n!) > O(2^n) > O(n^2) > O(nlogn) > O(n) > O(logn) > O(1) 

2. 查询算法（要求：会写代码）
    - 线性查询
        - 算法复杂度 n
    - 二分查找
        - 算法复杂度 log(n)

3. 排序算法（要求：部分会写代码，部分概念理解）
    - 会写简单的排序如 bubble sort

    - 算法复杂度查询表

    |Algorithm  |Time Complexity(worst)|Time Complexity(best)|Stablility|
    |-----------|----------------------|---------------------|----------|
    |Bubble     |n^2                   |n                    |Stable    |
    |Selection  |n^2                   |n^2                  |Unstable  |
    |Insertion  |n^2                   |n                    |Stable    |
    |Quick      |n^2                   |nlog(n)              |Unstable  |
    |Merge      |nlog(n)               |nlog(n)              |Stable    |

4. 递归（要求：概念理解）
    - 自己调用自己

5. 贪心（要求：概念理解）
    - 局部最优

6. 分治（要求：概念理解）
    - 大问题拆成小问题

7. 枚举（要求：概念理解）
    - 列出所有可能性

8. 回溯（要求：概念理解）
    - 会退回之前状态
    


   
    
        



