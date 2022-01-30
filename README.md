# Assignment-Week-5
MySql week5 homwork

###要求三：SQL CRUD

1.使用 INSERT 指令新增一筆資料到 member 資料表中，這筆資料的 username 和
password 欄位必須是 test。接著繼續新增至少 4 筆隨意的資料。

![image](https://user-images.githubusercontent.com/8243103/151700141-095af964-29e7-4942-b0ac-91bf0a3df897.png)
![image](https://user-images.githubusercontent.com/8243103/151700149-510c7aaa-e52f-42ab-a509-168d462067c4.png)

2.使用 SELECT 指令取得所有在 member 資料表中的會員資料。
![image](https://user-images.githubusercontent.com/8243103/151700161-b18aca62-c5b7-4d8a-afe7-c0b973b38725.png)


3.使用 SELECT 指令取得所有在 member 資料表中的會員資料，並按照 time 欄位，由
近到遠排序。
![image](https://user-images.githubusercontent.com/8243103/151700194-95f9b869-dbb2-4961-bae7-ff9d2dfacf75.png)


4.使用 SELECT 指令取得 member 資料表中第 2 ~ 4 共三筆資料，並按照 time 欄位，
由近到遠排序。( 並非編號 2、3、4 的資料，而是排序後的第 2 ~ 4 筆資料 )

![image](https://user-images.githubusercontent.com/8243103/151700207-a76aa565-6e8f-4d56-9538-0e853ff7c8dc.png)


5.使用 SELECT 指令取得欄位 username 是 test 的會員資料。

![image](https://user-images.githubusercontent.com/8243103/151700224-dca378db-1b54-4cb5-8b39-16b51de61705.png)


6.使用 SELECT 指令取得欄位 username 是 test、且欄位 password 也是 test 的資料。

![image](https://user-images.githubusercontent.com/8243103/151700237-cea97ea1-ae2c-4304-929c-478d8f7c46f4.png)


7.使用 UPDATE 指令更新欄位 username 是 test 的會員資料，將資料中的 name 欄位
改成 test2

![image](https://user-images.githubusercontent.com/8243103/151700244-d5168575-f9e8-4791-8345-aa584828a0a0.png)


###要求四：SQL Aggregate Functions

1.取得 member 資料表中，總共有幾筆資料 ( 幾位會員 )

![image](https://user-images.githubusercontent.com/8243103/151700255-43c62595-6d03-4b26-8561-ab84b655db2e.png)


2.取得 member 資料表中，所有會員 follower_count 欄位的總和。

![image](https://user-images.githubusercontent.com/8243103/151700261-0e031f18-1234-4fb5-ad0e-e9d61c45d78d.png)


3.取得 member 資料表中，所有會員 follower_count 欄位的平均數。

![image](https://user-images.githubusercontent.com/8243103/151700268-b6402a6a-df81-4eac-be0c-14400d0ee060.png)


###要求五：SQL JOIN (Optional)

![1643546283437](https://user-images.githubusercontent.com/8243103/151699958-13723f4d-4f91-430c-8f96-60b8dbe8ae8a.jpg)


1. 使用 SELECT 搭配 JOIN 語法，取得所有留言，結果須包含留言者會員的姓名。

語法:
mysql> SELECT message.content,member.username
    -> FROM message INNER JOIN member
    -> ON message.member_id=member.id;
![image](https://user-images.githubusercontent.com/8243103/151700281-53f279f0-7e32-4eb5-9de3-864c0e33f59d.png)


2. 使用 SELECT 搭配 JOIN 語法，取得 member 資料表中欄位 username 是 test 的所有
留言，資料中須包含留言者會員的姓名。

![image](https://user-images.githubusercontent.com/8243103/151700594-a9657ff7-3362-44c5-b58b-8421eebbf886.png)



