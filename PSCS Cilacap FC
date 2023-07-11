CREATE TABLE Players (
  id INT PRIMARY KEY AUTO_INCREMENT,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  date_of_birth DATE,
  address VARCHAR(100),
  salary DECIMAL(10, 2),
  position VARCHAR(50),
  height INT,
  weight INT
);

INSERT INTO Players (first_name, last_name, date_of_birth, address, salary, position, height, weight) VALUES
('Vio', 'Eginda', '1990-05-15', '123 Main Street', 5000.00, 'Goalkeeper', 185, 80),
('Handy', 'Sieghart', '1992-08-22', '456 Park Avenue', 6000.00, 'Defender', 180, 75),
('Terry', 'John', '1995-01-10', '789 Elm Road', 5500.00, 'Defender', 182, 78),
('Henry', 'Michael', '1993-04-05', '321 Oak Lane', 6500.00, 'Midfielder', 175, 70),
('Beckham', 'David', '1994-07-12', '654 Pine Street', 7000.00, 'Midfielder', 176, 73),
('Jon', 'Jones', '1991-11-30', '987 Cedar Avenue', 7500.00, 'Striker', 180, 75),
('Khabib', 'Nurmagomedov', '1996-03-18', '135 Maple Drive', 5500.00, 'Striker', 183, 79),
('Roberto', 'Carlos', '1992-06-25', '246 Walnut Court', 6000.00, 'Defender', 178, 77),
('James', 'Gordon', '1993-09-08', '975 Elm Street', 6500.00, 'Midfielder', 179, 72),
('Mark', 'Thompson', '1990-12-20', '864 Pine Avenue', 7000.00, 'Midfielder', 177, 74),
('Tsubasa', 'Ozora', '1994-02-03', '753 Cedar Lane', 7500.00, 'Striker', 181, 76);

CREATE TABLE Specialization (
  id INT PRIMARY KEY AUTO_INCREMENT,
  type VARCHAR(50),
  salary DECIMAL(10, 2)
);

INSERT INTO Specialization (type, salary) VALUES
('Goalkeeper', 9000.00),
('Defender', 8000.00),
('Midfielder', 9000.00),
('Striker', 11000.00);

CREATE TABLE Coach (
  id INT PRIMARY KEY AUTO_INCREMENT,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  date_of_birth DATE,
  address VARCHAR(100),
  specialization_id INT,
  FOREIGN KEY (specialization_id) REFERENCES Specialization(id)
);

INSERT INTO Coach (first_name, last_name, date_of_birth, address, specialization_id) VALUES
('Michael', 'Jordan', '1975-03-12', '123 Main Street', 2),
('Muhammad', 'Ali', '1980-06-25', '456 Park Avenue', 4),
('Gordon', 'Ramsay', '1982-09-05', '789 Elm Road', 1),
('Shaq', 'Oneal', '1978-12-10', '321 Oak Lane', 3),
('Christopher', 'Nolan', '1985-01-18', '654 Pine Street', 4),
('Anderson', 'Silva', '1983-04-20', '987 Cedar Avenue', 3);

SELECT * FROM Players;
SELECT Coach.first_name, Coach.last_name, Specialization.type, Specialization.salary
FROM Coach
INNER JOIN Specialization ON Coach.specialization_id = Specialization.id;




