# University Library OpenAPI

This repository contains the OpenAPI specification for the **University Library**, an online system for managing library resources in a university environment. The API provides full CRUD operations for handling books, students, and loan transactions.

## 📄 OpenAPI Specification

- **Version:** 3.0.3  
- **File:** `openapi_duzgun.yaml`  
- **Base URLs:**
  - Local: `http://localhost:3000`
  - Production: `https://api.universite-kutuphane.com/v1`

## ✨ Features

- **Books:** Manage library books (list, view, add, update, delete)
- **Students:** Manage student records (list, view, add, update, delete)
- **Loans:** Handle book loan and return processes

## 🔐 Security

The API uses an **API key** for authentication. Include the `X-API-Key` header in your requests.

```
X-API-Key: YOUR_API_KEY
```

## 🚀 Usage

Clone the repository:

```bash
git clone https://github.com/omerkavakli0/university-library-openapi.git
```

Navigate to the project directory:

```bash
cd university-library-openapi
```

Open the OpenAPI specification:

```bash
open openapi_duzgun.yaml
```

Or view it using Swagger Editor or Swagger UI.

## 📚 Documentation

To view and interact with the API documentation, use:

- [Swagger Editor](https://editor.swagger.io)
- Or host it with [Swagger UI](https://swagger.io/tools/swagger-ui/)

---

This specification was created as part of an academic assignment by **Doğukan Özek** (Student No: 171422001).
