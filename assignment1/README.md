# python-data-assignments/assignment1/
Ctrip Dataset
======
Data Source
-------
#This dataset contains top news in Associated Press on Ctrip website starting page:https://apnews.com/apf-topnews
#我在做编码的时候遇到的困难，第一个问题是如何append的问题，包括在写csv的时候即使参考了note里给的sample，但还是没有做出csv，在问了helper徐雯的时候，她告诉我应该要让元素在一个list里，我的是字符串，所以要先建一个空的list，用append。第二个问题是如何在link前面加上https://apnews.com， 因为我做出来的是只有后面的数字，这个问题，我和徐雯一起去问了学长，后来学长教的我们，另外学长还告诉了我么写csv的时候把w变成a，就可以把每天爬的数据append在一起，呈现在csv上。第三个问题是我在去重的时候，用pandas却读不出来csv文件，Google后发现要加一个delimiter='\t'，可以读出来，但是却无数据，问了老师之后，老师说要把t变成“，”就可以了。第四个是最后把去重后的内容重新放入csv里，结果csv内容无变化，问了老师之后，老师告诉我的内容是dfc的内容，但是我最后原本dfc.to_ csv的时候却错打成了df.to_csv 还有一个问题是，在爬地点的时候，发现地点和文本内容是一起的，无法切割出来，后来就请教了学长，学长告诉应该用split('(')[0] 语法。

Data fields
-------
* `Headlines`-String.e.g. `Writer Haruki Murakami plans archive at Japanese university`

* `Times` - Data String.e.g. `November 9, 2018`
* `Places`- String.e.g. `THOUSAND OAKS, Calif.`
* `Links`- url.e.g. `https://apnews.com/02bebe042ba94f68b510b918d9fb6d04`
* `Authors`-Srting.e.g. `By KRYSTA FAURIA and JONATHAN J. COOPER`
* `Tags`-String.e.g. `Los Angeles`

Data Volume
----------
#190 rows 3 colums

License
-------
#CC 4.0
