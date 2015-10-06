WordListTranslator
==================

一个（使用Bing）可以将大量英文短语批量翻译成中文的工具

### 下载 ###
点上面的Release.zip或者点这里：https://github.com/kaedei/WordListTranslater/blob/master/Release.zip

### 为什么写它 ###
一个Web项目要进行国际化，原来的英文版分支出了一个中文版。于是阿三领导扔给了我一个大概有8700行的Excel文件，里面有项目里所有的英文短语、句子，让我把它们翻译成中文（我是项目里唯一的中国程序员）。

### 怎么使用 ###
* 1.此工具使用Access数据库，所以你的电脑上至少要有Access 2007的OLEDB驱动，当然自己去改app.config里面的连接字符串也可以。
* 2.然后在Access数据库中新建个表，至少要包含三个列【自增长ID，需要翻译的，翻译之后的】，把需要翻译的英文导入到表中的【需要翻译的】列
* 3.修改代码中的app.config文件，设置各种参数（一看即懂，不再详述），包括连接字符串、表名、列名等
* 4.（可选）代码中使用了Bing Translate API，你可能需要自己填写client id和app key。当然用我的也可以，不过我不保证能一直可用。

### 这里有一个更详细的配置方法：http://blog.sina.com.cn/s/blog_58c506600101vneu.html ###

### 运行结果 ###
最终结果会存放在Access数据库里，可以随便拿来处理。
