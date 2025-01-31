#Database MySQL
---
CREATE DATABASE parking_system;

USE parking_system;

CREATE TABLE parking_records (
    id INT PRIMARY KEY AUTO_INCREMENT,
    license_plate VARCHAR(20) NOT NULL,
    vehicle_type ENUM('CAR', 'MOTORCYCLE') NOT NULL,
    check_in_time DATETIME NOT NULL,
    check_out_time DATETIME,
    fee INT NOT NULL,
    is_ticket_lost BOOLEAN DEFAULT FALSE
);
---
