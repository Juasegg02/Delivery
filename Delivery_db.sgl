Create database delivery_db;

CREATE TABLE user(
   id INT primary KEY auto_increment,
   name VARCHAR(100) NOT NULL,
   email VARCHAR(100) UNIQUE NOT NULL,
   phone VARCHAR(20), 
   address VARCHAR(255) NOT NULL
   );
   
   CREATE TABLE restaurant(
   id INT PRIMARY KEY AUTO_INCREMENT,
   name VARCHAR(100) NOT NULL,
   addres VARCHAR(255) NOT NULL UNIQUE,
   phone VARCHAR(20) NOT NULL
   );
   
   CREATE TABLE products(
   id INT PRIMARY KEY AUTO_INCREMENT,
   restaurant_id INT NOT NULL, 
   name VARCHAR(100) NOT NULL,
   description TEXT,
   price DECIMAL(10,2) NOT NULL,
   FOREIGN KEY (restaurant_id) REFERENCES restaurant(id)
   );
   
   CREATE TABLE Ordes(
   id INT PRIMARY KEY AUTO_INCREMENT,
   user_id INT NOT NULL,
   restaurant_id INT NOT NULL,
   date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
   status VARCHAR(50) DEFAULT 'Pendiente',  -- Pendiente,  En camino, Entregado, Cancelado
   FOREIGN KEY(user_id) REFERENCES user(id),
   FOREIGN KEY (restaurant_id) REFERENCES restaurant(id)
   );
   
   CREATE TABLE. order_details(
   id INT PRIMARY KEY AUTO_INCREMENT,
   order_id INT NOT NULL, 
   product_id INT NOT NULL,
   quantity INT NOT NULL,
   unitary_price DECIMAL(10,2) NOT NULL,
   FOREIGN KEY (order_id) REFERENCES orders(id),
   FOREIGN KEY (product_id) REFERENCES productos(id)
   );
