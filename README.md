# University Library OpenAPI

This repository contains the OpenAPI specification for the **University Library**, an online system designed as part of the _Açık Kaynak Kodlu Yazılımlar_ course assignment. The API provides CRUD operations for managing books, students, and loan transactions.

## 📄 OpenAPI Specification

- **Version:** 3.0.3  
- **File:** `openapi.yaml`  
- **Base URLs:**
  - Local: `http://localhost:3000`
  - Production: `https://api.universite-kutuphane.com/v1`

## ✨ Features

- **Books:** Create, read, update, and delete books in the library
- **Students:** Manage university student records
- **Loans:** Handle book borrowing and returning transactions

## 🔐 Security

This API uses an API key for authentication. Make sure to include the following header in your requests:

```
X-API-Key: YOUR_API_KEY
```

## 🚀 Usage

To use or test this API:

```bash
git clone https://github.com/dogukanozek/library_openapi.git
cd library_openapi
open openapi.yaml
```

You can load the file in [Swagger Editor](https://editor.swagger.io) for visualization and testing.

## 📚 Documentation

You may use any OpenAPI-compatible tools such as:

- Swagger UI
- Redoc
- Postman (import via YAML)

---

Prepared by **Doğukan Özek**  
Student No: **171422001**  
Course: **Açık Kaynak Kodlu Yazılımlar**