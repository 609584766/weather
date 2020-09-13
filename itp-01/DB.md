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

![](itp-01/database.png)