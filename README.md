# movingboxes
Keep track of what items are in your moving boxes. 
- Can't find an specific item? Search for it!

# Current version
Current version is 0.1. That means `{api_version}` value is `v0.1`.

# API
## Entities
- Box
- Item
## Operations
### Boxes
- `GET /api/{api_version}/boxes`: Get all boxes for the current user
- `GET /api/{api_version}/boxes/{box_id}`: Get an specific box by its ID
- `POST /api/{api_version}/boxes`: Create a new box
- `PUT /api/{api_version}/boxes/{box_id}`: Update an existing box
- `DELETE /api/{api_version}/boxes/{box_id}`: Delete a box
- `GET /api/{api_version}/boxes/search`: Search for boxes by name or description
- `POST /api/{api_version}/boxes/scan-qr`: Scan a QR code to get information about that box
- `GET /boxes/by-qr-code/{qr_code}`: Get information about the box associated to the QR code
### Items
- `GET /api/{api_version}/boxes/{box_id}/items`: Get all items in a specific box
- `GET /api/{api_version}/boxes/{box_id}/items/{item_id}`: Get a specific item in a box by its ID
- `POST /api/{api_version}/boxes/{box_id}/items`: Add a new item to a box
- `PUT /api/{api_version}/boxes/{box_id}/items/{item_id}`: Update an existing item in a box
- `DELETE /api/{api_version}/boxes/{box_id}/items/{item_id}`: Delete an item from a box
- `GET /api/{api_version}/items/search`: Search for items by name or description
### Additional endpoints
- 
- 
- `GET /api/{api_version}/users/{user_id}/boxes`: Get all boxes for a specific user (for administrators)
- `GET /api/{api_version}/users/{user_id}/items`: Get all items for a specific user (for administrators)
