# E-Commerce Website Project with Django Backend and HTML/CSS/JS Frontend



## Description

This is an E-Commerce Website project built using Django as the backend framework and HTML/CSS/JS for the frontend. The website allows users to browse and purchase various products, add them to their cart, and make payments using PayPal integration. The project aims to provide a seamless and user-friendly shopping experience.

## Features

1. User Registration and Authentication:
   - Users can sign up and create an account to log in.
   - Password reset functionality is available for users to recover their accounts.

2. Product Catalog:
   - Users can browse through the list of available products.
   - Products are categorized and can be filtered based on different attributes.
   - Product details pages showcase images, descriptions, and other relevant information.

3. Shopping Cart:
   - Users can add products to their cart and view the contents of the cart.
   - Quantity of items in the cart can be adjusted or items can be removed.

4. Checkout and Payment:
   - Users can proceed to checkout from the cart page.
   - PayPal payment gateway integration allows users to make secure payments.

5. Order History:
   - Users can view their order history and track the status of their previous purchases.

## Installation and Setup

1. Clone the repository:

```bash
git clone https://github.com/sudo-sahilroy/GreatKart-django
```

2. Navigate to the project directory:

```bash
cd ecommerce-project
```

3. Create a virtual environment (optional but recommended):

```bash
python -m venv venv
```

4. Activate the virtual environment:

   - Windows:

   ```bash
   venv\Scripts\activate
   ```

   - Linux/macOS:

   ```bash
   source venv/bin/activate
   ```

5. Install the required dependencies:

```bash
pip install -r requirements.txt
```

6. Set up the database:

```bash
python manage.py migrate
```

7. Create a superuser to access the Django admin panel:

```bash
python manage.py createsuperuser
```

8. Run the development server:

```bash
python manage.py runserver
```

9. Access the website locally by visiting `http://localhost:8000/` in your web browser.

## Configuration

To enable PayPal integration, you need to set up the following configuration:

1. Obtain PayPal API credentials:
   - Sign up for a PayPal developer account: [PayPal Developer](https://developer.paypal.com/).
   - Create a new REST API application and get the client ID and secret.

2. Update Django settings:
   - Open the `settings.py` file in the project's main directory.
   - Add the PayPal API credentials in the settings:

   ```python
   PAYPAL_CLIENT_ID = 'your_paypal_client_id'
   PAYPAL_SECRET_KEY = 'your_paypal_secret_key'
   ```

3. Configure the PayPal webhook (optional but recommended):
   - Set up a webhook to handle payment events and updates from PayPal.

## Contributing

If you want to contribute to this project, follow these steps:

1. Fork the repository.
2. Create a new branch for your changes:

```bash
git checkout -b feature/your-feature-name
```

3. Make your modifications and commit changes:

```bash
git commit -m "Add your feature or fix"
```

4. Push the changes to your fork:

```bash
git push origin feature/your-feature-name
```

5. Open a pull request in the original repository, describing your changes in detail.
   

## Acknowledgments

- The project was inspired by the desire to build a scalable and efficient e-commerce platform.
- Thanks to Django and its community for providing a robust backend framework.
- Appreciation to PayPal for their reliable and secure payment gateway integration.

## Contact

For any inquiries or feedback, please contact us at:
- Email: sahilroy2001.sr.com

Happy shopping!
