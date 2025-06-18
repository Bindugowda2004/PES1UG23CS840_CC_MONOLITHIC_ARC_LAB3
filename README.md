# PES1UG23CS840_CC_MONOLITHIC_ARC_LAB3


# CC_Monolith

A simple e-commerce monolithic web application built with Flask, supporting user authentication, product browsing, cart management, and checkout.

## Features

- User registration and login (JWT-based authentication)
- Product listing, viewing, and addition
- Shopping cart (add, remove, clear items)
- Checkout and payment simulation
- Load testing scripts using Locust

## Project Structure

```
auth/           # User authentication logic and database access
cart/           # Cart management logic and database access
checkout/       # Checkout logic
products/       # Product management logic and database access
locust/         # Locust load testing scripts
templates/      # Jinja2 HTML templates
main.py         # Flask application entry point
requirements.txt
```

## Setup

1. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

2. **Run the application:**
   ```sh
   python main.py
   ```

   The app will be available at [http://localhost:5000](http://localhost:5000).

3. **Access the app:**
   - Register a new user or use the test user (`test123` / `test123`).
   - Browse products, add to cart, and checkout.

## Load Testing

Load testing scripts are available in the [`locust/`](locust/) directory.

To run a Locust test (example: browse):
```sh
locust -f locust/browse-locustfile.py
```

## Database

- `auth.db` - User authentication data
- `products.db` - Product catalog
- `carts.db` - Shopping cart data

Databases are created automatically on first run.

## Adding Products

You can add products via the `/product` page in the web UI.

## License

This project is for educational
