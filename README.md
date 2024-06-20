# Authentication

### **Sign Up - Registration new user**

```http
  POST /register
```

| Parameter  | Type     | Description                             |
| :--------- | :------- | :-------------------------------------- |
| `username` | `string` | **Required**. username of user to fetch |
| `password` | `string` | **Required**. valid password            |

Response :

```json
{
  "message": "User registered successfully"
}
```

### **Sign In - Login**

```http
  POST /login
```

| Parameter  | Type     | Description                             |
| :--------- | :------- | :-------------------------------------- |
| `username` | `string` | **Required**. username of user to fetch |
| `password` | `string` | **Required**. valid password            |

Response :

```json
{
  "message": "User Success login successful"
}
```

# Fruit

### **Predict your image**

```http
  POST /predict
```

Header :

- **Content-Type:** application/json
- **Authorization:** Token

| Parameter | Type   | Description                                 |
| :-------- | :----- | :------------------------------------------ |
| `image`   | `file` | **Required**. the image you want to predict |

Response :

```json
{
  "predicted": "fresh_strawberry",
  "message": "Image has already been predicted",
  "timestamp": "Jun 12, 2024, 12:33:18.700 PM"
}
```

### **Get last history of predict**

```http
  GET /history
```

Header :

- **Content-Type:** application/json
- **Authorization:** Token

| Parameter | Type | Description |
| :-------- | :--- | :---------- |
|           |      |             |

Response :

```json
{
  "predicted": "fresh_strawberry",
  "timestamp": "Jun 12, 2024, 12:33:18.700 PM"
}
```
