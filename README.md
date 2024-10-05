create database if not exists instagram;
use instagram;
create table user(
id int ,
age int,
name varchar(30) not null,
email varchar(50) unique,
follower int default 0,
following int 
);
CREATE TABLE post (
    id INT PRIMARY KEY,
    content VARCHAR(100),
    user_id INT,
    foreign key (user_id) references user(id)
);
drop table user;
drop database collage;

