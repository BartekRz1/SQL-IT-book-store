Creating and Inserting table 
````
CREATE TABLE `customers` (
  `Customers ID` int(11) NOT NULL,
  `Name` text NOT NULL,
  `Last Name` text NOT NULL,
  `Emile` varchar(25) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;


INSERT INTO `customers` (`Customers ID`, `Name`, `Last Name`, `Emile`) VALUES
(1, 'olivia', 'smith', 'olivia.smith@example.com'),
(2, 'liam', 'anderson', 'liam.anderson@example.com'),
(3, 'emma', 'thomas', 'emma.thomas@example.com'),
(4, 'aiden', 'taylor', 'aiden.taylor@example.com'),
(5, 'ethan', 'johnson', 'ethan.johnson@example.com'),
(6, 'ava', 'williams', 'ava.williams@example.com'),
(7, 'noah', 'brown', 'noah.brown@example.com'),
(8, 'sophia', 'martinez', 'sophia.martinez@example.c');
````

![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/eca0056b-71cf-4e0d-b4dd-6bc817589859)



Rename Customers ID and deleting data from column emile

````
ALTER TABLE `customers` CHANGE `Customers ID` `CustomersID` INT(11) NOT NULL AUTO_INCREMENT;
UPDATE customers set emile = "";
````

![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/b274dfe2-822e-450f-9418-ce4447320fc6)


Updating data
````
UPDATE `customers` SET `Emile` = 'emma@thomas.example.com' WHERE `customers`.`CustomersID` = 3;
UPDATE `customers` SET `Emile` = 'aiden@taylor.example.com' WHERE `customers`.`CustomersID` = 4;
UPDATE `customers` SET `Emile` = 'ethan@johnson.example.com' WHERE `customers`.`CustomersID` = 5;
UPDATE `customers` SET `Emile` = 'ava@williams.example.com' WHERE `customers`.`CustomersID` = 6;
UPDATE `customers` SET `Emile` = 'noah@brown.example.com' WHERE `customers`.`CustomersID` = 7;
UPDATE `customers` SET `Emile` = 'sophia@martinez.example.com' WHERE `customers`.`CustomersID` = 8;
UPDATE `customers` SET `Emile` = 'olivia@smith.example.com' WHERE `customers`.`CustomersID` = 1;
UPDATE `customers` SET `Emile` = 'liam@anderson.example.com' WHERE `customers`.`CustomersID` = 2;
````

![image](https://github.com/BartekRz1/SQL-IT-book-store/assets/131479846/448b0337-109e-4e0e-a575-e1eb86eef8c7)
