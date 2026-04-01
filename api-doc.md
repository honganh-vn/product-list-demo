# 🛍️ Product API Documentation

Base URL:  
https://my-json-server.typicode.com/honganh-vn/product-list-demo

---

# 📦 1. Product Model

### Description
Cấu trúc dữ liệu của một sản phẩm.

---

### JSON Example

```json
{
  "id": 1,
  "name": "iPhone 14 Pro Max",
  "price": 29990000,
  "image": "https://example.com/image.jpg",
  "description": "Flagship Apple smartphone",
  "category": "phone",
  "stock": 10
}

| Field       | Type   | Required | Description      |
| ----------- | ------ | -------- | ---------------- |
| id          | number | Yes      | ID sản phẩm      |
| name        | string | Yes      | Tên sản phẩm     |
| price       | number | Yes      | Giá (VND)        |
| image       | string | Yes      | URL ảnh          |
| description | string | No       | Mô tả sản phẩm   |
| category    | string | Yes      | Danh mục         |
| stock       | number | Yes      | Số lượng tồn kho |


📋 2. Get Product List (Pagination)

GET /products

Description

Lấy danh sách sản phẩm, hỗ trợ phân trang theo chuẩn JSON Server.

| Param  | Type   | Required | Description                   |
| ------ | ------ | -------- | ----------------------------- |
| _page  | number | No       | Trang hiện tại (bắt đầu từ 1) |
| _limit | number | No       | Số lượng sản phẩm mỗi trang   |
