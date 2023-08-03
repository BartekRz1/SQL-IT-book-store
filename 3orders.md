Creating table orders
````
CREATE TABLE `it book store`.`orders` 
(`OrderID` INT NOT NULL AUTO_INCREMENT , 
`BookID` INT NOT NULL , `CustomersID` INT NOT NULL , 
`Date` DATE NOT NULL , `Status` TEXT NOT NULL DEFAULT 
'pending' , PRIMARY KEY (`OrderID`)) ENGINE = InnoDB;

INSERT INTO `orders` (`OrderID`, `BookID`, `CustomersID`, `Date`, `Status`) 
VALUES 
  ('', 1, 2, '2023-08-03', 'pending'),
  ('', 2, 3, '2023-08-03', 'shipped'),
  ('', 4, 1, '2023-08-02', 'completed'),
  ('', 6, 4, '2023-08-01', 'pending'),
  ('', 8, 5, '2023-08-01', 'shipped'),
  ('', 10, 2, '2023-08-03', 'pending'),
  ('', 3, 3, '2023-08-02', 'completed');
````
![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/367394fb-82ac-4c88-b39f-045045b4c363)



Creating first relations in orders table

````
ALTER TABLE `orders`
ADD CONSTRAINT `fk_orders_books` FOREIGN KEY (`BookID`) REFERENCES `books` (`BookID`),
ADD CONSTRAINT `fk_orders_customers` FOREIGN KEY (`CustomersID`) REFERENCES `customers` (`CustomersID`);
````

![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/f9c43692-7cbd-4b7c-95d7-ef420dedcaf5)
