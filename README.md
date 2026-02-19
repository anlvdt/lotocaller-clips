# Kho Câu Rao Video - Kêu Lô Tô

Kho chia sẻ bộ clip câu rao video cho ứng dụng [Kêu Lô Tô](https://keuloto.netlify.app).

## Cách dùng

1. Mở ứng dụng Kêu Lô Tô
2. Bấm tab **Chia Sẻ** trên thanh điều hướng
3. Chọn bộ clip → Bấm **Tải về**
4. Clip sẽ tự động thêm vào kho của bạn

## Cách đóng góp

1. **Tạo bộ clip** trong ứng dụng (tab Câu Rao Video → Quét hoặc thêm thủ công)
2. **Xuất JSON** (nút Xuất trong sidebar)
3. **Fork repo** này
4. Thêm file JSON vào thư mục `packs/`
5. Cập nhật `index.json` với thông tin bộ clip
6. **Tạo Pull Request**

## Định dạng file

### `index.json`
```json
{
  "packs": [
    {
      "id": "ten-bo-clip",
      "name": "Tên Bộ Clip",
      "author": "Tên bạn",
      "description": "Mô tả ngắn",
      "clipCount": 30,
      "file": "packs/ten-bo-clip.json",
      "tags": ["tag1", "tag2"],
      "updated": "2026-02-19"
    }
  ]
}
```

### File pack (`packs/*.json`)
```json
{
  "name": "Tên Bộ Clip",
  "author": "Tên bạn",
  "clips": {
    "1": [{"videoId": "xxx", "start": 5.0, "end": 12.0, "label": "...", "source": "..."}],
    "2": [{"videoId": "xxx", "start": 15.0, "end": 22.0, "label": "...", "source": "..."}]
  }
}
```

## Lưu ý

- Chỉ chia sẻ clip từ video **công khai** trên YouTube
- Không chia sẻ nội dung vi phạm bản quyền hoặc pháp luật
- Mỗi clip chỉ chứa **tham chiếu** (videoId + thời gian), không chứa nội dung video
