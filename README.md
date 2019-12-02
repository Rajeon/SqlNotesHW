What is MySQL:
MySQL is a fast, easy to use relational database. It is currently the most popular open-source database. It is very commonly used in conjunction with PHP scripts to create powerful and dynamic server-side applications.

MySQL is used for many small and big businesses. It is developed, marketed and supported by MySQL AB, a Swedish company. It is written in C and C++.

Insert Into users(first_name, last_name, email, password, location, dept, is_admin, register_date)
Values ('John', 'Doe', 'JohnDoe@gmail.com', '654321', 'Massachusetts', 'devleopment', 1, now());

Select * From users;

Select * From users Where location='Massachusetts' And dept='sales';

Select * From users Where id_admin > 0;

Delete From users WHere id= 6;

Update users Set email= 'freddy@gmail.com' Where id = 2;

Select * From users Order By last_name ASC;

Select Distinct loaction From users;

Select location From Users;

Select * From users Where dept Like '%t%';

Select
users.first_name,
users.last_name,
post.title,
post.publish_date
From users
Inner Join posts
On users.id = posts.user_id
Order By posts.

Select
comments.body,
post.title,
users.first_name,
users.last_name
From comments
Inner Join posts On posts.id = commments.post_id
Inner Join users On users.id = comments.user_id
Order By post.title

Select UCASE(first_name), LCASE(last_name) From users;
Select location, Count(location) From users Where loaction = 'Massachusetts' Group By location;

truncate table customers;  

drop table customers;  
