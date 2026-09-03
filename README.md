# 🌹 tarot2 — Sensual Tarot 78 Lá (Bộ Dữ Liệu Prompt Sinh Ảnh)

Dự án chuẩn hóa việc tạo hình **bộ bài Tarot 78 lá** phong cách **fine-art / tranh dầu cổ điển gợi cảm**
(chuẩn thị giác lấy từ lá **THE STAR** — `cards/17-the-star.png`).

## Cấu trúc

```
tarot2/
├── README.md                    ← file này
├── cards/                       ← ảnh PNG các lá (784×1360, tỉ lệ ~7:12)
│   ├── card-blank.png           ← phôi nền (giấy da + viền góc vàng)
│   ├── 00-fool.png ...          ← các lá đã tạo, đặt tên theo "slug"
│   └── 17-the-star.png          ← ⭐ lá CHUẨN PHONG CÁCH (style anchor)
└── tarot prompt/
    ├── 00-MASTER-PROMPT.md      ← quy chuẩn tổng + master prompt (khung, huy hiệu, anatomy lock)
    ├── 01-CARD-TABLE.md         ← bảng thông số 72 nhân vật nữ (biên tập "quyến rũ")
    ├── 02-CHARACTER-SPECS.md    ← bảng thông số 72 nhân vật nữ (biên tập "gợi cảm" — mới nhất)
    ├── cards.json               ← ⭐ DỮ LIỆU CHÍNH: 78 lá, song ngữ Anh/Việt
    └── template.md              ← master template sinh ảnh, song ngữ (EN để sinh ảnh / VI để đọc)
```

## Nguyên tắc song ngữ

| Nội dung | Tiếng Anh (EN) | Tiếng Việt (VI) |
|---|---|---|
| `cards.json` | khóa gốc: `scene`, `hair`, `build`, `emblem`, `count.layout`... | khóa hậu tố `_vi`: `scene_vi`, `hair_vi`... |
| `template.md` | code block 🇬🇧 | code block 🇻🇳 |
| Bảng 01/02 | chuỗi EN trong cột tóc/mắt = dữ liệu prompt | cột mô tả Việt sẵn có |

- **EN là bản dùng sinh ảnh** (model ảnh hiểu tiếng Anh tốt hơn); **VI là bản để đọc/chỉnh sửa**. Sửa ý tưởng ở bản VI trước, rồi đồng bộ lại bản EN.
- **`title` giữ tiếng Anh** vì là chữ IN LÊN lá bài (VD: "THE FOOL"); `title_vi` chỉ là ghi chú tên Việt tham khảo.

## Quy tắc cứng khi sinh ảnh (HARD RULES)

1. **Style anchor**: mọi lá phải khớp khung & ánh sáng của `cards/17-the-star.png` (full-bleed, viền vàng
   mảnh đường kép + 4 hoa văn góc, **KHÔNG biểu tượng/emblem trên bầu trời**, tên lá chữ vàng viết tay
   ở đáy cảnh font đồng nhất — **không** medallion, **không** banner).
2. **Anatomy Lock**: mỗi nhân vật tối đa 2 tay, 2 chân, 1 đầu, 1 thân; khớp nối tự nhiên; không thừa/khuyết chi.
3. **Count Lock**: `count.n` trong `cards.json` là ràng buộc CỨNG về số lượng vật phẩm bộ bài
   (gậy/cốc/kiếm/xu); `count = null` nghĩa là không có vật phẩm bộ bài nào.
4. **Nhân vật (GLOBAL — SCENE THE STAR)**: mọi nhân vật nữ dùng đúng chuẩn mô tả scene của **The Star**
   (`17-the-star.png`): *"một người phụ nữ đứng ngang eo trong hồ nước trong vào ban đêm, cơ thể cong ngửa và
   xoay ba phần tư về phía người xem, tóc ướt đổ dọc sống lưng, cả hai tay giơ lên đổ nước từ hai cái vò, một
   gối nhấc lên"*; cô ấy 20 tuổi, thon mảnh, eo nhỏ, chân dài, da sáng, tóc vàng nhạt lấp lánh rất dài và ướt.
   **Thay thế toàn bộ** thông số nhân vật/tư thế riêng của từng lá. KHÔNG sao chép sao/biểu tượng trên trời.
5. **Chất lượng (Clean Frame + Micro-Detail)**: khung viền vàng phải sạch tuyệt đối (không noise/đốm/nét đứt);
   chi tiết vi mô tối đa (lông mi, mống mắt, sợi tóc, kết cấu vải nếu có, lỗ chân lông, cạnh trang sức);
   phong cách kết xuất **4K UHD / ultra-detail / sharp focus** — quy định tại `template.md` (CLEAN FRAME + MAXIMUM MICRO-DETAIL).
6. **Không mô tả trang phục lụa (HARD RULE)**: prompt sinh ảnh **KHÔNG nhắc** tới lụa quấn hông / lụa xuyên
   thấu / lụa drape (`silk drape`, `sheer drape`, `lụa quấn hông`, `lụa xuyên thấu`); không còn khóa
   `wardrobe`/`wardrobe_vi` trong `cards.json`. Tư thế/ánh sáng (và nếp vải nếu thuộc bối cảnh riêng) tạo
   gợi cảm fine-art tinh tế, duyên dáng, không dung tục.
7. **Chân dung nghệ thuật tôn vinh cơ thể phụ nữ (Fine-Art Figure Portrait)**: mỗi lá là một **bức
   chân dung nhân thể fine-art** — nhân vật nữ luôn là **trái tim thị giác** của lá bài (bố cục
   chân dung 3/4 đến toàn thân), theo truyền thống các bậc thầy nhân thể cổ điển
   (Ingres, Bouguereau, Cabanel); tư thế yên quý thanh nhã, da phát sáng tán sắc dưới da,
   tỉ lệ hài hòa — tôn vinh vẻ đẹp cơ thể phụ nữ như mỹ thuật thuần túy (không dung tục).
