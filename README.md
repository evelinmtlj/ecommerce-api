###  🛒 Easy Shop (Backend API)

--  ###Overview

Easy Shop is a Spring Boot REST API for an e-commerce application. The backend supports product browsing, category management, product search and filtering, and role-based access for administrators. This project focused on backend development and bug fixing while working with an existing UI.

-- ### Features

 - User registration and login

 - Browse products by category

 - Search and filter products

 - Admin-only product and category management

 ###  🧩 Project Phases
Phase 1 – CategoriesController

The CategoriesController was implemented with full CRUD functionality.

Features:

 - Retrieve all categories

-  Retrieve a category by ID

- Add a new category (ADMIN only)

- Update an existing category (ADMIN only)

- Delete a category (ADMIN only)


  <img width="895" height="917" alt="image" src="https://github.com/user-attachments/assets/823dfafe-f801-4b59-880d-5fb9519ebd67" />


### Bug 1: Incorrect Search Results
Fix:

Tested search queries using different combinations of parameters

Corrected SQL logic in the DAO to properly handle optional filters

Verified results using Insomnia and unit tests
<img width="782" height="506" alt="image" src="https://github.com/user-attachments/assets/f5de491d-0b74-4b37-a097-ff7073ca4627" />

### Bug 2: Duplicate Products on Update

Issue: Updating a product created a new record instead of updating the existing one.

Fix:

Identified incorrect SQL logic using INSERT instead of UPDATE

Corrected DAO method to update products by ID

Ensured administrators can safely update products without duplication

<img width="1011" height="802" alt="image" src="https://github.com/user-attachments/assets/2b9776c6-6f00-4a92-9fcc-339cd8d14bc8" />

### Small bug in frontend 
<img width="936" height="548" alt="image" src="https://github.com/user-attachments/assets/002cb5c4-9cbd-4436-ad71-f732864a7281" />
- Fixed a front-end bug in the price filter where the minimum price label appeared twice, improving UI clarity and usability.


 ### Testing

API endpoints tested using Insomnia

Search and filter logic validated with multiple scenarios

### Conclusions 
- This project demonstrates backend API development, debugging, security enforcement, and testing using Java and Spring Boot.



  
