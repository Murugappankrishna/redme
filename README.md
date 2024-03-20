
# Shopping Billing Management 

## Front-End
### Key Features

1. **Product Management:** This system offers the capability to add, edit, and delete products from the inventory. Each product can be described with details such as ID, name, price, description, and image link.

2. **User-Friendly Interface:** With an responsive user interface, users can easily navigate through various functionalities including adding products to the cart and managing inventory.

3. **Responsive Design:** The design is optimized for different screen sizes, ensuring a seamless experience across various devices. This is achieved through the use of media queries in CSS.

4. **Data Persistence:** Utilizing local storage, the system ensures that user data, such as items added to the cart, remains intact even if the webpage is refreshed or closed temporarily.

5. **Null Field Validation:** JavaScript validation is implemented to ensure that all required fields are filled out before any product-related action is performed. This prevents unintended behavior and ensures data accuracy.

### Live Demo and Website Deployment 
- **Live Demo:** [Link to the deployed website](https://solartis-shoppingbilling-management.netlify.app/)
- **Deployment:** The following site  is deployed using **Netlify** services 


###  Source Code Repository
- **GitHub Repository:** [Link to the GitHub repository](https://github.com/Murugappankrishna/Solartis_Front_End_final)

- **To Get The File**- `git clone https://github.com/Murugappankrishna/Solartis_Front_End_final.git`

### Quick Start
1. Clone the repository to your local machine.
2. Navigate to the `login.html` file located at `Solartis_Front_End_final/login/login.html`.
3. Open `login.html` in your preferred web browser to start using the application.

### File Structure
- The project directory structure is organized as follows:

```
project-root/
│
├── home/
│   ├── homepage.css
│   └── homepage.html
│
├── login/
│   ├── login.css
│   └── login.html
│
├── Edit/
│   ├── edit.css
│   ├── edit.html
│   └── edit.js
│
├── add/
│   ├── add.css
│   ├── add.html
│   └── add.js
│
├── cart/
│   ├── cart.css
│   ├── cart.html
│   └── cart.js
│
├── delete/
│   ├── delete.css
│   ├── delete.html
│   └── delete.js
│
└── products.js
```
### User Interface/Features Screenshots
- Login Page
  
![Login Page](Screenshots/LoginPage.png)
- Home Page
  
![Home Page](Screenshots/HomePage.png)

- Responsive Home Page
  
![Responsive Page](Screenshots/Intreactive2.png)

- Code Implementation
  
```
CSS
/* Media query for screen width up to 1000px */
@media (max-width: 1000px) {
  .container {
    grid-template-columns: repeat(2, 233px);
  }
}
```

```
CSS
/* Media query for screen width up to 500px */
@media (max-width: 500px) {
  .container {
    grid-template-columns: repeat(1, 233px);
  }
```
- Add Products Page
  
![Add Products Page](Screenshots/AddPage.png)
- Edit Products Page
  
![Edit Products  Page](Screenshots/EditPage.png)
- Remove Product
  
![Remove Product Page](Screenshots/DeletePage.png)
- View All Products
  
![All Product Page](Screenshots/ProductsPage.png)
- Cart Page
  
![All Product Page](Screenshots/AddToCart.png)
- Responsive Cart Page

![All Product Page](Screenshots/CartIntreactive1.png)
- Usage Of Local Storage
  
![Remove Product Page](Screenshots/localstorage.png)

- Code Implementation
  
```
JavaScript
// Retrieve products from local storage
shopItems = JSON.parse(localStorage.getItem("products"));
```

```
JavaScript
// Set default products if local storage is empty
if (!localStorage.getItem("products")) {
  localStorage.setItem("products", JSON.stringify(shopItemsData));
}
```

