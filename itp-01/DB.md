CREATE TABLE host (
id INT auto_increment,
name VARCHAR(30) NOT NULL,
address VARCHAR(50),
phone VARCHAR(15),
PRIMARY KEY (id)
) ENGINE = innodb;

CREATE TABLE user (
id INT auto_increment,
name VARCHAR(30) NOT NULL,
address VARCHAR(50),
phone VARCHAR(15),
PRIMARY KEY (id)
) ENGINE = innodb;

CREATE TABLE password (
id INT auto_increment,
price INT,
userid INT,
PRIMARY KEY (id),
FOREIGN KEY (userid) REFERENCES user(id)
) ENGINE = innodb;

![](weather/itp-01/database.png)
<img width="415" alt="database" src="https://user-images.githubusercontent.com/70703392/93009200-b23e4880-f54b-11ea-87ed-27cbf6a678a9.png">
