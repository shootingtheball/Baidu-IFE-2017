一、 Html:

1，sort里面的比较函数，因为数组是二维的，所以稍作修改 

2，发现不能对空内容设置nodeValue，于是只能用innerHTML在父元素里面放了一个"1"

3，有关那个字符串，我发现数组也得用+连接。但不需要加引号，可能是因为数组里的数据格式本身就是现成的，文本加了引号，数字没有加引号

二、 Html-improve1

1，改进了sort函数

2，用了更加粗暴的innerHTML,不过是在创造出来的li元素里

三、Html-improve2

1，不是在li元素里使用innerHTML,而是把li包含在字符串里，在外部的ul元素上使用。

2，因为不是在改变子元素的内容，然后用appendChild粘到父元素上，少了粘贴这个动作，就得用+=
