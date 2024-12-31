# Clearerio_assignment

```
{
conversation:
  "conversation_id": "string",      // ID hội thoại
  "from": {
    "id": "string",                 // ID khách hàng
    "name": "string",               // Tên khách hàng
    "email": "string"               // Email khách hàng
  },
  "message_id": "string",           // ID tin nhắn
  "message": "string",              // Nội dung tin nhắn
  "type": "string",                 // Loại tin nhắn [INBOX, COMMENT, RATING]
  "inserted_at": "datetime",        // Thời gian tạo tin nhắn
  "has_phone": "boolean",           // Có chứa số điện thoại hay không
  "phone_info": ["string"],         // Danh sách số điện thoại (nếu có)
  "is_hidden": "boolean",           // Tin nhắn đã ẩn hay chưa
  "is_removed": "boolean",          // Tin nhắn đã bị xoá hay chưa
  "like_count": "int?",             // Số lượt like (nếu là comment)
  "page_id": "string",              // ID của trang
  "customerID": "long"              // Liên kết đến ID khách hàng (nếu có)
}

```

```
{
Transaction:
  "orderId": "long",            // ID đơn hàng
  "orderDate": "datetime",      // Ngày đặt hàng
  "branchId": "int",            // ID chi nhánh
  "branchName": "string",       // Tên chi nhánh
  "CustomerID": "long",         // ID khách hàng
  "customerName": "string",     // Tên khách hàng
  "totalAmount": "decimal",     // Tổng số tiền đơn hàng
  "status": "int",              // Trạng thái đơn hàng
  "statusValue": "string",      // Giá trị trạng thái đơn hàng (dạng chữ)
  "productId": "long",          // ID sản phẩm
  "productCode": "string",      // Mã sản phẩm
  "productName": "string",      // Tên sản phẩm
  "isMaster": "boolean",        // Hàng chính (true) hay hàng phụ (false)
  "price": "decimal",           // Giá sản phẩm
  "note": "string"              // Ghi chú đơn hàng
}
```

```
{
CustomerDB:
  "CustomerID": "long",          // ID khách hàng
  "CustomerName": "string",      // Tên khách hàng
  "gender": "boolean?",          // Giới tính (true: nam, false: nữ)
  "birthDate": "date?",          // Ngày sinh khách hàng
  "contactNumber": "string",     // Số điện thoại khách hàng
  "Region": "string",            // Khu vực
  "email": "string",             // Email khách hàng
  "organization": "string",      // Công ty
  "taxCode": "string",           // Mã số thuế
  "debt": "decimal",             // Nợ hiện tại
  "retailerId": "int",           // ID cửa hàng
  "modifiedDate": "datetime?",   // Thời gian cập nhật
  "createdDate": "datetime"      // Thời gian tạo
}
```

```
{
  "id": "long",                  // ID hàng hóa
  "code": "string",              // Code hàng hóa
  "barCode": "string",           // Mã vạch hàng hóa
  "retailerId": "int",           // ID cửa hàng
  "name": "string",              // Tên sản phẩm
  "categoryId": "int",           // ID nhóm hàng hóa
  "categoryName": "string",      // Tên nhóm hàng hóa
  "tradeMarkId": "int",          // ID thương hiệu
  "description": "string",       // Mô tả sản phẩm
  "basePrice": "decimal",        // Giá sản phẩm
  "unit": "string",              // Đơn vị tính
  "weight": "double",            // Trọng lượng
  "allowsSale": "boolean?",      // Có được bán trực tiếp không
  "hasVariants": "boolean?",     // Có biến thể không
  "createdDate": "datetime",     // Ngày tạo
  "modifiedDate": "datetime"     // Ngày cập nhật
}
```

