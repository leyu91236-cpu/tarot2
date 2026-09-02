# 🔮 SENSUAL TAROT 78 LÁ — MASTER PROMPT SPECIFICATION

Bản chuẩn hóa quy chuẩn tạo hình và bố cục toàn bộ 78 lá bài Tarot:

1. **Quy chuẩn hiển thị nội dung & khung viền (Visual Anchor Standard — THE STAR)**:
   * Lấy lá **`cards/17-the-star.png`** làm quy chuẩn DUY NHẤT cho toàn bộ bộ bài — chuẩn cho cả **phần ảnh bên trong** lẫn **phần viền bên ngoài**.
   * **Phần viền ngoài**: khung viền vàng MẢNH hình đường kép (double line-art) + 4 hoa văn góc cổ điển, sắc nét, đối xứng hoàn hảo — **đè trực tiếp lên cảnh**, không có dải giấy da riêng.
   * **KHÔNG còn oval medallion ở đỉnh, KHÔNG còn dải ruy băng/banner ở đáy, KHÔNG còn biểu tượng/emblem trên bầu trời** (cập nhật mới): bầu trời/thượng cảnh chỉ là cảnh tự nhiên; **tên lá bài được viết tay trực tiếp lên phần dưới của cảnh** bằng chữ antique-gold phát sáng (trừ The Star giữ sao lớn là motif cảnh vì đó là nội dung lá).
   * **Phần ảnh bên trong**: phong cách hội họa fine-art/oil-painting của The Star — **cảnh full-bleed tràn kín toàn bộ canvas từ mép này sang mép kia**, phối cảnh thoáng đãng, ánh sáng ấm, chiều sâu không gian lùi dần về hậu cảnh, chi tiết sắc nét. Mỗi lá vẫn giữ bối cảnh và bảng màu riêng của mình, chỉ chuẩn hóa về chất lượng nét vẽ, cách đổ sáng và độ chi tiết theo The Star.
   * **Loại bỏ cổng vòm / cột đá phụ chiếm diện tích**: Không dùng cột đá nhân tạo đóng khung gò bó, để không gian khoáng đạt, tự nhiên theo đúng bối cảnh của từng lá bài.

2. **Quy chuẩn tạo hình nhân vật (Sensual Fine-Art Figure Standard)**:
   * Kế thừa phong cách tạo hình sống động, gợi cảm và cổ điển từ tài liệu gốc `01-CARD-TABLE.md` (hình mẫu tiêu biểu như lá **The Empress**: *"a voluptuous nude empress, one breast bared, a crown of flowers in loosened hair, reclining on a velvet throne amid ripe golden wheat and fruits, a heart-shaped shield of Venus leaning beside her"*).
   * **100% Nhân vật nữ** trong độ tuổi thanh xuân từ **18 đến 25 tuổi**.
   * Mỗi lá bài giữ nét đặc trưng độc bản về vóc dáng (*slender, voluptuous, athletic, statuesque*), mái tóc và thần thái.
   * **CHUẨN TRANG PHỤC (WARDROBE STANDARD — HARD RULE)**: mọi nhân vật nữ mặc **giải lụa MỎNG MANH chỉ quấn quanh HÔNG — che phần dưới cơ thể**, **BỘ NGỰC TRẦN** (*bare bust*) theo truyền thống nhân thể fine-art cổ điển (Ingres, Bouguereau, Cabanel); tóc vuốt ra sau vai không che cơ thể; **màu lụa riêng từng lá** (khóa `wardrobe`/`wardrobe_vi` trong `cards.json`); lá hiệp sĩ giữ giáp kèm lụa quấn hông.
   * **CHÂN DUNG NGHỆ THUẬT TÔN VINH CƠ THỂ (FINE-ART FIGURE PORTRAIT — HARD RULE)**: mọi lá phải được dựng như một **bức chân dung nhân thể fine-art tôn vinh vẻ đẹp cơ thể phụ nữ** — bố cục 3/4 đến toàn thân theo truyền thống các bậc thầy nhân thể cổ điển (Ingres, Bouguereau, Cabanel); nhân vật nữ luôn là trái tim thị giác của lá kể cả giữa cảnh vật phức tạp; tư thế yên quý, cử chỉ thanh nhã, da phát sáng tán sắc dưới da, tỉ lệ hài hòa miên man — tôn vinh cơ thể phụ nữ như mỹ thuật thuần túy: duyên dáng, thảnh thơi, tráng lệ, không dung tục.
   * **CẤM CƠ THỂ BỊ DI DẠNG (ANATOMY LOCK — HARD RULE)**: Mỗi nhân vật chỉ được có **tối đa 2 tay, 2 chân, 1 đầu, 1 thân**; mọi khớp (vai, khuỷu, cổ tay, hông, gối, cổ chân) phải nối tự nhiên với thân, **không thừa chi, không chi mọc dính vào sườn/hông/ngực, không tay cụt, không khớp biến dạng, không ngón tay sai số lượng**. Kiểm tra giải phẫu kỹ trước khi chốt ảnh: nếu thấy 3 tay / tay dính thân / chân sai khớp → **vẽ lại**, không chấp nhận bản lỗi. Ưu tiên tư thế 2 tay tách rõ khỏi thân (có nách, khuỷu, cổ tay rõ ràng) để giảm nguy cơ lỗi.

3. **Cấu trúc 3 Lớp Chiều Sâu (3-Layer Depth — chuẩn Star v2)**:
   * **Lớp 1 (Cảnh)**: Phối cảnh hội họa fine-art **full-bleed** phủ kín toàn bộ canvas, ánh sáng ấm áp, chiều sâu không gian lùi dần về hậu cảnh.
   * **Lớp 2 (Tên)**: **KHÔNG có huy hiệu/emblem trên bầu trời**; chỉ còn **tên lá bài viết tay antique-gold phát sáng nằm trực tiếp ở phần dưới của cảnh**, font calligraphy serif đồng nhất toàn series.
   * **Lớp 3 (Khung viền)**: Khung viền vàng mảnh đường kép + 4 hoa văn góc — **ĐÈ LÊN TRÊN mép cảnh** (foreground ornament over background scene) để tạo chiều sâu phân lớp.

---

## Master Prompt Template (Chuẩn The Star v2)

> Prompt tiếng Anh bên dưới là bản dùng sinh ảnh; bản dịch tiếng Việt đầy đủ đặt tại `template.md` (phần 🇻🇳).

```text
A single tarot card "{TITLE}" matching the EXACT full-bleed layout, scale, framing and lighting style of the reference card THE STAR: a painterly fine-art oil-painting scene filling the entire canvas edge to edge, framed by a thin double golden line-art border with four ornate golden corner flourishes painted ON TOP of the scene edges.

NO EMBLEM (HARD RULE): the sky contains ABSOLUTELY NO emblem, symbol or glowing motif — natural sky/scenery only.
At the lower part of the scene: the hand-lettered title "{TITLE}" in glowing antique-gold lettering, laid directly onto the scene (no banner, no medallion).

Scene content:
{SCENE}. {CHARACTER_SPECIFICATION} {COUNT_LOCK}

Depth layering: paint the scene first covering the whole canvas, then draw the thin double golden line-art border and the four corner flourishes ON TOP of the scene edges — foreground ornament overlapping the background content for a strong sense of depth.

Sensual fine-art anatomy, painterly warm oil-painting lighting against subtle shadows, rich atmospheric perspective and depth, symmetrical thin golden frame border (perfectly clean, grain-free, continuous lines — NO noise, NO speckles, NO broken strokes on the frame), maximum micro-detail (eyelashes, iris texture, hair strands, silk weave, skin pores), perfectly centered, portrait orientation 7:12 aspect ratio, vintage classical oil-painting fine-art illustration, 4K UHD, ultra high definition, sharp focus, high detail.
```
