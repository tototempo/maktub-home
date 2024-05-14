# Maktub Home

## 1. Introduction
Maktub Home is a web application designed for a home decor business. It features a _Single Page Application (SPA)_ for the frontend developed using **Vue.js**, enabling users to browse and purchase products seamlessly, and an admin dashboard for managing the inventory and orders. The backend of the application is built using **Laravel** and **MySQL**.

## 2. Table of Contents
1. [Technologies Used](#3-technologies-used)
2. [About](#4-about)
   - [Client Page](#client-page)
   - [Admin Page](#admin-page)
3. [Key Learnings](#5-key-learnings)
4. [Gallery](#6-gallery)
   - [Screenshots](#screenshots)
   - [Videos](#videos)

## 3. Technologies Used
- **Frontend:** Vue.js (SPA, Vue Router, Vuex), Vite, Bootstrap, CSS
- **Backend:** PHP, Laravel, Eloquent ORM
- **Database:** MySQL (Amazon RDS)
- **Deployment & Server:** AWS EC2, Apache
- **APIs:** Custom APIs developed in Laravel, QuickChart API
- **Development Tools:** npm
- **Version Control:** Git

## 4. About
Maktub Home was developed to provide a modern, efficient, and user-friendly e-commerce platform for a local home decor business. 
The project integrates the latest web development technologies to ensure a smooth user experience and robust backend management.
It is built by myself from 0 while I was learning to use Laravel, Vue.js and the other technologies mentioned above.
The web app consists of two main views:
### Client Page
- Developed with **Vue.js, Vuex and Vue Router**.
- Smooth animations using latest **CSS3** features.
- Catalog filter and search.
- **Real time update of product's stock** (If 'x' buys the last unit of a product that 'y' has in it's cart it will automatically be updated thanks to Vuex and let 'y' know that that product is out of stock).
- Complete [cart and checkout experience.](Client/Order%20Creation%20Flow.mp4).
- Mailing upon succesful order creation using **Amazon SES** to both the client and admin. [Click here](Client/Mail%20of%20Order.mp4) to see the email the client receives.
- Order search using randomly-generated order number and real time update of order status. [Click here](Client/Order%20Search%20&%20Status%20Update%20From%20Admin%20Manager.mp4) to see a video showcase of this feature.
- Data sanitization using **DOMPurify** library and data encryption using **CryptoJS** & **Laravel's OpenSSL**.
- Implemented **SEO strategies** for improved search engine visibility and ranking.
- Implemented performance optimization techniques including **lazy loading** (_for large files and routes in Vue Router_), **image compression** (_Apache's mod_deflate module_), and code minification for enhanced user experience and faster page loading times.
- Enhanced security measures such as **HTTPS**, HSTS CSRF protection, and XSS prevention to safeguard user data and prevent malicious attacks.
- The site tracks user's metrics such as time spent on the page and visited products, enabling deeper insights for optimization and refinement.
### Admin Page
- Secure authentication using Laravel's built-in library.
- Enhanced **security measures** include:
  - **Verification of user's IP address** for admin login authentication. [Click here](https://youtu.be/ys5cFIo-mnw) to see a video demo of it.
  - Implementation of additional _passkey_ authentication for unregistered IPs to access the login.
  - Automated IP banning mechanism for excessive login attempts.
  - Other security measures like **CORS**, **XSS Protection**, **Rate Limiting**, etc.
- Complete **admin dashboard** for managing products, orders, discount codes and assets.
- Comprehensive statistics dashboard enabling detailed analysis of specific metrics for individual months.
- Graph generation using **Quickchart API** to provide deeper insights in statistics for different periods of time. [Click here](https://youtu.be/SoI5PCMuKNI) to see a video demo of it.
- **Notification** system for order creations, new IP's registered and statistics.
- Frontend developed with **Blade**, **Bootstrap** and **CSS**.

## 5. Key Learnings
Developing Maktub Home provided valuable experience in:
- Building a full-stack web application using Laravel and Vue.js.
- Implementing state management with Vuex and routing with Vue Router.
- Deploying web applications on AWS EC2 instances and using Amazon RDS for database management
- Ensuring secure and efficient data handling and user authentication processes.

## 6. Gallery
Below are some screenshots and videos showcasing the functionality and design of Maktub Home.

### Screenshots
#### Landing Page
 ![Client Landing Page](Screenshots/Client%20Landing%20Page.PNG)
#### Cart
![Client Cart](Screenshots/Client%20Cart.PNG)
#### Catalog
![Client Catalog](Screenshots/Client%20Catalog.PNG)
#### Admin Stat Dashboard
![Admin Stat Dashboard](Screenshots/Admin%20Stat%20Dashboard.PNG)
#### Admin Stats Graph Example
![Admin Stat](Screenshots/Admin%20Stats.PNG)

### Videos
Here are some videos showcasing the website functionality. Feel free to explore the repo and take a look at all of them!
#### Order Creation Flow

#### Mail of Order

#### Admin Asset Manager
[![Admin Asset Manager](https://i9.ytimg.com/vi/MINBuPo4vKw/mqdefault.jpg?sqp=CLS7j7IG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGCggOih_MA8=&rs=AOn4CLDUpSI-dVMVvvJqcBkDGNmXVx99Ig)](https://youtu.be/SoI5PCMuKNI)

Feel free to explore the repository to learn more about the project. If you have any questions or suggestions, please don't hesitate to reach out.
