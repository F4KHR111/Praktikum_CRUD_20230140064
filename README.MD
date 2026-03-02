# 🚀 User Management API Documentation

**Base URL:** `http://localhost:8080`

---

## 🛠️ Daftar Endpoint (Methods)

### 1. ➕ Tambah User Baru (POST)
**Endpoint:** `/api/users`  
**Fungsi:** Menambahkan data user baru ke database.

**Request Body (JSON):**
```json
{
  "name": "R. Muhammad Fakhri Wirdiyan",
  "age": 20
}
```
Respon Sukses (201 Created):
```json
{
  "status": "success",
  "data": {
    "id": "44f14616-b22e-479f-9f55-b2c56e76c8b3",
    "name": "R. Muhammad Fakhri Wirdiyan",
    "age": 20
  }
}
```

### 2. 👁️ Melihat  User (GET)
**Endpoint:** `/api/users`  
**Fungsi:** Melihat data user baru.

**Respon Sukses (200):*

```json

{
"data": [
{
"age": 20,
"id": "44f14616-b22e-479f-9f55-b2c56e76c8b3",
"name": "R. Muhammad Fakhri Wirdiyan"
}
],
"status": "success"
}
```



### 3. 📝 Edit User  (PUT)
**Endpoint:** `http://localhost:8080/api/users/44f14616-b22e-479f-9f55-b2c56e76c8b3`  
**Fungsi:** Mengedit data user baru.

**Request Body (JSON):*

```json

{
  "name": "Fakhri",
  "age": 21
}
```
Respon Sukses (200):
```json
{
    "data": {
        "age": 21,
        "id": "44f14616-b22e-479f-9f55-b2c56e76c8b3",
        "name": "Fakhri"
    },
    "status": "success"
}
```

### 4. 🗑️ Hapus User  (PUT)
**Endpoint:** `http://localhost:8080/api/users/44f14616-b22e-479f-9f55-b2c56e76c8b3`  
**Fungsi:** Menghapus 1 data users.

**Request Body (JSON):*

```json

{
  "name": "Fakhri",
  "age": 21
}
```
Respon Sukses (200):
```json
{
  "data": "success delete user with id 44f14616-b22e-479f-9f55-b2c56e76c8b3",
  "status": "success"
}
```

![Tampilan WEB.png](../Tampilan%20WEB.png)