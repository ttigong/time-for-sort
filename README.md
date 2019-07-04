# 常用排序算法速度比较

[排序算法](https://en.wikipedia.org/wiki/Sorting_algorithm)在计算机科学的理论和应用中具有重要价值。本人使用 [Python](https://www.python.org/) 语言，对常用的六种[排序算法](https://en.wikipedia.org/wiki/Sorting_algorithm)，包括[冒泡排序](https://en.wikipedia.org/wiki/Bubble_sort)、[插入排序](https://en.wikipedia.org/wiki/Insertion_sort)、[选择排序](https://en.wikipedia.org/wiki/Selection_sort)、[归并排序](https://en.wikipedia.org/wiki/Merge_sort)、[快速排序](https://en.wikipedia.org/wiki/Quicksort)以及 [Timsort](https://en.wikipedia.org/wiki/Timsort) 进行了速度对比，其中 [Timsort](https://en.wikipedia.org/wiki/Timsort) 用 [Python](https://www.python.org/) 解释器内置的 [sorted()](https://docs.python.org/3/library/functions.html#sorted) 函数予以实现，其余算法采用本人编写的代码。实验平台为本人古董级的联想 Y470 笔记本电脑 (Intel Core i3-2310M CPU @ 2.10 GHz)，操作系统为 Windows 7 64 位，[Python](https://www.python.org/) 版本为 3.7.3，采用 [Jupyter Notebook](https://jupyter.org/) 实现代码。实验采用两种方法，其一是对 0 到 9999 这 10000 个整数随机打乱后计算每种算法对同一打乱序列排序所用的时间，其二是随机生成 10000 个 [0.0, 1.0) 均匀分布的浮点数，计算每种算法对同一生成序列排序所用的时间。两种方法的结果相一致，算法用时按照从大到小的顺序依次为：[冒泡排序](https://en.wikipedia.org/wiki/Bubble_sort) > [插入排序](https://en.wikipedia.org/wiki/Insertion_sort) > [选择排序](https://en.wikipedia.org/wiki/Selection_sort) > [归并排序](https://en.wikipedia.org/wiki/Merge_sort) > [快速排序](https://en.wikipedia.org/wiki/Quicksort) > [Timsort](https://en.wikipedia.org/wiki/Timsort)，其中最长用时与最短用时大约相差 4 个数量级。

本实验只是一个用于演示的简单实验，所用序列完全随机且不含有重复元素。进一步的实验可尝试近似随机，近似有序，含有重复元素，重复元素分布集中或分散等多种类型的序列，也可以增加其他[排序算法](https://en.wikipedia.org/wiki/Sorting_algorithm)。

更详细的内容请参考发布于[知乎](https://www.zhihu.com/)上面的[这篇文章](https://zhuanlan.zhihu.com/p/72147937)。