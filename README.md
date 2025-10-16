# Inventory Management System with .NET and React
A full-stack Inventory Management System built with React.js (frontend), ASP.NET Web API (.NET Framework) as backend, and Microsoft SQL Server as the database. Implements CRUD operations, authentication, and analytics dashboard for efficient stock management.

## Basic structure 
```bash
inventory-management-system-dotnet-react/
│
├── README.md
├── .gitignore
├── backend/                        # ASP.NET Web API project (using .NET Framework)
│   ├── InventoryManagement.API/     # Main API project
│   │   ├── Controllers/
│   │   │   ├── ProductsController.cs
│   │   │   ├── SuppliersController.cs
│   │   │   ├── UsersController.cs
│   │   │   └── AuthController.cs
│   │   ├── Models/
│   │   │   ├── Product.cs
│   │   │   ├── Supplier.cs
│   │   │   ├── User.cs
│   │   │   └── Transaction.cs
│   │   ├── Data/
│   │   │   ├── InventoryContext.cs
│   │   │   └── DbInitializer.cs
│   │   ├── DTOs/
│   │   │   ├── ProductDto.cs
│   │   │   └── AuthDto.cs
│   │   ├── Services/
│   │   │   ├── ProductService.cs
│   │   │   ├── AuthService.cs
│   │   │   └── SupplierService.cs
│   │   ├── Web.config
│   │   ├── Global.asax.cs
│   │   ├── App_Start/
│   │   │   ├── WebApiConfig.cs
│   │   │   └── RouteConfig.cs
│   │   └── InventoryManagement.API.csproj
│   └── InventoryManagement.Tests/   # (Optional) Unit Tests
│
├── frontend/                        # React app
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   ├── ProductTable.jsx
│   │   │   ├── ProductForm.jsx
│   │   │   └── DashboardCards.jsx
│   │   ├── pages/
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Products.jsx
│   │   │   ├── Suppliers.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   ├── services/
│   │   │   ├── api.js               # Axios instance
│   │   │   ├── productService.js
│   │   │   ├── authService.js
│   │   │   └── supplierService.js
│   │   ├── App.js
│   │   ├── index.js
│   │   └── styles/
│   │       └── main.css (or Tailwind setup)
│   ├── package.json
│   ├── .env
│   └── README.md
│
└── docs/                            # Optional: Diagrams, SQL scripts, API docs
    ├── ERD.png
    ├── API_Routes.md
    └── DatabaseSchema.sql
```