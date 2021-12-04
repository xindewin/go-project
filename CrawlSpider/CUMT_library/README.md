## 爬虫——CUMT图书馆图书信息

两个功能：

1.输入要查询的书籍名，获取一系列图书信息

```go
    Bookname:="三体"
	SearchBook(Bookname,1,10)//第二个参数为页面数，第三个是返回图书个数

//{"status":"200 ","msg":"操作成功","data":{"all":2360,"booklist":[{"bookId":413400,"name":"三体. Ⅲ. Ⅲ, 死神永生, Dead end","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-229-03093-3","pcount":3,"ecount":1,"searchCode":"I247.55/L-236.2/3","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=636363636264686C6665626A666559A1A292AA94A798A5A094A59E59643835303437373133"},{"bookId":373428,"name":"三体. Ⅹ, 观想之宙","author":"宝树著","publisher":"重庆出版社","isbn":"978-7-229-03981-3","pcount":3,"ecount":1,"searchCode":"I247.5/B-764/5","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=61625F6862645F616966569E9F8FA791A495A29D91A29B56613139313732313130"},{"bookId":1207694,"name":"三体. 第三部, 死神永生","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-229-12441-0","pcount":2,"ecount":0,"searchCode":"I247.55/1:3","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=676767676668706A6868666F6E695DA5A696AE98AB9CA9A498A9A25D683136383736303037"},{"bookId":1207692,"name":"三体. 第一部","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-229-12441-0","pcount":2,"ecount":0,"searchCode":"I247.55/1:1","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=69696969686A726C6A6A6871706B5FA7A898B09AAD9EABA69AABA45F6A3135323633393039"},{"bookId":1207693,"name":"三体. 第二部, 黑暗森林","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-229-12441-0","pcount":2,"ecount":0,"searchCode":"I247.55/1:2","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=6666666665676F696767656E6D685CA4A595AD97AA9BA8A397A8A15C673136353235383836"},{"bookId":619579,"name":"三体","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-5366-9293-0","pcount":3,"ecount":1,"searchCode":"I247.55/L-236.2/1","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=62636062696960626265579FA090A892A596A39E92A39C57623437313738393031"},{"bookId":619578,"name":"三体. II, 黑暗森林","author":"刘慈欣著","publisher":"重庆出版社","isbn":"978-7-5366-9396-8","pcount":3,"ecount":1,"searchCode":"I247.55/L-236.2/2","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=6666666665676C6A6C6B656C6A6F5CA4A595AD97AA9BA8A397A8A15C673131313337373636"},{"bookId":138688,"name":"三体问题","author":"汪家訸编著","publisher":"科学出版社","isbn":"","pcount":4,"ecount":0,"searchCode":"O933.3/W419","image":""},{"bookId":581606,"name":"《三体》中的物理学","author":"李淼著","publisher":"四川科学技术出版社","isbn":"978-7-5364-8068-1","pcount":4,"ecount":1,"searchCode":"O4-49/L-519","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=62646068616760626962579FA090A892A596A39E92A39C57623532323435353131"},{"bookId":734411,"name":"《三体》中的物理学","author":"李淼著","publisher":"湖南科学技术出版社","isbn":"978-7-5710-0148-3","pcount":1,"ecount":0,"searchCode":"O4-49/L-519.2","image":"https://unicover.duxiu.com/coverNew/CoverNew.dll?iid=62656067636360636A69579FA090A892A596A39E92A39C57623135323836363331"}]}}

```

2.输入图书id,获取图书，条码号，索书号，馆藏信息

```go
    Bookid:=589144
	SearchId(Bookid)
//map[条码号:C02132046 索书号:TP301/F-926 馆藏地点:南湖校区-南湖自然科学图书阅览室]
```

