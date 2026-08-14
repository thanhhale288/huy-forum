# Tổng kết chương trình Cyber Clinic — 7 buổi × 3 giờ

Tài liệu tổng hợp toàn bộ slide/sổ tay trong thư mục này. Mỗi buổi tương đương **1 buổi học 3 tiếng**; nội dung được **cân bằng độ sâu** giữa các buổi (không phình theo số trang slide gốc: Buổi 1/6/7 chi tiết, Buổi 2–5 dạng sổ tay tóm tắt).

**Sợi chỉ đỏ cả khóa:** An toàn thông tin không phải việc của riêng IT — là trách nhiệm toàn tổ chức; bảo vệ theo vòng đời liên tục (Govern → Identify → Protect → Detect → Respond → Recover).

---

## Bản đồ khóa học (nhịp 3 giờ)

| Buổi | Chủ đề | Trọng tâm vận hành | Gợi ý phân bổ 3h |
|------|--------|--------------------|------------------|
| 1 | Xu hướng & khung pháp lý ATTT cho MSME | Vì sao phải làm + nghĩa vụ pháp lý | 45′ bối cảnh · 75′ pháp lý · 45′ thảo luận/case · 15′ chốt |
| 2 | Tài sản số + Danh tính & truy cập | Có gì cần bảo vệ + ai được vào | 20′ mở · 70′ tài sản/NIST · 70′ MFA/IAM · 20′ chốt |
| 3 | Kỹ nghệ xã hội, BEC, mã độc | Con người bị thao túng thế nào | 20′ mở · 80′ BEC/OOB · 50′ mã độc/USB · 30′ khôi phục/quiz |
| 4 | WiFi, thiết bị, VPN, làm việc từ xa | Môi trường kết nối & endpoint | 20′ mở · 70′ WiFi/router · 50′ thiết bị · 40′ VPN/BYOD |
| 5 | Dữ liệu, chia sẻ, AI, văn hóa báo cáo | Bảo vệ dữ liệu trong vận hành hàng ngày | 20′ mở · 60′ phân loại · 50′ chia sẻ · 40′ AI · 30′ văn hóa |
| 6 | Sao lưu, phục hồi & ứng phó sự cố | Khi sự cố xảy ra — làm gì | 25′ tình huống · 55′ backup 3-2-1 · 55′ IR 6 bước · 45′ thực hành |
| 7 | Kỹ năng mềm khi hỗ trợ doanh nghiệp | Đi làm thực tế với MSME | 20′ vai trò · 70′ giao tiếp · 50′ rủi ro/KRI · 40′ thực hành |

---

## Buổi 1 — Xu hướng & khung pháp lý an toàn thông tin cho SME/MSME

**Nguồn:** Slide bài giảng đầy đủ (76 trang) — ThS/LS Lưu Xuân Vĩnh.

### Mục tiêu buổi (3h)
- Nhìn bức tranh ATTT toàn cầu & Việt Nam, vì sao MSME là mục tiêu.
- Nắm khung pháp lý VN liên quan ATTT / an ninh mạng / dữ liệu cá nhân.
- Hiểu hướng hợp nhất Luật An ninh mạng 2025 và mức chế tài đang siết.

### 1. Bức tranh toàn cảnh
- Các vụ breach lớn toàn cầu (y tế, quốc phòng, consumer) cho thấy: chi phí khắc phục cao, thời gian phục hồi dài, dữ liệu cá nhân là tài sản bị nhắm.
- Việt Nam: nhiều vụ lộ dữ liệu lớn (VNG, Thế Giới Di Động/Điện Máy Xanh, Vietnam Airlines…); 2025 tấn công tập trung mạnh vào dịch vụ tiêu dùng, bán lẻ/TMĐT; rò rỉ nội bộ (GitHub, Postman…) cũng đáng lo.
- Xu hướng: CaaS (Cybercrime-as-a-Service), ransomware, phishing/social engineering, rủi ro IoT/mobile, data flow + AI/Big Data thiếu mã hóa/khử nhận dạng.

### 2. Thực trạng MSME Việt Nam
- **Định nghĩa:** Luật Hỗ trợ DNNVV 2017 — ≤200 lao động BHXH bình quân + vốn ≤100 tỷ hoặc doanh thu ≤300 tỷ (chi tiết theo lĩnh vực tại NĐ 80/2021).
- MSME ~**98%** doanh nghiệp; siêu nhỏ ~69%; tạo >80% việc làm; đóng góp >45% GDP.
- Thực trạng: ~**61%** SME bị tấn công mạng trong 1 năm; ~40% mất dữ liệu quan trọng; ~35% gián đoạn dài; chi phí khắc phục ước **50–100 nghìn USD**/sự cố nhỏ.
- Điểm yếu điển hình: hạ tầng mỏng, phụ thuộc SaaS/cloud; thiếu nhân sự ATTT/IR; phản ứng chậm; nhận thức nhân viên thấp.

### 3. Khung pháp lý (tinh gọn để dạy 3h)
**Thế giới (để đối chiếu):** GDPR/NIS2/CRA (EU); NIST CSF + disclosure (US); CSL/DSL/PIPL (TQ); PDPA/Cybersecurity Act (SG)… — chung: accountability, TOMs, quản trị chuỗi cung ứng.

**Việt Nam — trục chính cho MSME:**
1. **Luật An ninh mạng 2025** (hiệu lực 01/7/2026 theo tài liệu sổ tay): **hợp nhất** Luật ATTM 2015 + Luật ANM 2018 → một khung an ninh + an toàn + dữ liệu + nhân lực; đầu mối Bộ Công an.
2. **Luật Bảo vệ dữ liệu cá nhân 91/2025/QH15** (hiệu lực 01/01/2026) + nghị định hướng dẫn (tài liệu nhắc NĐ 356/2025 thay NĐ 13/2023).
3. Các luật liên quan: Hiến pháp (đời tư); Luật Dữ liệu; CNTT; Viễn thông; BVNTD (chồng lấn mạnh với DLCN ở B2C); Bộ luật Lao động (còn mỏng về DLCN nhân sự).

**3 nhóm nghĩa vụ tối thiểu cần nhớ:**
- An toàn thông tin mạng
- An ninh mạng
- Bảo vệ dữ liệu cá nhân (vai trò: Bên kiểm soát / Bên xử lý / Kiểm soát-và-xử lý)

**Chế tài (điểm dạy “đau”):**
- Vi phạm DLCN có thể phạt tới **5% doanh thu** năm trước.
- Phạt hành chính theo nhóm hành vi (tin giả, malware, cản trở hệ thống…); nghĩa vụ phản hồi quyền chủ thể (rút đồng ý, sửa, xóa) có thời hạn ngắn.
- Thông điệp: *Không gian mạng là ảo — hậu quả pháp lý là thật*; chi phí phạt/bồi thường > chi phí đầu tư phòng thủ nếu chủ quan.

### 4. Đào tạo nhân lực (góc pháp lý)
- Thiếu hụt nhân sự ATTT lớn; cần đào tạo liên ngành **kỹ thuật + pháp lý**.
- Đề xuất: tư duy **CIA → CIA-P** (thêm Privacy); Privacy by Design; giảng dạy chéo với luật sư/chuyên gia privacy.

### Thông điệp chốt Buổi 1
MSME không “nhỏ quá nên không ai tấn công”; pháp lý đang siết; tuân thủ = chứng minh được biện pháp đã làm, không chỉ “có chính sách trên giấy”.

---

## Buổi 2 — Nhận diện tài sản số & quản trị danh tính/truy cập

**Nguồn:** Sổ tay tóm tắt P1 + P2.

### Mục tiêu buổi (3h)
- Kiểm kê tài sản số theo 3 bước; map sang NIST CSF 2.0.
- Áp dụng mật khẩu/passphrase hiện đại + MFA + quyền tối thiểu + thu hồi quyền.
- Loại bỏ phần mềm crack khỏi tư duy “tiết kiệm”.

### Phần A — Tài sản số & rủi ro (P1)
**Tình huống mở:** Email giao dịch bị chiếm → mạo danh yêu cầu khách chuyển tiền (thiếu kiểm kê, thiếu MFA, thiếu giám sát đăng nhập).

**Rủi ro =** mối đe dọa khai thác lỗ hổng của tài sản → tác động bất lợi.

**NIST CSF 2.0 — 6 chức năng (câu hỏi SME):**
| Chức năng | Câu hỏi thực tế |
|-----------|-----------------|
| Govern | Ai chịu trách nhiệm? Có chính sách/ngân sách? |
| Identify | Đang có tài sản nào? Cái nào quan trọng? |
| Protect | MFA, phân quyền, sao lưu, mã hóa? |
| Detect | Cảnh báo đăng nhập lạ, rà soát định kỳ? |
| Respond | Ai xử lý sự cố? Có quy trình? |
| Recover | Khôi phục dữ liệu/hệ thống thế nào? |

**5 việc SME cần làm với tài sản số:** danh sách tài sản quan trọng → người chịu trách nhiệm → phân quyền → MFA → sao lưu định kỳ. Đây là vận hành **liên tục**, không checklist một lần.

**4 mối đe dọa phổ biến:** BEC · Phishing/Smishing · Xác thực yếu · Thiết bị/PM lỗi thời (+ ransomware nếu không có backup).

**Kiểm kê 3 bước:** Liệt kê → Phân loại → Đánh giá (ưu tiên).  
Nhóm ưu tiên cao: email DN, CSDL khách hàng, laptop, mã nguồn.

### Phần B — Danh tính là vành đai mới (P2)
**Tình huống:** Cùng mã độc — tài khoản Admin vs User thường → thiệt hại khác nhau.  
**Zero Trust tinh thần:** MFA + quyền tối thiểu + thu hồi khi nghỉ việc.

**Mật khẩu (NIST SP 800-63B — tinh gọn):**
- Ưu tiên **độ dài** (≥8 bắt buộc, khuyến nghị ≥15); cho phép dán (password manager).
- Không ép công thức hoa/số/ký tự; không đổi định kỳ trừ khi bị xâm phạm; chặn mật khẩu đã lộ.
- Passphrase: **Dài → Ngẫu nhiên → Duy nhất**.

**MFA ưu tiên:** Email → Ngân hàng/ví → MXH → Tài khoản công việc/cloud.  
Lưu ý: OTP/app giảm rủi ro; **FIDO2/passkey/khóa cứng** mới kháng phishing mạnh.

**Quản trị truy cập:** đúng người – đúng quyền – đúng thời điểm; tách nhiệm vụ; rà soát định kỳ.  
Khi nghỉ việc: **Disable trước, Delete sau** (giữ chứng cứ/bàn giao).

**Phần mềm crack:** rủi ro mã độc + chế tài bản quyền (NĐ xử phạt; có thể hình sự Điều 225 BLHS với pháp nhân).

### Thông điệp chốt Buổi 2
1. Tài sản số phải được kiểm kê và ưu tiên.  
2. MFA + quyền tối thiểu + thu hồi kịp thời.  
3. Chỉ dùng phần mềm hợp pháp.  
4. ATTT là việc của mọi người.

---

## Buổi 3 — Kỹ nghệ xã hội, lừa đảo tài chính & mã độc

**Nguồn:** Sổ tay tóm tắt Buổi 3.

### Mục tiêu buổi (3h)
- Nhận diện social engineering; dừng 10 giây trước khi click.
- Chống BEC bằng xác thực ngoài kênh (OOB) và phân tách phê duyệt thanh toán.
- Ứng xử đúng với USB/mã độc và khôi phục sau sự cố chiếm tài khoản.

### Nội dung cốt lõi
**Social engineering:** thao túng tâm lý, không cần bẻ khóa hệ thống.  
Ví dụ: email giả Google/Microsoft “hộp thư đầy” → mất mật khẩu → mở đường BEC.

**6 kịch bản BEC:** giả giám đốc · giả NCC đổi STK · giả hóa đơn · chiếm email thật chen thanh toán · giả luật sư/đối tác · chuyển hướng lương.

**5 việc chống lừa đảo tài chính (làm ngay):**
1. OOB khi đổi số tài khoản thanh toán (**quan trọng nhất**)
2. Tách người tạo lệnh / duyệt / chuyển tiền
3. MFA email, kế toán, ngân hàng, cloud
4. SPF/DKIM/DMARC
5. Dừng 10 giây trước khi click/mở file/gửi tin

**OOB:** xác minh bằng kênh độc lập đã biết trước (gọi số nội bộ/chính thức), không gọi lại số trong email nghi ngờ.

**Kênh tấn công:** Phishing · Vishing · Smishing (SMS/Zalo → app giả → lấy OTP) · USB giả thiết bị / macro / USB Killer.

**5 hành vi rủi ro cao:** đưa OTP qua điện thoại · đăng nhập qua link SMS/Zalo · cắm USB lạ · đổi STK không xác minh · upload tài liệu mật lên công cụ công khai.

**Checklist 4 dấu hiệu nghi ngờ:** nguồn bất thường · yêu cầu lệch quy trình · áp lực thời gian/giữ bí mật · xin OTP/mật khẩu/CCCD/cài app lạ.

**Khôi phục 3 bước:** Bảo vệ tài khoản (đổi MK + MFA) → Thu hồi quyền/phiên lạ → Rà soát chia sẻ Drive/OneDrive.

### Thông điệp chốt Buổi 3
Kẻ tấn công thắng khi bạn vội. Đổi tài khoản thanh toán = luôn OOB. Nghi ngờ → cô lập trước, xác minh sau.

---

## Buổi 4 — WiFi, thiết bị, VPN & làm việc từ xa

**Nguồn:** Sổ tay tóm tắt Buổi 4.

### Mục tiêu buổi (3h)
- Khóa “cửa mạng” văn phòng (router/WiFi khách).
- Bảo vệ endpoint (laptop/điện thoại/USB).
- Làm việc ngoài văn phòng an toàn (VPN/BYOD/remote policy).

### Nội dung cốt lõi
**Tình huống:** WiFi quán cafe + hợp đồng lớn + Fanpage + không VPN → chiếm MXH → lừa khách.

**WiFi công ty “mở cửa” khi:** MK yếu · không đổi admin router · nhân viên/khách chung SSID · MK dán tường · firmware cũ · phủ sóng quá rộng.

**5 việc làm ngay:**
1. Đổi mật khẩu router mặc định  
2. MK WiFi mạnh, khác router  
3. **WiFi khách riêng, cách ly LAN**  
4. Cập nhật firmware 1–2 tháng/lần  
5. Xóa kết nối lạ định kỳ  

**Thiết bị:** laptop (hợp đồng/email/KT), điện thoại (Zalo OA/ngân hàng), USB/ổ cứng (thường thiếu MK).  
Lỗi nguy hiểm: không khóa màn hình · crack · không update (WannaCry) · USB lạ · dùng chung 1 tài khoản.  
Mất máy → mã hóa ổ đĩa + MK mạnh + Find My Device.

**Làm việc từ xa:**
- WiFi công cộng → **bắt buộc VPN** (ví dụ Cloudflare WARP miễn phí).
- Ưu tiên 4G/5G khi nhạy cảm; privacy screen; không share màn hình thừa.
- Không mở dữ liệu nhạy cảm nơi đông người.
- Ransomware: không crack · không mở file lạ · update OS · backup 3-2-1.

**BYOD tối thiểu:** OS cập nhật · AV hợp lệ · MK/vân tay · khóa màn ≤5 phút · không crack · ký BYOD Agreement.  
**Remote work policy:** VPN bắt buộc · chỉ dùng Drive/OneDrive/email công ty · MFA · báo ngay khi mất máy.

### Thông điệp chốt Buổi 4
WiFi yếu = cửa không khóa. Máy không vá = cửa sổ cho hacker. Crack đắt hơn phần mềm miễn phí hợp pháp.

---

## Buổi 5 — Bảo vệ dữ liệu, kiểm soát chia sẻ, AI & văn hóa không đổ lỗi

**Nguồn:** Sổ tay tóm tắt Buổi 5.

### Mục tiêu buổi (3h)
- Phân loại dữ liệu và hiểu vòng đời dữ liệu.
- Chia sẻ có kiểm soát (không “Anyone with the link”).
- Dùng AI an toàn; xây văn hóa báo cáo sớm.

### Nội dung cốt lõi
**3 vòng bảo vệ:** Con người + Governance + Công nghệ.  
Thống kê nhắc trong slide: nhiều NV không biết chính sách phân loại; phần lớn breach liên quan hành vi con người; chi phí trung bình breach rất cao.

**7 hành vi rủi ro nơi làm việc:** link Drive “anyone” · gửi KH qua Gmail cá nhân · nhét dữ liệu nhạy cảm vào ChatGPT · MK trong Excel · không khóa màn · tải file lạ · trộn folder cá nhân/công ty.

**DLCN (theo NĐ 13/2023 trong sổ tay; buổi 1 đã cập nhật hướng Luật 91/2025):**  
- Cơ bản vs Nhạy cảm.  
- Ma trận DN: Công khai → Nội bộ → Bảo mật → Tuyệt mật.  
- Vòng đời: Thu thập → Lưu trữ → Sử dụng → Chia sẻ → Lưu dài hạn → Xóa an toàn.  
- Vi phạm có thể phạt nặng (nhắc mức tới **5% doanh thu**).

**Chia sẻ an toàn — 7 bước:** nhu cầu → phân loại → người nhận → phê duyệt theo mức mật → quyền tối thiểu → audit log → thu hồi khi hết hạn.  
Ưu tiên “Người cụ thể” + ngày hết hạn; tránh share cả folder; thu hồi NV cũ; NDA với đối tác.

**AI an toàn:**  
Rủi ro: rò rỉ dữ liệu · hallucination · phụ thuộc AI · bản quyền mơ hồ.  
**Nguyên tắc vàng:** không nhập KH/tài chính/mã nguồn/bí mật KD vào AI công cộng.  
**Data masking:** Mask → Prompt → Điền lại; luôn kiểm chứng kết quả.

**Văn hóa không đổ lỗi:** báo cáo sớm giảm thiệt hại lớn; IR theo tinh thần Identify→Protect→Detect→Respond→Recover.

### Thông điệp chốt Buổi 5
Dữ liệu được bảo vệ vì mọi người hiểu trách nhiệm — không chỉ vì có nhiều công cụ. Phân loại trước, rồi mới chia sẻ/AI.

---

## Buổi 6 — Sao lưu, phục hồi & ứng phó sự cố

**Nguồn:** Slide chi tiết Topic 1 + 2 + 3 (cùng bài, 3 mạch: chuẩn bị backup · quy trình IR · thực hành triển khai).

### Mục tiêu buổi (3h)
- Hiểu backup chỉ “thật” khi **restore được**.
- Thực hiện đúng 6 bước ứng phó; checklist 30 phút đầu.
- Mang về mẫu: IR Card, danh bạ khẩn cấp, mục tiêu ATTT 90 ngày.

### Topic 1 — Chuẩn bị trước sự cố (Backup)
**Tình huống ransomware:** file kế toán bị mã hóa, backup cloud cũ 3 tuần / không offline → thảo luận 30 phút đầu.

**Vì sao SME dễ dính:** thiếu backup/test restore · không IT chuyên trách · crack/BYOD · dữ liệu tập trung 1–2 người · tâm lý “công ty nhỏ” · NV chưa đào tạo.

**Thiệt hại tham chiếu slide:** nhiều SME phá sản sau sự cố lớn; downtime trung bình dài; chi phí phục hồi cao hơn phòng ngừa nhiều lần; case VN: ~9 ngày dừng, mất ~800 triệu doanh thu.

**Dấu hiệu cảnh báo (báo trong 5 phút):** máy chậm/CPU 100% · popup/AV bị tắt · file không mở / đổi đuôi `.locked` · email tự gửi · đăng nhập IP lạ · KH báo tin nhắn lạ từ công ty.

**Nguyên tắc vàng khi sự cố:** đừng hoảng · đừng tự ý sửa · báo 5 phút · cách ly (rút mạng/tắt WiFi, ngắt sync cloud) · ghi nhận bằng chứng · **không trả tiền chuộc**.

**Backup 3-2-1:** 3 bản · 2 loại phương tiện · 1 bản offsite.  
Sai lầm phổ biến: không test restore · 1 ổ duy nhất · ổ backup luôn cắm · tưởng cloud tự backup · không người chịu trách nhiệm.  
**Restore test:** chọn 3–5 file → copy máy khác → mở kiểm tra → đo thời gian → ghi log; tháng 1 lần, quý full system.

### Topic 2 — Quy trình ứng phó 6 bước (vòng lặp)
1. **Chuẩn bị:** 3-2-1, IR Card, phân vai, danh bạ, tabletop mỗi quý  
2. **Phát hiện:** NV/KH/AV/log/cloud alert — ghi thời gian & phạm vi  
3. **Kiểm soát/cách ly:** rút mạng (**không tắt máy** nếu cần giữ log RAM), ngắt sync, khóa TK, không cắm USB backup vào máy nhiễm  
4. **Xóa bỏ:** tìm patient zero, quét malware, đổi MK, gỡ PM lạ, vá lỗ hổng, rà quyền admin & mail rules  
5. **Phục hồi:** xác nhận sạch → restore backup đã verify → theo dõi 24–48h → MFA lại → thông báo bên liên quan / cân nhắc VNCERT  
6. **Rút kinh nghiệm:** root cause → cập nhật chính sách/đào tạo → cải tiến Chuẩn bị  

Phân vai: Giám đốc (quyết định/truyền thông) · IT (kỹ thuật) · Kế toán (giao dịch/ngân hàng) · Mọi NV (báo sớm, không tự xử).  
Phân mức sự cố 1/2/3 — không chắc thì xử như mức cao nhất trước.

### Topic 3 — Thực hành & vận hành 90 ngày
**Checklist 30 phút đầu:** báo quản lý/IT · cách ly · không xóa/không trả tiền · xác định phạm vi · kiểm tra backup gần nhất · chụp bằng chứng · kiểm tra email bị chiếm · liên hệ VNCERT nếu lộ DLCN.

**Mục tiêu đo được (ví dụ 90 ngày):**
- MFA 100% tài khoản quan trọng  
- Backup dữ liệu quan trọng hàng ngày  
- Vá lỗi ≤ 7 ngày  
- Test restore mỗi tháng  
- Diễn tập IR mỗi quý  

Lịch: **tuần** (log backup, đăng nhập lạ, quét AV, update, quyền Drive) · **tháng** (restore 1 file, TK không dùng, danh bạ, quy trình) · **quý** (tabletop, maturity, phishing training, kế hoạch quý sau).

**Thực hành lớp:** case BEC chuyển 250 triệu · thiết kế backup 3-2-1 · diễn tập ransomware · điền IR Card · danh bạ khẩn cấp · thử backup/restore cloud thật.

### Thông điệp chốt Buổi 6
Backup chưa test = backup ảo. Sự cố: cách ly + báo cáo + giữ hiện trường. Không trả tiền chuộc. IR là vòng lặp cải tiến.

---

## Buổi 7 — Kỹ năng mềm khi làm việc với doanh nghiệp

**Nguồn:** Slide bài giảng + mẫu doanh nghiệp (nhãn Bài 7–8 trên slide).

### Mục tiêu buổi (3h)
- Hiểu vai trò sinh viên trong dự án hỗ trợ MSME.
- Giao tiếp “trẻ nhưng không non”: phá băng, nói ngôn ngữ DN, trả lời đúng phạm vi.
- Mang khung rủi ro/KRI để quan sát và tư vấn đúng mức.

### Nội dung cốt lõi
**Vai trò:** mỗi nhóm ~2 SV hỗ trợ 3–5 DN; nhận mentorship từ thầy/cô & chuyên gia; chương trình Vườn ươm hỗ trợ kiến thức/phương pháp.

**Kỹ năng phá băng / chuyên nghiệp:**
- Đến sớm 10–15′, trang phục, thẻ đeo, tài liệu sẵn.
- Slide giới thiệu bản thân ngắn; hỏi DN đang lo ATTT gì trước khi “bắn” giải pháp.
- Nói ngôn ngữ DN: tránh jargon; lấy ví dụ gần (MK 123456, email giả); đưa link kiểm tra uy tín.
- **Không** sao chép/lưu/chia sẻ dữ liệu KH & tài liệu nội bộ; xin phép; chỉ dùng dữ liệu phục vụ việc được giao.

**Khi chưa chắc:** “Em cần kiểm tra lại để đảm bảo chính xác và phản hồi sau” — không bịa luật.

**Hình ảnh đại sứ:** chuyên nghiệp · chính trực · chủ động · đúng giờ · trách nhiệm · tôn trọng cam kết · trung thực · bảo mật · quan sát–đề xuất–hỗ trợ.

**Bản đồ rủi ro DN (để hỏi đúng người):**
| Mức | Khu vực | Bộ phận ảnh hưởng |
|-----|---------|-------------------|
| Cao | PM & thiết bị đầu cuối | Toàn DN |
| Cao | Dữ liệu KH & tài chính | KT – KD – BGĐ |
| TB–Cao | Email & giao tiếp | KD – Mua hàng – Lãnh đạo |
| TB | Nhân sự / insider | HR – IT |
| TB | Website & TMĐT | Marketing – KD online |
| Thấp hơn (tùy DN) | Hạ tầng mạng & cloud | IT – Vận hành |

**Khung quản trị:** tư duy ISO 31000 + ISO 27001 (nhận diện–đánh giá–xử lý rủi ro; không cần chứng nhận ngay).

**KRI đại diện (siêu nhỏ / nhỏ / vừa):**  
- Người: phishing, nhận thức, SE report, insider  
- Kỹ thuật: malware/ransomware, lỗ hổng chưa vá, shadow IT, admin không MFA  
- Quy trình/tuân thủ: backup restore fail, PII request trễ hạn, thời gian báo cáo sự cố PII, thiết bị thiếu bảo mật cơ bản  

**3 nhóm năng lực SV cần:** nền tảng + pháp lý · kỹ thuật chuyên môn · quản trị & mềm (đánh giá tài sản/rủi ro, IR plan, tư vấn tuân thủ, đào tạo NV).

### Thông điệp chốt Buổi 7
Trẻ nhưng không non. Hiểu DN trước khi nói bảo mật. Bảo mật dữ liệu DN là điều kiện để được tin. Tư vấn bằng rủi ro đo được, không bằng thuật ngữ.

---

## Phụ lục A — Việc “làm ngay” mang về doanh nghiệp (xuyên suốt khóa)

1. Kiểm kê tài sản số quan trọng + người sở hữu  
2. MFA 100% email/cloud/ngân hàng/admin  
3. Password manager; bỏ tài khoản admin dùng hằng ngày  
4. Thu hồi/disable quyền khi nghỉ việc trong ngày  
5. OOB khi đổi STK thanh toán; tách tạo lệnh/duyệt/chi  
6. Đổi MK router; tách WiFi khách  
7. Backup 3-2-1 + test restore tháng này  
8. IR Card + danh bạ khẩn cấp dán văn phòng  
9. Cấm crack; update OS định kỳ  
10. Quy tắc AI: mask dữ liệu; không dán PII/bí mật vào AI công cộng  

---

## Phụ lục B — Thuật ngữ nhanh

| Thuật ngữ | Nghĩa ngắn |
|-----------|------------|
| MSME | Doanh nghiệp siêu nhỏ, nhỏ và vừa |
| NIST CSF 2.0 | Khung quản trị rủi ro ATTT 6 chức năng |
| BEC | Lừa đảo chiếm/giả email doanh nghiệp để chuyển tiền |
| MFA | Xác thực đa yếu tố |
| OOB | Xác thực ngoài kênh đang bị nghi ngờ |
| 3-2-1 | 3 bản backup, 2 loại media, 1 offsite |
| IR | Ứng phó sự cố |
| PII / DLCN | Dữ liệu cá nhân |
| BYOD | Mang thiết bị cá nhân đi làm |
| Zero Trust | Không tin mặc định; luôn xác thực & quyền tối thiểu |

---

## Phụ lục C — Nguồn gốc file trong thư mục

| Buổi | File |
|------|------|
| 1 | `Buổi 1 - Xu hướng và khung pháp lý an toàn thông tin cho SME MSME.pdf` |
| 2 | `Buổi 2 - Sổ tay tóm tắt (P1).pdf` + `(P2).pdf` |
| 3 | `Buổi 3 - Sổ tay tóm tắt.pdf` |
| 4 | `Sổ tay tóm tắt buổi 4.pdf` |
| 5 | `Sổ tay tóm tắt buổi 5.pdf` |
| 6 | `Buổi 6_Topic 1.pdf` · `Topic 2.pdf` · `Topic 3.pdf` |
| 7 | `[Slide bài giảng + Mẫu doanh nghiệp] Buổi 7.pdf` |

---

*Ghi chú biên soạn: Buổi 1 và 6/7 được **nén** về cùng mật độ với Buổi 2–5 để mỗi buổi dạy được trong ~3 giờ; chi tiết pháp lý/so sánh điều luật đầy đủ vẫn nằm ở slide gốc Buổi 1.*
