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

