# Inventory Management System

This project is a simple Inventory Management System built using Django and Django Rest Framework. It supports CRUD operations on inventory items with caching support and JWT authentication.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- Python installed on your system.
- `pipenv` for managing dependencies.

### Installation

1. **Install Pipenv**  
   If `pipenv` is not already installed, install it using the following command:
   ```bash
   pip install pipenv

2.Install Project Dependencies
pipenv install

3.Start the Development Server
runserver.bat



The development server should now be running at http://127.0.0.1:8000/.

API Endpoints
1. List All Items
URL: http://127.0.0.1:8000/api/items/
Method: GET
Description: Retrieve a list of all items in the inventory.
2. Retrieve a Specific Item
URL: http://127.0.0.1:8000/api/items/<id>/
Method: GET
Description: Retrieve the details of a specific item by its ID.
Example: http://127.0.0.1:8000/api/items/1/
3. Update an Item
URL: http://127.0.0.1:8000/api/items/<id>/
Method: PUT
Description: Update the details of an existing item by its ID. The data should be sent in JSON format.
Example: http://127.0.0.1:8000/api/items/1/
Request Body Example:
{
    "name": "Updated Item",
    "description": "Updated description.",
    "quantity": 30,
    "price": 15.99
}
4. Delete an Item
URL: http://127.0.0.1:8000/api/items/<id>/
Method: DELETE
Description: Delete an item from the inventory by its ID.
Example: http://127.0.0.1:8000/api/items/1/
5. Create Single or Multiple Items
URL: http://127.0.0.1:8000/api/items/
Method: POST
Description: Add one or more items to the inventory. The data should be in the following format:

{
    "post_data": [     
        {
            "name": "Item 6",
            "description": "This is the sixth item.",
            "quantity": 20,
            "price": 9.99
        },
        {
            "name": "Item 7",
            "description": "This is the sixth item.",
            "quantity": 20,
            "price": 9.99
        },{
            "name": "Item 8",
            "description": "This is the sixth item.",
            "quantity": 20,
            "price": 9.99
        }
    ]
}
