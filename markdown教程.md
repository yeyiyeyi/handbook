# <一> 标题

文字前面带有几个#就代表了几级标题，分别对应h1-h6

可以在文本下方使用====来识别一级标题，----来识别二级标题

一级标题 
=======  

二级标题
-------

>注意：不同编辑器对#的兼容性不同，请在#与文本之间留一个空格

# <二> 段落
要创建段落，请使用空白行将一行或者多行文本进行分隔  
>不要用空格(spaces)或制表符(tabs)缩进段落

   i cant see you .

dont do this. ok?  

# <三> 换行
1) 在一行的末尾添加两个或多个空格，然后按回车键，即可创建一个换行",< br >"称为结尾空格  
2) 直接在文字末尾添加"< br >"  
3) 在文字末尾直接键入回车换行
4) 最好不要使用在文字末尾添加/的方式换行

# <四> 强调

### **粗体**

在文本的前后添加两个星号**或者两个下划线__  
** text **   __ ni __  
>为兼容性考虑，若是中间文本加粗，请使用**

### **斜体**

在文本前后添加一个星号*或下划线_
>为兼容性考虑，若是中间文本斜体，请使用*  

*你好哦* * 你好哦 * _nihaoo_ _ nihaoo_   
>若要同时使用加粗和斜体 请使用*** 你好 ***

# <五> 引用语法

要创建快引用，请在段落前添加>符号  
> may i love you  

**嵌套块引用**
> may i love you
>> may i love you  

带有其他元素的块引用
> #### The quarterly results look great!
> 
> - Revenue was off the chart.
> - Profits were higher than ever.
> 
> *Everything* is going according to **plan**.  
# <六> 列表
**有序列表**  
>使用1.为兼容性考虑不要使用1）  
1. may
2. i
3. love
4. you  

**无序列表**  

在列表项前面添加破折号(-),星号(*)或者加号(+).  

缩进一个或多个列表项可创建嵌套列表。  
- may
   - i
   - love
- you 

>为了兼容性考虑，同一个列表使用相同的符号

**在列表中嵌套其他元素**  

将该元素缩进四个空格或一个制表符，并且需要上下留一个空行  

*段落*
- may
- i

    may i love you

- love
- you  

*块*  
- may
- i

    >may i love you

- love
- you   

*代码块*  

代码块通常采用四个空格或一个制表符缩进。  
当它们被放进列表中时，请将它们缩进八个空格或两个制表符。  

1. open the file.
2. may i love you  

        <html>
          <head>
            <title>Test</title>
          </head>  
3. thisone  

*图片*
1. open the file
2. may

    ![Tux,the Linux mascot](/assets/images/tux.png)  


3. close the file  

*列表*
1. first
2. second
    - indented
    - indented  
3. list

# <七> 代码  
要将单词或短语表示为代码，请将其包裹在反引号(`)中  

type `hello`  

### ***转义反引号***  

若代码的单词或短语包含一个或多个反引号，则可以使用双反引号包裹  
``use `code` in your markdown file ``  

### ***代码块***  

创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符  
    <html>
     <head>
     </head>
    </html>  
Note:创建不用缩进的代码块，使用围栏式代码块  

***围栏式代码块***  
使用受保护的代码块，在代码块之前和之后的行上使用三个反引号(```)或三个波浪号（~~~）  
```
{
    "first":"john",
    "last":"smith",
    "age":25
}  

```
***语法高亮***   
添加语法突出显示，在受防护的代码块之前的反引号旁边指定一种语言  
```json  
{
    "first":"john",
    "last":"smith",
    "age":25
}   

```    
# <八> 分割线  
在单独一行上使用三个或多个星号(***)、破折号(---)或下划线(___),并且不能包含其他内容  
***  
---  
____________  
>为了兼容性，请在分割线的前后添加空白行  
# <九> 链接  
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选  
超链接Markdown语法代码：[超链接显示名](超链接地址"超链接title")  
这是一个错误[markdown 语法](https://markdown.com.cn)  

***给链接增加Title***  

链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔  
这是一个链接 [markdown语法](https://markdown.com.cn "最好的markdown教程")  

***网址和email地址***  

使用尖括号可以很方便的把url或者email地址变成可点击的链接  
<https://markdown.com.cn>  
<face@example.com>  

***带格式化的链接***  
强调链接，在链接语法前后增加星号。要将链接表示为代码，请在方括号中添加反引号。  
i love you **[abe](https://eff.org)**.  
This is the *[Markdown Guide](https://www.markdowguide.org)*.  
see the section on [`code`](#code).  

***引用类型链接***  

**链接的第一部分格式**  
[hobbit-hole][1]  
[hobbit-hole] [1]  

**链接的第二部分格式**  
1. 放在括号中的标签，其后紧随一个冒号和至少一个空格。  
2. 链接的URL，可以选择将其括在尖括号中。  
3. 链接的可选标题，可以将其括在双引号，单引号或括号中。  

[1]:<https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"  

# <十> 图片  
添加图片，使用感叹号，在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本  
！[图片alt](图片链接"图片title")  
![这是图片](/assets.jpg "magic gardens")  

**链接图片** 

[![这是图片](/assets.jpg "magic gardens")](https://markdown.com.cn)   

# <十一> 转义字符   
**特殊字符在前面加\来转义**  
 \* without the back.   

**可以做转义的字符**  
\ ` * _ {} [] () # + - . ! |   

**特殊字符自动转义**   
< &lt ; & &amp ;  
<http://images.google.com/images?num=30&q=larry+bird>  
  
# <十二> 内嵌HTML  
对于 HTML 的块级元素 < div>、< table>、< pre> 和 < p>，请在其前后使用空行（blank lines）与其它内容进行分隔。  

尽量不要使用制表符（tabs）或空格（spaces）对 HTML 标签做缩进，否则将影响格式。

在 HTML 块级标签内不能使用 Markdown 语法。例如 < p>italic and * * bold * *</> 将不起作用。






