### docker-compose - v2ray(Vmess + TLS + WebSocket)

---

1. Sau khi sao chép dự án này vào máy chủ:

- `cd docker-vray` và thực hiện lệnh `bash start-v2ray.sh`

Để sử dụng đường dẫn khác, vui lòng sửa đổi chuỗi `/HelloWorld` trong `data/nginx/conf.d/v2ray.conf` trước khi chạy tập lệnh `start-v2ray.sh` <b>trước</b>

Nếu Docker hoặc docker-compose chưa được cài đặt, vui lòng thực hiện lệnh `bash install-docker.sh` <b>trước khi</b> chạy tập lệnh `start-v2ray.sh`

Nếu tính năng tăng tốc TCP không được bật, vui lòng thực hiện lệnh `bash install-bbr.sh` <b>sau khi</b> chạy tập lệnh `start-v2ray.sh` (máy chủ có thể tự động khởi động lại)

2. Cài đặt `docker-compose`

```
curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

```
chmod +x /usr/local/bin/docker-compose
```

```
ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```
