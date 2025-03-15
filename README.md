# FarmFlo - Direct Market Access for Farmers

## 🌾 Overview
FarmFlo is a B2C (Business-to-Consumer) marketplace designed to empower farmers by providing direct access to consumers. This platform eliminates middlemen, ensures fair pricing, and reduces commission costs. 

Farmers can list their products, set prices, and manage orders, while consumers can browse available products and make secure purchases. The platform leverages modern web technologies to offer a seamless and efficient marketplace experience.

## 🚀 Features
- **Direct Farmer-to-Consumer Sales:** Farmers can list and sell their products directly to buyers.
- **Transparent Pricing:** Eliminates middlemen and ensures fair pricing.
- **Secure Transactions:** Integrated secure payment system for reliable transactions.
- **Inventory Management:** Farmers can add, edit, and remove product listings.
- **Order Management:** Consumers can track their purchases and order history.
- **User Authentication:** Secure login system for both farmers and buyers.
- **Responsive UI:** Optimized for mobile and desktop devices.
- **Search & Filters:** Users can easily find products based on categories and pricing.
- **Real-Time Notifications:** Instant updates on orders and messages.

## 🛠️ Tech Stack
**Frontend:**
- React.js (Vite) for fast and optimized UI rendering.
- Tailwind CSS for styling and responsiveness.
- Zustand for state management.

**Backend:**
- Node.js & Express.js for API and server-side logic.
- MongoDB for database management.
- Firebase for real-time notifications.

**Other Technologies:**
- Stripe for secure payments.
- Cloudinary for image uploads.
- Postman for API testing.

## 🏗️ Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Node.js (>=16.x.x)
- MongoDB (local or Atlas)
- Git

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/sktigpta/Farm-floo.git
cd Farm-floo
```

### 2️⃣ Install Dependencies
#### Frontend
```bash
cd client
npm install
```

#### Backend
```bash
cd server
npm install
```

### 3️⃣ Set Up Environment Variables
Create a `.env` file in the server directory and add:
```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
STRIPE_SECRET_KEY=your_stripe_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
```

### 4️⃣ Run the Application
#### Start Backend
```bash
cd server
npm run dev
```

#### Start Frontend
```bash
cd client
npm run dev
```

## 📌 API Endpoints
### Authentication
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Authenticate user |

### Products
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET | `/api/products` | Get all products |
| POST | `/api/products` | Add a new product (farmer only) |
| PUT | `/api/products/:id` | Update a product (farmer only) |
| DELETE | `/api/products/:id` | Delete a product (farmer only) |

### Orders
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET | `/api/orders` | Get all orders |
| POST | `/api/orders` | Place a new order |
| GET | `/api/orders/:id` | Get order details |

## 🛡️ Security Measures
- **JWT Authentication**: Ensures secure user sessions.
- **Input Validation**: Prevents SQL injection and data corruption.
- **HTTPS Encryption**: Uses SSL certificates for secure data transmission.
- **Role-Based Access Control**: Restricts access to sensitive features.

## 🤝 Contributing
We welcome contributions! Follow these steps:
1. Fork the repository.
2. Create a new branch (`feature-branch`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a Pull Request.

## 🎯 Future Enhancements
- Implement AI-based pricing suggestions for farmers.
- Introduce a rating and review system for products.
- Add support for multiple payment gateways.
- Build a mobile app version.

## 📄 License
This project is licensed under the MIT License.

## 📬 Contact
For queries or suggestions, reach out:
- Email: sktigpta@gmail.com
- GitHub: [FarmFlo Repo](https://github.com/sktigpta/Farm-floo)

Happy Farming! 🌱
