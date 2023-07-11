CREATE DATABASE tourism;
USE tourism;
CREATE TABLE destinations (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    country VARCHAR(100) NOT NULL,
    description TEXT,
    rating FLOAT
);
CREATE TABLE hotels (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    destination_id INT,
    rating FLOAT,
    address TEXT,
    FOREIGN KEY (destination_id) REFERENCES destinations(id)
);
CREATE TABLE bookings (
    id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    hotel_id INT,
    check_in_date DATE,
    check_out_date DATE,
    FOREIGN KEY (hotel_id) REFERENCES hotels(id)
);
INSERT INTO destinations (name, country, description, rating)
VALUES
    ('Bali', 'Indonesia', 'Bali is a beautiful island known for its stunning beaches and rich culture.', 4.7),
    ('Paris', 'France', 'Paris is the capital of France and a global center for art, fashion, and culture.', 5.0),
    ('Tokyo', 'Japan', 'Tokyo is a vibrant metropolis that blends modernity with traditional Japanese culture.', 4.8);
INSERT INTO hotels (name, destination_id, rating, address)
VALUES
    ('Hotel A', 1, 4.2, '123 Beach Road, Bali, Indonesia'),
    ('Hotel B', 1, 4.6, '456 Sunset Boulevard, Bali, Indonesia'),
    ('Hotel C', 2, 4.8, '789 Avenue des Champs-Élysées, Paris, France'),
    ('Hotel D', 3, 4.5, '321 Shinjuku Street, Tokyo, Japan');
INSERT INTO bookings (guest_name, hotel_id, check_in_date, check_out_date)
VALUES
    ('Kana Hanazawa', 1, '2023-08-01', '2023-08-05'),
    ('Konomi Suzuki', 3, '2023-09-15', '2023-09-20'),
    ('Han Soohe', 2, '2023-10-10', '2023-10-15');
SELECT * FROM destinations;
SELECT * FROM hotels;
SELECT * FROM bookings;
SELECT * FROM hotels WHERE destination_id = 1;
SELECT AVG(rating) AS average_rating FROM hotels WHERE destination_id = 3;
UPDATE destinations SET rating = 5 WHERE id = 3;
UPDATE hotels SET address = '789 Aston Denpasar, Bali, Indonesia' WHERE id = 2;
DELETE FROM bookings WHERE id = 3;
INSERT INTO bookings (guest_name, hotel_id, check_in_date, check_out_date)
VALUES ('Saerom', 4 , '2023-08-01', '2023-08-05');
DELETE FROM bookings WHERE id = 1;
DELETE FROM bookings WHERE id = 2;
INSERT INTO bookings (guest_name, hotel_id, check_in_date, check_out_date)
VALUES ('Tzuyu', 1 , '2023-12-01', '2023-12-05');
INSERT INTO bookings (guest_name, hotel_id, check_in_date, check_out_date)
VALUES ('Chitanda Eru', 3 , '2023-7-01', '2023-7-05');
INSERT INTO bookings (guest_name, hotel_id, check_in_date, check_out_date)
VALUES ('Kazuha', 2 , '2023-1-01', '2023-1-05');
INSERT INTO destinations (name, country, description, rating)
VALUES ('Seoul', 'South Korea', 'It is a bustling metropolis with a blend of traditional and contemporary architecture.', 4.5);
