# rn-assignment6-11038463
 
Project Overview
This project is a React Native application designed to simulate a basic e-commerce shopping cart experience. Users can browse products, add items to their cart, and manage their cart items. The cart's state is saved locally on the device using AsyncStorage to ensure persistence across sessions.

Features
Product Listing Screen: Displays available products with an option to add them to the cart.
Cart Screen: Lists items added to the cart with options to remove them.
Add to Cart Functionality: Allows users to add products to the cart from the product listing screen.
Remove from Cart Functionality: Allows users to remove items from the cart screen.
Local Storage: Uses AsyncStorage to store the cart items locally on the device.

Design and Functionality
UI Design
The application’s design aims to be clean and user-friendly:
Product Listing Screen: Each product is displayed with its image, name, price, and an "Add to Cart" button.
Cart Screen: Displays items added to the cart, each with a "Remove" button and a summary section showing the total price.
Navigation: Intuitive navigation between the product listing and cart screens using header buttons.

Data Storage
AsyncStorage: Selected for its simplicity and effectiveness in storing JSON data locally. It allows the cart's state to persist between app sessions.

Component Breakdown
HomeScreen.js:
Displays the list of products.
Uses ProductItem components for rendering each product.
Handles adding items to the cart and updating AsyncStorage.

CartScreen.js:
Retrieves and displays cart items from AsyncStorage.
Uses CartItem components for rendering each cart item.
Handles removing items from the cart and updating AsyncStorage.

ProductItem.js:
A reusable component for displaying individual products on the HomeScreen.
Includes the product image, name, price, and an "Add to Cart" button.

CartItem.js:
A reusable component for displaying individual cart items on the CartScreen.
Includes the product name, price, and a "Remove" button.

State Management
Utilizes React's useState and useEffect hooks for managing state.
Cart items are managed locally within components and are synced with AsyncStorage for persistence.

Local Storage with AsyncStorage
AsyncStorage:
Stores cart items as JSON strings.
Provides methods to get, set, and remove items from the storage.
Ensures cart data is preserved between app sessions.
Implementation Details

Key Components
HomeScreen.js:
Displays products in a scrollable list.
Uses ProductItem for each product.
Handles adding products to the cart and storing them in AsyncStorage.

CartScreen.js:
Displays cart items retrieved from AsyncStorage.
Uses CartItem for each item in the cart.
Handles removing items from the cart and updating AsyncStorage.

ProductItem.js:
Renders individual product details and includes an "Add to Cart" button.
CartItem.js:
Renders individual cart item details and includes a "Remove" button.

Conclusion
This React Native e-commerce app provides a simple and intuitive shopping cart experience. The use of AsyncStorage ensures that cart data is persisted across sessions, offering a seamless user experience. The modular component design allows for easy scalability and maintenance.

Screenshots
HomeScreen: Displaying the list of products.
![screenshot2](<myapp/assets/screenshot2.png>)
![screenshot3](<myapp/assets/screenshot3.png>)

CartScreen: Displaying selected items in the cart.
![screenshot1](<myapp/assets/screenshot1.png>)