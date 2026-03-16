#  CartWave - Ride the Shopping Wave

> **Shop Smarter with AI-Powered Search**

CartWave is a modern, intelligent e-commerce platform that revolutionizes online shopping with natural language AI search. Find products the way you think - just describe what you want!

![CartWave](https://img.shields.io/badge/CartWave-v1.0.0-blue?style=for-the-badge)
![React](https://img.shields.io/badge/React-18.2.0-61DAFB?style=for-the-badge&logo=react)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-Connected-47A248?style=for-the-badge&logo=mongodb)

---

##  **What is CartWave?**

CartWave is your intelligent shopping companion that understands natural language. No more complex filters or endless scrolling - just type what you're looking for in plain English, and our AI finds it instantly!

### ** Key Features**

-  **AI-Powered Search**: Use natural language to find products
-  **Beautiful Modern UI**: Gradient designs with smooth animations
-  **Lightning Fast**: Instant search results
-  **Secure Authentication**: User login/logout with session management
-  **Fully Responsive**: Perfect on desktop, tablet, and mobile
-  **Smart Cart**: Redux-powered shopping cart
-  **Easy Checkout**: Streamlined purchase process

---

##  **Quick Start**

### **Prerequisites**
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### **Installation**

```bash
# Clone the repository
git clone https://github.com/yourusername/cartwave.git

# Navigate to project directory
cd cartwave

# Install dependencies
npm install --legacy-peer-deps

# Set up environment variables
cp api/config/config.env.example api/config/config.env
# Edit config.env and add your MongoDB URI

# Start both frontend and backend
npm run dev
```

### **Access CartWave**
-  **Frontend**: http://localhost:3000
-  **Backend API**: http://localhost:4001

---

##  **Features Showcase**

### **1. AI-Powered Smart Search** 
```
"Show me running shoes under $100 with good reviews"
"Find laptops for gaming under $1500"
"Accessories under $50"
```
CartWave understands and finds exactly what you need!

### **2. Beautiful Modern Design** 
- **Gradient Navbar**: Purple-blue gradient with smooth animations
- **Hero Section**: Eye-catching banner with call-to-action
- **Product Cards**: Hover effects, shadows, and smooth transitions
- **AI Search Card**: Stunning gradient card with professional design
- **Professional Footer**: Complete with social links and contact info

### **3. User Authentication** 
- Secure login and registration
- Session management with JWT
- User greeting in navbar
- Logout functionality

### **4. Smart Shopping Cart** 
- Add/remove products
- Real-time cart updates
- Redux state management
- Persistent cart data

---

##  **Technology Stack**

### **Frontend**
-  React 18.2.0
-  Bootstrap 5 + Custom CSS
-  Redux Toolkit
-  React Router v6
-  React Hot Toast
-  React Loading Skeleton

### **Backend**
-  Node.js + Express
-  MongoDB with Mongoose
-  JWT Authentication
-  Cookie Parser
-  Concurrently for dev

### **AI/ML**
-  Natural Language Processing
-  Smart Query Parsing
-  Relevance Scoring
-  Intelligent Filtering

---

##  **Project Structure**

```
cartwave/
├── api/
│   ├── controllers/
│   │   ├── productController.js    # AI search logic
│   │   ├── userController.js       # Authentication
│   │   └── orderController.js      # Order management
│   ├── models/
│   │   ├── Product.js
│   │   ├── User.js
│   │   └── Order.js
│   ├── routes/
│   │   ├── productRoute.js
│   │   ├── userRoute.js
│   │   └── orderRoute.js
│   ├── data/
│   │   └── products.json           # Product catalog
│   └── server.js                   # Main server
├── src/
│   ├── components/
│   │   ├── Navbar.jsx              # CartWave navbar
│   │   ├── Footer.jsx              # Professional footer
│   │   ├── Products.jsx            # AI search UI
│   │   └── main.jsx                # Hero section
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── Products.jsx
│   │   ├── Login.jsx
│   │   ├── Register.jsx
│   │   └── Cart.jsx
│   ├── redux/
│   │   ├── store.js
│   │   └── reducer/
│   │       └── handleCart.js
│   ├── App.css                     # Custom styling
│   └── index.js
└── package.json
```

---

##  **API Endpoints**

### **Products**
- `GET /api/v1/local-products` - Get all products
- `POST /api/v1/ai-search` - AI-powered search
- `GET /api/v1/product/:id` - Get single product

### **Authentication**
- `POST /api/v1/simple-register` - Register user
- `POST /api/v1/simple-login` - Login user
- `GET /api/v1/logout` - Logout user

### **Orders**
- `POST /api/v1/order/new` - Create order
- `GET /api/v1/orders/me` - Get user orders

---

##  **Testing AI Search**

### **Example Queries**

```bash
# Price-based search
curl -X POST http://localhost:4001/api/v1/ai-search \
  -H "Content-Type: application/json" \
  -d '{"query": "shoes under $100"}'

# Category + Price
curl -X POST http://localhost:4001/api/v1/ai-search \
  -H "Content-Type: application/json" \
  -d '{"query": "laptops under $1500"}'

# Rating-based
curl -X POST http://localhost:4001/api/v1/ai-search \
  -H "Content-Type: application/json" \
  -d '{"query": "products with good reviews"}'
```

---

##  **Design Highlights**

### **Color Palette**
```css
Primary Gradient:   #667eea → #764ba2 (Purple-Blue)
Success Gradient:   #4facfe → #00f2fe (Cyan)
Accent Gradient:    #f093fb → #f5576c (Pink)
Dark Gradient:      #2c3e50 → #34495e (Professional Dark)
```

### **Typography**
- **Font Family**: Poppins (Google Fonts)
- **Clean & Modern**: Professional look

### **Animations**
-  Fade-in effects
-  Hover transformations
-  Smooth transitions
-  Card elevations

---

##  **What Makes CartWave Special?**

1. **Natural Language AI** - No complex filters needed
2. **Beautiful Design** - Modern gradient UI with smooth animations
3. **User-Friendly** - Intuitive interface for everyone
4. **Fast Performance** - Instant search results
5. **Secure** - JWT authentication and secure sessions
6. **Responsive** - Perfect on all devices
7. **Maintainable** - Clean, well-structured code

---

##  **Future Enhancements**

-  OpenAI GPT-4 integration for advanced NLP
-  Product recommendations based on browsing history
-  Voice search capability
-  Image-based product search
-  Multi-language support
-  Advanced filters (brand, size, color)
-  Wishlist functionality
-  Product comparison tool
-  Payment gateway integration (Stripe/PayPal)
-  Admin dashboard

---

##  **About**

CartWave is built with ❤️by me who believe shopping should be simple, fast, and enjoyable.

** Ride the Shopping Wave!**
