# Backend

Phần xử lý phía sau của [Coffee App](./coffee-app.md).

## Kiến trúc

### API
Nhận request từ app, trả dữ liệu JSON.

### Database
Lưu đơn hàng và thông tin món.

## Luồng xử lý

### Tạo đơn
API nhận đơn, ghi vào Database.

### Cập nhật trạng thái
Quán đổi trạng thái, API đẩy về cho khách.

```python
def create_order(items):
    ## dòng này nằm trong code block, sẽ bị bỏ qua
    return db.save(items)
```

## Tham khảo
- Xem thêm [[coffee-app]]
