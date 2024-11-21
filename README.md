# RFID-based-Inventory-Management-System
A streamlined RFID-based Inventory Management System combining online orders and in-store purchases. Features real-time stock updates, RFID tag scanning, customer registration, and order verification. Uses PHP, MySQL, Firebase (for UID sync), and runs on XAMPP. Integration of systems is in progress.

RFID-Based Inventory Management System
1.	Project Overview
This project involves the design and development of an RFID-based Inventory Management System that integrates both online and offline purchase methods. The system allows customers to register on the website, place orders online, or directly buy from a physical store. It ensures that inventory data is updated in real-time, providing accurate stock levels on the website and preventing discrepancies.
Additionally, the system incorporates Firebase for real-time UID updates when RFID tags are scanned. Although the integration of Firebase with the website is not complete, two separate systems have been developed:
A local host/website using PHP and MySQL for customer and inventory management.
A system that pushes scanned RFID tag UIDs to Firebase.

2.	Hardware Components
The following hardware components are used in the project:
a.	RAIN RFID / RC522 RFID Module
Scans RFID tags attached to items in the store for inventory management.
b.	Round Tag
An RFID tag attached to each item to uniquely identify the product.
c.	ESP32
A microcontroller used to interface the RFID module with the system and send UIDs to Firebase.
d.	Buck Converter
Regulates the power supply to the ESP32 and other components from the battery source.
e.	Battery Source
Provides the necessary power to the system.

3.	Software Stack
The software components used in this project include:
Frontend: HTML, CSS, JavaScript
Provides the user interface for the website where customers can register, view products, and place orders.
Backend: PHP
Manages customer registration, order processing, and communication with the database.
Database: MySQL (Local) & Firebase (for UID handling) 
MySQL stores customer data, inventory details, and order information.
Firebase receives and processes UIDs from scanned RFID tags for future integration with the website.

4.	Workflow
4.1. Online Order Workflow
a)	Customer Registration:
Customers register on the website by providing details like name, contact information, and shipping address.
b)	Placing an Order:
Customers browse the product catalog on the website and place orders for desired items.
c)	Order Verification:
The distributor verifies and confirms orders. Upon confirmation, the database updates the order details, and the website reflects changes in the inventory.
d)	Stock Management:
The ordered quantity is deducted from the stock, and the updated inventory is displayed. Out-of-stock items trigger an appropriate notification on the website.
4.2. Store Purchase Workflow
a)	RFID Tag Scanning:
Items purchased in-store are scanned using the RFID reader module. The scanned UID is sent to Firebase.
b)	Billing:
The system retrieves item details from the database, and the billing process is initiated.
c)	Inventory Update:
The inventory in the database is updated and reflected on the website. Notifications are displayed for out-of-stock items.

5.	Features
a)	Real-Time Stock Updates:
Inventory levels are dynamically updated for both online and in-store purchases.
b)	Customer Registration:
Users can register, track orders, and manage their profiles.
c)	Stock Alerts:
Notifications are automatically sent for out-of-stock items.
d)	Order Management:
Orders placed online are verified by a distributor before confirmation.
e)	UID Integration with Firebase:
RFID tag UIDs are pushed to Firebase for real-time updates (integration with the website is ongoing).

6.	Future Enhancements
a)	Firebase and Website Integration:
Full synchronization of Firebase data with the website for seamless inventory updates.
b)	Blockchain Integration:
To enhance the security of inventory and order tracking.
c)	Mobile App Development:
A mobile app for customers to place orders and track inventory on the go.

7.	Conclusion
The RFID-Based Inventory Management System offers an efficient solution for managing inventory across both online and offline sales channels. While currently divided into two separate systems, the planned Firebase integration will enable seamless real-time updates. The system ensures accurate stock tracking, real-time updates, and a smooth customer experience, with potential for future expansions like blockchain and mobile app support.

