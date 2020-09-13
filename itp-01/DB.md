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
%E6%88%AA%E5%B1%8F2020-09-12%E4%B8%8B%E5%8D%8810.19.38.png