# SimpleShop

SimpleShop is an online shopping platform developed using ASP.NET MVC, C#, SQL, and ADO.NET. This project allows users to buy products, order products online, and register as sellers to sell their products.

## Features

- User Registration and Login
- Product Browsing and Searching
- Add to Cart and Checkout
- Order Processing
- Seller Registration and Product Management
- Order History and Order Tracking

## Technologies Used

- ASP.NET MVC
- C#
- SQL Server
- ADO.NET
- Entity Framework

## Database Design

### Tables

- **Users**: UserID, Username, Password, Email, Role (buyer/seller)
- **Products**: ProductID, Name, Description, Price, Quantity, SellerID
- **Orders**: OrderID, UserID, OrderDate, TotalAmount, OrderStatus
- **OrderDetails**: OrderDetailID, OrderID, ProductID, Quantity, Price
- **Cart**: CartID, UserID, ProductID, Quantity

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/SimpleShop.git
    ```

2. Open the project in Visual Studio.

3. Restore NuGet packages:
    ```sh
    Update-Package -reinstall
    ```

4. Update the database connection string in `web.config`:
    ```xml
    <connectionStrings>
        <add name="SimpleShopDb" connectionString="your_connection_string_here" providerName="System.Data.SqlClient" />
    </connectionStrings>
    ```

5. Update the database schema:
    ```sh
    Update-Database
    ```

6. Build and run the project.

## Usage

### User Registration and Login

- Navigate to the registration page to create an account.
- Login with your credentials.

### Browsing Products

- Browse products on the home page.
- Search for products using the search bar.

### Adding to Cart and Checkout

- Add products to your cart.
- Proceed to checkout, enter shipping details, and place your order.

### Seller Registration and Dashboard

- Register as a seller using the seller registration page.
- Manage your products and view orders from the seller dashboard.

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

If you have any questions or suggestions, feel free to open an issue or contact me at your.email@example.com.
