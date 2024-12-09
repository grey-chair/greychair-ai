# **Grey Chair: Property Management Platform**

## **Overview**
Grey Chair is a next-generation property management platform that streamlines property operations, tenant communications, and financial planning. It is designed to serve multiple user roles, including **property managers**, **tenants**, **contractors**, **owners**, **HOAs**, and **prospective tenants**. Built on Firebase for real-time data management, Grey Chair offers transparency, efficiency, and actionable insights to all stakeholders.

### **Positioning Statement**
Grey Chair stands out by combining **property health scoring**, **tenant scoring**, and **reserve fund planning** into one seamless platform. By empowering property managers with tools for proactive decision-making and providing tenants with transparency and convenience, Grey Chair bridges the gap between property management and modern user expectations.

---

## **Core Features**
1. **User Authentication and Role Management**:
   - Secure login with Firebase Authentication.
   - Role-based access for tenants, property managers, contractors, owners, and prospective tenants.
2. **Tenant Dashboard**:
   - View leases, payments, maintenance requests, and notifications.
3. **Maintenance Workflow**:
   - Submit and track maintenance requests.
   - Assign contractors and update task statuses.
4. **Property Management**:
   - Manage properties, units, and tenant assignments.
5. **Financial Health Monitoring**:
   - Reserve fund tracking and automated financial insights.
6. **Notifications System**:
   - Real-time alerts for tenants, property managers, and contractors.
7. **Prospective Tenant Portal**:
   - Explore available properties, schedule tours, and submit applications.
8. **Appliance Tracking**:
   - Monitor appliance health and schedule maintenance.

---

## **Tech Stack**
### **Frontend**:
- **React.js**: Dynamic and responsive UI framework.
- **Firebase SDK**: Integrated with Authentication, Firestore, and Storage.

### **Backend**:
- **Node.js with Express.js**: Lightweight and scalable backend framework.
- **Firebase Admin SDK**: Server-side operations for authentication and Firestore.

### **Database**:
- **Firestore (NoSQL)**: Scalable, real-time database.

### **Other Services**:
- **Firebase Storage**: For file uploads like lease agreements and profile photos.
- **Stripe/PayPal**: For payment processing (future integration).

---

## **Developer Setup**

### **Prerequisites**
- **Node.js**: Version 16 or above.
- **Firebase Account**: Access to Firebase Console for project setup.
- **Git**: Version control system.

### **Project Setup**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/grey-chair.git
   cd grey-chair
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up Firebase**:
   - Create a Firebase project in the [Firebase Console](https://console.firebase.google.com/).
   - Enable **Authentication** (email/password), **Firestore**, and **Storage**.
   - Generate Firebase configuration keys.

4. **Configure environment variables**:
   - Create a `.env` file in the project root:
     ```plaintext
     FIREBASE_API_KEY=your_api_key
     FIREBASE_AUTH_DOMAIN=your_project_id.firebaseapp.com
     FIREBASE_PROJECT_ID=your_project_id
     FIREBASE_STORAGE_BUCKET=your_project_id.appspot.com
     FIREBASE_MESSAGING_SENDER_ID=your_sender_id
     FIREBASE_APP_ID=your_app_id
     ```
   - Replace `your_*` placeholders with your Firebase credentials.

5. **Start the development server**:
   ```bash
   npm start
   ```

---

## **Project Structure**
```plaintext
grey-chair/
├── public/               # Static assets (HTML, images, etc.)
├── src/
│   ├── components/       # Reusable React components
│   ├── context/          # Context API providers (e.g., AuthContext)
│   ├── firebase/         # Firebase configuration and service logic
│   ├── pages/            # Page-level React components
│   ├── services/         # Backend API and Firestore interaction
│   ├── styles/           # Global and modular CSS styles
│   ├── utils/            # Utility functions (e.g., formatters)
│   └── App.js            # Root React component
├── .env                  # Environment variables for Firebase configuration
├── package.json          # Project metadata and dependencies
└── README.md             # Project documentation
```

---

## **Key Development Areas**

### **1. Prospective Tenant Workflow**
1. **Explore Available Properties**:
   - Public-facing property listing page.
   - Filters for location, price range, and unit type.
2. **Schedule Tours**:
   - Calendar integration for property managers to manage tour requests.
   - Prospective tenants can request specific time slots.
3. **Submit Rental Applications**:
   - Application form for prospective tenants.
   - Integration with Firestore to store application details.
   - Notifications for property managers when applications are received.

---

### **2. Tenant Workflow**
1. **Dashboard**:
   - View profile, lease details, maintenance requests, and payment history.
2. **Submit Maintenance Requests**:
   - Simple form to report issues with optional photo upload.
3. **View Notifications**:
   - Rent reminders, maintenance updates, and property news.

---

### **3. Property Management Workflow**
1. **Manage Properties**:
   - CRUD operations for properties and units.
   - Assign tenants to units.
2. **View Lease Agreements**:
   - Access lease details and manage renewals.
3. **Handle Maintenance Requests**:
   - Assign contractors and track task progress.

---

### **4. Notifications System**
1. **For Tenants**:
   - Rent reminders and maintenance updates.
2. **For Prospective Tenants**:
   - Tour confirmations and application status updates.
3. **For Property Managers**:
   - Overdue rent notifications and maintenance escalations.

---

## **Testing**
- **Unit Tests**:
  - Test all backend APIs (e.g., registration, login, role validation).
- **Integration Tests**:
  - Test data flow between frontend and backend.
- **Frontend Tests**:
  - Use Jest/React Testing Library for UI testing.

---

## **Roadmap**
### **Phase 1: MVP Development**
- Firebase setup (Authentication, Firestore, and Storage).
- Core workflows for tenants and property managers.
- Public property listings for prospective tenants.

### **Phase 2: Feature Expansion**
- Advanced notification system.
- Contractor assignment and appliance tracking.
- Tenant scoring and property health metrics.

### **Phase 3: Advanced Features**
- Reserve fund planning.
- AI-driven insights for property performance.
- Integration with third-party tools (e.g., Zillow, QuickBooks).

---

## **Contact**
- **Team**: Grey Chair Development Team
- **Support Email**: support@greychair.com
- **GitHub**: [Grey Chair Repository](https://github.com/grey-chair/greychair-ai)
