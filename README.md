# Maktub Home

## 1. Introduction
Maktub Home is a web application designed for a home decor business. It features a _Single Page Application (SPA)_ for the frontend, developed using **Vue.js**, which enables users to browse and purchase products seamlessly, and an admin dashboard for managing the inventory and orders. The backend of the application is built using **Laravel** and **MySQL**.

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
- **Backend:** Laravel, PHP, Eloquent ORM
- **Database:** MySQL (AWS RDS)
- **Deployment & Server:** AWS EC2, Apache, AWS SES
- **APIs:** Custom APIs developed in Laravel, QuickChart API
- **Development Tools:** npm, Composer, Laravel Tinker
- **Version Control:** Git

<img src="https://img.shields.io/badge/vue.js%20-%23323330.svg?&style=for-the-badge&logo=vue.js&logoColor=white&color=%234FC08D"/> <img src="https://img.shields.io/badge/vite%20-%23323330.svg?&style=for-the-badge&logo=vite&logoColor=%23FBC02D&color=%23646CFF"/> <img src="https://img.shields.io/badge/bootstrap%20-%23563D7C.svg?&style=for-the-badge&logo=bootstrap&logoColor=white"/> <img src="https://img.shields.io/badge/css3%20-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white"/> <img src="https://img.shields.io/badge/Laravel%20-%23323330.svg?&style=for-the-badge&logo=laravel&logoColor=white&color=%23FF2D20"> <img src="https://img.shields.io/badge/PHP%20-%23323330.svg?&style=for-the-badge&logo=php&logoColor=white&color=%23777BB4"> <img src="https://img.shields.io/badge/mysql%20-%2320232a.svg?&style=for-the-badge&logo=mysql&logoColor=white&color=%234479A1"/> <img src="https://img.shields.io/badge/Amazon RDS%20-%23323330.svg?&style=for-the-badge&logo=amazonrds&logoColor=white&color=%23527FFF"> <img src="https://img.shields.io/badge/Amazon EC2%20-%23323330.svg?&style=for-the-badge&logo=amazonec2&logoColor=white&color=%23FF9900"> <img src="https://img.shields.io/badge/Apache%20-%23323330.svg?&style=for-the-badge&logo=apache&logoColor=white&color=%23D22128"> <img src="https://img.shields.io/badge/Amazon SES%20-%23323330.svg?&style=for-the-badge&logo=amazonsimpleemailservice&logoColor=white&color=%23DD344C"> <img src="https://img.shields.io/badge/npm%20-%23323330.svg?&style=for-the-badge&logo=npm&logoColor=white&color=%23CB3837"> <img src="https://img.shields.io/badge/Composer%20-%23323330.svg?&style=for-the-badge&logo=composer&logoColor=white&color=%23885630"> <img src="https://img.shields.io/badge/Git%20-%23323330.svg?&style=for-the-badge&logo=git&logoColor=white&color=%23F05032">

## 4. About
Maktub Home was developed to provide a modern, efficient, and user-friendly **e-commerce platform** for a local home decor business. The project integrates the latest web development technologies to ensure a **smooth user experience** providing an intuitive navigation and **responsive design** across all devices as well as **robust backend** management. It was built by myself from scratch while I was learning to use Laravel, Vue.js, and the other technologies mentioned above.
The web app consists of two main views:
### Client Page
- Developed with **Vue.js, Vuex and Vue Router**.
- Smooth animations using latest **CSS3** features.
- Mobile responsiveness for seamless browsing across all devices.
- Catalog filter and search.
- **Real-time stock updates** (When a customer purchases the last unit of a product that is in another user's cart, the product's availability is automatically updated to reflect the stock status).
- Complete [cart and checkout experience.](Client/Order%20Creation%20Flow.mp4).
- Sending emails upon successful order creation using **Amazon SES** to both the client and admin. [Click here](Client/Mail%20of%20Order.mp4) to see the email the client receives.
- Order search using randomly-generated order number and real time update of order status. [Click here](Client/Order%20Search%20&%20Status%20Update%20From%20Admin%20Manager.mp4) to see a video showcase of this feature.
- Data sanitization using **DOMPurify** library and data encryption using **CryptoJS** & **Laravel's OpenSSL**.
- Implemented **SEO strategies** for improved search engine visibility and ranking.
- Implemented performance optimization techniques, including **lazy loading** (_for routes in Vue Router as well for large files_), **image compression** (_Apache's mod_deflate module_), and code minification for enhanced user experience and faster page loading times.
- Enhanced security measures such as **HTTPS**, **HSTS**, **CSRF** protection, and **XSS** prevention to safeguard user data and prevent malicious attacks.
- The site tracks user's metrics such as time spent on the page and visited products, enabling deeper insights for optimization and refinement.
### Admin Page
- Secure authentication using Laravel's built-in library.
- Enhanced **security measures** including:
  - **Verification of user's IP address** for admin login authentication. [Click here](https://youtu.be/ys5cFIo-mnw) to see a video demo of it.
  - Implementation of additional _passkey_ authentication for unregistered IPs to access the login.
  - Automated _IP banning_ mechanism for excessive login attempts.
  - Other security measures like **CORS**, **XSS Protection**, **Rate Limiting**, etc.
- Complete **admin dashboard** for managing products, orders, discount codes and assets.
- Comprehensive statistics dashboard enabling detailed analysis of specific metrics for individual months.
- Graph generation using **Quickchart API** to provide deeper insights in statistics for different periods of time. [Click here](https://youtu.be/SoI5PCMuKNI) to see a video demo of it.
- **Notification** system for order creations, new IPs registered and statistics.
- Frontend developed with **Blade**, **Bootstrap** and **CSS**.
- Mobile responsiveness for a smooth experience across all devices.

## 5. Key Learnings
Developing Maktub Home provided valuable experience in:
- Building a **full-stack** web application using modern technologies and frameworks.
- Defining, documenting, and maintaining the **requirements** for the application.
- Communicating and understanding the **client's needs** for the site.
- Developing a smooth experience for the user using a SPA and implementing **performance** optimizations for faster loading times.
- Gaining insights into user behavior through analytics and feedback mechanisms.
- Implementing **state management** for the application.
- Confronting **deployment challenges** and optimizing **server configurations** for a great application hosting.
- Ensuring secure and efficient data handling and user **authentication** processes.
- Implementing **security** measures for both the server and the client.
- Understanding and implementing **SEO strategies** for improved search engine visibility.
- Integrating **multiple technologies** within the project.

## 6. Gallery
In this section you'll find some screenshots and videos showcasing the functionality and design of Maktub Home.

### Screenshots
#### Landing Page
 ![Client Landing Page](Screenshots/Client%20Landing%20Page.PNG)
#### Cart
![Client Cart](Screenshots/Client%20Cart.PNG)
#### Catalog
![Client Catalog](Screenshots/Client%20Catalog.PNG)
#### Admin Stats Dashboard
![Admin Stat Dashboard](Screenshots/Admin%20Stat%20Dashboard.PNG)
#### Admin Graph Generation for Statistics
![Admin Stat](Screenshots/Admin%20Stats.PNG)

### Videos
Here are some videos showcasing the website functionality. I invite you to explore the repository and take a look at all of them!
#### Order Creation Flow

#### Mail Received Upon Order Creation

#### Admin Asset Manager
[![Admin Asset Manager](https://i9.ytimg.com/vi/MINBuPo4vKw/mqdefault.jpg?sqp=CLS7j7IG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGCggOih_MA8=&rs=AOn4CLDUpSI-dVMVvvJqcBkDGNmXVx99Ig)](https://youtu.be/uCMrwZqKlBU)

#### Admin Order Manager
[![Admin Order Manager](https://i9.ytimg.com/vi/uCMrwZqKlBU/mqdefault.jpg?sqp=CNj6j7IG-oaymwEmCMACELQB8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGFogZShcMA8=&rs=AOn4CLAMUTCqS8ceeUkqxreCGLtQnxyT6Q)](https://youtu.be/SoI5PCMuKNI)

Feel free to explore the repository as well as the [web page](https://maktubhome.com) to learn more about the project. If you have any questions or suggestions, please don't hesitate to reach out via [mail](mailto:tototemporelli12@gmail.com).
