Creating a books table
````
CREATE TABLE `it book store`.`books` (
  `BookID` INT(255) NOT NULL AUTO_INCREMENT,
  `Title` VARCHAR(255) NOT NULL,
  `Authors` TEXT NOT NULL,
  `InventoryStatus` TEXT NOT NULL DEFAULT 'in stock',
  `Price` INT(255) NOT NULL,
  PRIMARY KEY (`BookID`)
) ENGINE=InnoDB;
INSERT INTO `books`(`BookID`, `Title`, `Authors`, `InventoryStatus`, `Price`)
VALUES 
    (1, 'The Phoenix Project', 'Gene Kim and Kevin Behr', 'in stock', 25.99),
    (2, 'Clean Code: A Handbook of Agile Software Craftsmanship', 'Robert C. Martin', 'in stock', 32.50),
    (3, 'Artificial Intelligence: A Guide for Thinking Humans', 'Melanie Mitchell', 'out of stock', 19.95),
    (4, 'Cracking the Coding Interview: 189 Programming Questions and Solutions', 'Gayle Laakmann McDowell', 'in stock', 28.00),
    (5, 'The DevOps Handbook: How to Create World-Class Agility, Reliability, and Security in Technology Organizations', 'Gene Kim, Patrick Debois, John Willis, and Jez Humble', 'out of stock', 34.99),
    (6, 'The Pragmatic Programmer: Your Journey to Mastery', 'Andrew Hunt and David Thomas', 'in stock', 22.75),
    (7, 'Python Crash Course: A Hands-On, Project-Based Introduction to Programming', 'Eric Matthes', 'in stock', 19.95),
    (8, 'Design Patterns: Elements of Reusable Object-Oriented Software', 'Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides', 'out of stock', 27.50),
    (9, 'Data Science for Business: What You Need to Know about Data Mining and Data-Analytic Thinking', 'Foster Provost and Tom Fawcett', 'in stock', 23.99),
    (10, 'Deep Learning', 'Ian Goodfellow, Yoshua Bengio, and Aaron Courville', 'out of stock', 29.95);
````

![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/6ef57d6e-4d55-42e6-bab9-dcb6836f34ae)

