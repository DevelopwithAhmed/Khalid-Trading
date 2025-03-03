# Khalid-Trading
Online Shopping Website

Overview

This is an Angular-based online shopping website featuring various product categories, including fruits, vegetables, meat, and furniture. The website provides a responsive and user-friendly interface with an intuitive navigation menu.

Features

Home Page: Overview of the website.

Products Page: Displays different product categories (Fruits, Vegetables, Meat, Furniture).

Product Details: Detailed information on each product.

Navigation Menu: Includes a mobile-friendly hamburger menu that auto-closes on link click.

Responsive Design: Optimized for mobile, tablet, and desktop screens.

Technologies Used

Frontend: Angular, TypeScript, HTML, CSS

Styling: SCSS, Flexbox, Grid

Routing: Angular Router

Installation

To set up the project locally, follow these steps:

Clone the repository:

git clone https://github.com/your-username/your-repository.git

Navigate to the project folder:

cd your-repository

Install dependencies:

npm install

Run the development server:

ng serve

Open the browser and go to:

http://localhost:4200

Folder Structure

src/
│-- app/
│   │-- components/
│   │   │-- header/
│   │   │-- products/
│   │   │-- product-details/
│   │-- services/
│-- assets/
│-- styles/
│-- index.html

Navigation Menu Issue Fix

To ensure the mobile navigation menu closes after clicking a link, the closeMenu() function is used in header.component.ts:

closeMenu() {
  const checkBox = document.getElementById('check') as HTMLInputElement;
  if (checkBox) {
    checkBox.checked = false;
  }
}

And each navigation link includes:

<a [routerLink]="['/home']" (click)="closeMenu()">Home</a>

Contributing

Fork the repository.

Create a new branch (git checkout -b feature-name).

Commit your changes (git commit -m 'Add new feature').

Push to the branch (git push origin feature-name).

Open a pull request.

License

This project is licensed under the MIT License.

Contact

For any questions, feel free to contact:

Email: your-email@example.com

GitHub: Your GitHub Profile

