# Prompt Log - Trang Agent Valorant

## 1. Tạo trang Agent
**Prompt:** Tạo trang web giới thiệu 29 Agent Valorant (Season 26 Act V) gồm 4 vai trò: Duelist, Initiator, Controller, Sentinel (bao gồm Miks và Veto). Dùng thuần HTML + CSS, radio input + `:checked` selector thay JS, layout 3 cột (abilities | portrait | info), hiệu ứng floating, scanlines, glassmorphism, neon glow theo vai trò. CSS riêng tại `Css/agent.css`.

**Kết quả:** Tạo `Page/Agent.html` và `Css/agent.css`. 29 agent đầy đủ, chọn agent bằng CSS `:checked ~` selector, layout 3 cột HUD, floating animation, aura, scanlines, màu theo vai trò (đỏ/vàng/tím/xanh).

---

## 2. Mở rộng layout cho vừa màn hình
**Prompt:** Make it more fit into the site, there are plenty of space.

**Kết quả:** Sửa `agent.css` — bỏ `max-width: 1400px`, tăng cột giữa `320px → 420px`, `align-items: stretch` để 3 panel cao bằng nhau, portrait `min-height 420px → 520px`, ảnh `max-width 280px → 380px`, tên agent `3rem → 3.5rem`, thêm breakpoint `1100px`.

---

## 3. Thay emoji role bằng ảnh logo
**Prompt:** Change the agent logo from image to replace current emoji, also make it responsive for mobile.

**Kết quả:** Thay emoji ⚔ 🔍 🌀 🛡 trong `.role-tab` và `.role-badge` bằng `<img>` từ Valorant API (`media.valorant-api.com/roles/...`). CSS dùng `inline-flex + align-items: center`, icon `1em x 1em`, `filter: brightness(0) invert(1)`.

---

## 4. Giới hạn logo role ngang bằng chữ
**Prompt:** Giới hạn lại logo role cho ngang bằng chữ.

**Kết quả:** Sửa `agent.css` — `.role-tab` và `.role-badge` dùng `inline-flex`, `img` set `width: 1em; height: 1em` để icon tự khớp với `font-size`, `object-fit: contain` chống méo.

---

## 5. Tăng kích thước icon role
**Prompt:** Cho cái img bự lên tí nữa.

**Kết quả:** Tăng `width/height` của `img` trong `.role-tab` và `.role-badge` từ `1em → 1.4em`.
