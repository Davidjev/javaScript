# Shopping Cart App

This is a simple shopping cart app built with vanilla JavaScript. It allows users to browse a list of products, add them to a shopping cart, and view the total price of the cart. Users can also order the products in the cart, which currently only logs the items to the console.

### Getting Started

- Clone this repository to your local machine  
- Open the index.html file in your web browser

### Code Structure

#### Product Class

The Product class is a simple class that creates a product with a title, imageUrl, description, and price.

#### Component Class

The Component class is a base class that provides some basic functionality for rendering elements to the DOM. It contains a createRootElement() method that creates a root element with optional tag, cssClasses, and attributes. It also has a render() method that must be implemented by any child classes.

#### ShoppingCart Class

The ShoppingCart class extends the Component class and manages the items in the shopping cart. It contains a set cartItems() method that updates the items array and the total price of the cart when a new item is added. It also contains a get totalAmount() method that calculates the total price of all items in the cart. The render() method creates the HTML elements for the cart and the orderButton event listener that logs the items in the cart to the console.

#### ProductItem Class

The ProductItem class extends the Component class and renders a single product item. It contains an addToCart() method that adds the product to the shopping cart. The render() method creates the HTML elements for the product item and the addCartButton event listener that adds the product to the cart.

#### ProductList Class

The ProductList class extends the Component class and renders a list of products. It contains a private #products array that is fetched from a backend API. The fetchProducts() method populates the #products array with new Product objects. The renderProducts() method creates a new ProductItem for each product in the #products array. The render() method creates the HTML elements for the product list and calls the renderProducts() method.

#### Shop Class

The Shop class creates new instances of the ShoppingCart and ProductList classes and renders them to the DOM.

#### App Class

The App class initializes the Shop class and provides a static addProductToCart() method that is called when a product is added to the cart.
