# Shop Manager Model and Repository Classes

This repository provides a design recipe for creating Model and Repository classes for a database table in the context of a Shop Manager application.

## Table of Contents
- [Introduction](#introduction)
- [Table Design](#table-design)
- [Test SQL Seeds](#test-sql-seeds)
- [Model and Repository Classes](#model-and-repository-classes)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Shop Manager Model and Repository classes are designed to provide an interface for interacting with a database table and managing the shop's items, orders, and order items.

## Project Design
The Project design can be found in the `shop_manager_main_design.md` file. It includes the structure and relationships between the `items`, `orders`, and `order_items` tables. The main schema `shop_manager_schema.sql`

## Test SQL Seeds
To ensure proper testing, it is recommended to have seed data stored in PostgreSQL. If you don't already have seed data, you can use the provided SQL seeds located in the `seeds_shop_manager.sql` file. These seeds populate the `items`, `orders`, and `order_items` tables with sample data.

## Model and Repository Classes
The Model classes represent the entities in the database table, while the Repository classes provide methods for interacting with the database.

The following classes are implemented:
- `Item`: Represents an item in the shop.
- `ItemRepository`: Provides methods for managing items.
- `Order`: Represents an order placed by a customer.
- `OrderRepository`: Provides methods for managing orders.
- `OrderItem`: Represents a relationship between an order and an item.
- `OrderItemRepository`: Provides methods for managing order items.

Please refer to the code files for the implementation details and method signatures.

## Testing
Testing is an important part of ensuring the correctness of the Model and Repository classes. You can find test examples in the `examples.rb` file. These examples demonstrate the usage of the Repository classes and their methods.

To run the tests, make sure you have RSpec installed. Then, execute the following command in your terminal:

```shell
rspec examples.rb
```

To run the tests, make sure you have a PostgreSQL database set up and configured properly. You can reload the SQL seeds before each test run to ensure a consistent state of the database.

## Contributing

Contributions are welcome! If you have any improvements or suggestions, please feel free to submit a pull request.

## License

This project is licensed under the MIT License.
