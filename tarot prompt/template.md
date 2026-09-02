# 📝 MASTER TEMPLATE SINH ẢNH — CHUẨN THE STAR v2 (SONG NGỮ)

> Bản **TIẾNG ANH (EN)** là prompt dùng trực tiếp cho model sinh ảnh (điền vào các biến
> `{TITLE}` `{EMBLEM}` `{SCENE}` `{CHARACTER_SPECIFICATION}` `{COUNT_LOCK}`).
> Bản **TIẾNG VIỆT (VI)** là bản dịch để đọc hiểu và chỉnh sửa — khi sửa ý tưởng, sửa bản VI trước
> rồi cập nhật lại bản EN tương ứng.

---

## 🇬🇧 BẢN TIẾNG ANH (dùng để sinh ảnh)

```text
A single tarot card "{TITLE}" matching the EXACT full-bleed layout, scale, framing and lighting style of the reference card THE STAR: a painterly fine-art oil-painting scene filling the entire canvas edge to edge, framed by a thin double golden line-art border with four ornate golden corner flourishes painted ON TOP of the scene edges.

Inside the scene, in the upper area: {EMBLEM} rendered as a glowing antique-gold motif floating in the sky.
At the lower part of the scene: the hand-lettered title "{TITLE}" in glowing antique-gold lettering, laid directly onto the scene (no banner, no medallion).

Scene content:
{SCENE}. {CHARACTER_SPECIFICATION} {COUNT_LOCK}

Depth layering: paint the scene first covering the whole canvas, then draw the thin double golden line-art border and the four corner flourishes ON TOP of the scene edges — foreground ornament overlapping the background content for a strong sense of depth.

STRICT ANATOMY (HARD RULE): exactly two arms, two legs, one head and one torso per character; every joint (shoulder, elbow, wrist, hip, knee, ankle) must connect naturally to the body — NO extra limbs, NO limbs fused into the ribs, hip, chest or back, NO missing/amputated arms, NO deformed joints, NO wrong finger counts. Keep both arms clearly separated from the torso with visible armpits, elbows and wrists.

Sensual fine-art anatomy, painterly warm oil-painting lighting against subtle shadows, rich atmospheric perspective and depth, symmetrical thin golden frame border, perfectly centered, portrait orientation 7:12 aspect ratio, vintage classical oil-painting fine-art illustration, high detail.
```

---

## 🇻🇳 BẢN TIẾNG VIỆT (bản dịch tham khảo)

```text
Một lá bài tarot "{TITLE}" bám theo ĐÚNG bố cục full-bleed, tỉ lệ, cách đóng khung và phong cách ánh sáng của lá tham chiếu THE STAR: một cảnh hội họa dầu fine-art phủ kín toàn bộ canvas từ mép này sang mép kia, được đóng khung bởi một đường viền vàng mảnh hình đường kép cùng bốn hoa văn góc vàng cầu kỳ được vẽ ĐÈ LÊN TRÊN các mép của cảnh.

Bên trong cảnh, ở vùng phía trên: {EMBLEM} được thể hiện như một biểu tượng vàng cổ phát sáng lơ lửng trên bầu trời.
Ở phần dưới của cảnh: tên lá bài viết tay "{TITLE}" bằng chữ vàng cổ phát sáng, đặt trực tiếp lên cảnh (không banner, không medallion).

Nội dung cảnh:
{SCENE}. {CHARACTER_SPECIFICATION} {COUNT_LOCK}

Hiệu ứng phân lớp chiều sâu: vẽ cảnh trước, phủ kín toàn bộ canvas, sau đó vẽ đường viền vàng mảnh hình đường kép và bốn hoa văn góc ĐÈ LÊN TRÊN các mép của cảnh — đồ trang trí tiền cảnh chồng lên nội dung hậu cảnh để tạo cảm giác chiều sâu mạnh.

GIẢI PHẪU NGHIÊM NGẶT (QUY TẮC CỨNG): mỗi nhân vật có đúng hai tay, hai chân, một đầu và một thân; mọi khớp (vai, khuỷu, cổ tay, hông, gối, cổ chân) phải nối tự nhiên với cơ thể — KHÔNG thừa chi, KHÔNG chi dính vào sườn, hông, ngực hay lưng, KHÔNG tay bị mất/cụt, KHÔNG khớp biến dạng, KHÔNG sai số lượng ngón tay. Giữ hai cánh tay tách rõ khỏi thân với nách, khuỷu và cổ tay nhìn thấy rõ.

Giải phẫu fine-art gợi cảm, ánh sáng ấm kiểu tranh dầu vẽ trên những vùng bóng tinh tế, phối cảnh không khí giàu chiều sâu, khung vàng mảnh đối xứng, căn giữa hoàn hảo, khổ dọc tỉ lệ 7:12, minh họa fine-art tranh dầu cổ điển cổ kính, độ chi tiết cao.
```

---

## 🔑 CHÚ THÍCH BIẾN

| Biến | Nguồn lấy trong `cards.json` | Ghi chú |
|---|---|---|
| `{TITLE}` | `title` (EN) | Chữ in trên lá — giữ tiếng Anh |
| `{EMBLEM}` | `emblem` (EN) / xem `emblem_vi` | Huy hiệu vàng phát sáng trong cảnh |
| `{SCENE}` | `scene` (EN) / xem `scene_vi` | Bối cảnh + hành động chính |
| `{CHARACTER_SPECIFICATION}` | ghép `age` + `hair` + `build` (EN) | Thêm mắt/da/nét riêng từ `02-CHARACTER-SPECS.md` |
| `{COUNT_LOCK}` | `count.layout` (EN) / xem `layout_vi` | `count = null` → dùng khoá "không có vật phẩm bộ bài nào" |
