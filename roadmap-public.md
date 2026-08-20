# LỘ TRÌNH BACKEND DEVELOPER — Sinh viên Software Engineering

> **Đây là lộ trình cá nhân, công khai để tham khảo.** Nó được xây quanh một ràng buộc cụ thể: lịch học từng kỳ đã biết trước, và hai môn nặng nhất về backend rơi vào kỳ 3. Mọi mốc đều tính ngược từ đó. Nếu bạn ở hoàn cảnh khác, phần đáng lấy là **cách tổ chức** — mô hình AI 3 nấc, nguyên tắc chọn môn theo trọng số, cơ chế checkpoint — chứ không phải lịch cụ thể.

> **Bản này đã lược bỏ phần riêng tư:** mục tiêu điểm số, kế hoạch xin việc, và các ghi chú cá nhân khác. Cấu trúc và lý do đằng sau mỗi quyết định thì giữ nguyên.

---

## 0. NGUYÊN TẮC NỀN

1. **Mô hình dùng AI theo 3 nấc:**
   - **Nấc 1 (Giai đoạn 0-1, đến hết 6/9/2026):** cấm AI viết code, chỉ giải thích khái niệm.
   - **Nấc 2 (Giai đoạn 2-3, kỳ 3-4):** AI là giám khảo/reviewer — chê code mình viết, không nhận code AI sinh sẵn.
   - **Nấc 3 (từ đầu kỳ 5, hoặc ngay khi vào bất kỳ môi trường làm việc thật nào — tùy cái nào đến trước):** AI-assisted có thẩm định — AI viết boilerplate/test cho phần đã chứng minh tự viết được, mình review từng dòng.
2. **Quy tắc tiếng Anh mặc định:** mọi tài liệu học, README, commit message, comment trong code — 100% tiếng Anh, không ngoại lệ.
3. **Xuất phát điểm kỹ thuật:** nắm HTTP/REST/CRUD ở mức khái niệm, Git flow cơ bản, vừa tạo project Spring Boot đầu tiên. Chưa viết được CRUD hoàn chỉnh, chưa viết SQL bằng tay.
4. **Trượt môn = lùi toàn bộ lộ trình.** Không đánh đổi.
5. **Commit GitHub hàng ngày** là thước đo kỷ luật, không phải năng lực.
6. **Phương án khi trễ nhịp:** mỗi checkpoint đi kèm 3-5 câu hỏi đạt/không đạt. Nếu **≥2 câu trả lời "không"**, coi là trễ nhịp và cắt theo thứ tự định sẵn: đọc thêm ngoài chương trình → LeetCode vượt chỉ tiêu → tính năng phụ của dự án → hoạt động ngoại khoá. **Không bao giờ cắt:** SQL, Git flow, dự án cá nhân lõi, testing, đọc code người khác.

   Quyết thứ tự cắt lúc đang bình tĩnh tốt hơn quyết lúc còn hai ngày và đang hoảng.
7. **Ưu tiên môn theo trọng số backend.** Không đầu tư đều tay cho mọi môn — xếp hạng theo mức độ liên quan tới nghề, rồi dồn thời gian vào nhóm cao nhất:

| Kỳ | Môn trọng tâm | Vì sao |
|---|---|---|
| 3 | DBI202, LAB211 | Database và lập trình ứng dụng — nền trực tiếp |
| 4 | CSD201, PRJ301, SWR302 | Cấu trúc dữ liệu, Java web, phân tích yêu cầu |
| 5 | SWP391, SWT301 | Project nhóm và testing |
| 6 | OJT202 | Thực tập doanh nghiệp |
| 7 | SWD392 | Kiến trúc phần mềm — thứ phân biệt junior với senior |
| 9 | Đồ án tốt nghiệp | Showcase toàn bộ kỹ năng |

   Các môn còn lại: học đủ qua môn, không đầu tư thêm. **Không đua GPA tổng** — thời gian tiết kiệm được đổ vào dự án cá nhân và đọc code.

8. **Chiến lược Elective (mới):** có 4 slot elective — SE-0001 (kỳ 5), SE-0002 và SE-0003 (kỳ 7), SE-0004 (kỳ 8). Nguyên tắc: **chọn môn liên quan backend, không chọn môn dễ điểm.** Ưu tiên theo thứ tự: Cloud/DevOps > Security > Distributed Systems > Data Engineering. Trước mỗi kỳ có elective, dành 1 buổi đọc danh sách môn mở và tìm hiểu môn nào dạy thật, không chỉ đọc tên môn.

---

## 1. VIỆC LÀM HÀNG NGÀY — TỪ HÔM NAY

- [ ] ≥1 commit GitHub/ngày (kể cả chỉ là log học được gì).
- [ ] Mọi thứ viết ra (code, comment, note, README) — tiếng Anh.
- [ ] Cuối ngày tự hỏi: tự gõ bao nhiêu %, AI viết hộ bao nhiêu %? Mục tiêu >90% ở Nấc 1-2.

**Hàng tuần (Chủ nhật):**
- [ ] Tổng kết `WEEKLY_LOG.md` bằng tiếng Anh: học được gì, còn mù mờ gì.
- [ ] Chạy ít nhất 1 bài test tự kiểm tra (mục 8) — **từ kỳ 3**.
- [ ] Chỉ tiêu LeetCode/SQL của tuần đó — nói to bằng tiếng Anh khi giải.

**Từ kỳ 3 (7/9/2026), thêm:**
- [ ] **1h/tuần đọc code người khác:** mở source một thư viện nhỏ hoặc một dự án Spring Boot mẫu trên GitHub, tự giải thích được nó làm gì. Đây là kỹ năng thực tế nhất khi vào OJT — việc đầu tiên luôn là đọc code cũ, không phải viết mới.

**Từ kỳ 4 (khoảng 1/2027), thêm:**
- [ ] **1 buổi mock technical interview tiếng Anh / 2 tuần với AI:** giải thích thuật toán, trả lời "walk me through your project", luyện vocab kỹ thuật.

---

## 2. MỐC THỜI GIAN TỔNG QUAN

| Giai đoạn | Thời gian | Kỳ | Môn trọng tâm | Trọng tâm tự học |
|---|---|---|---|---|
| 0 | 2/7 – 1/8/2026 | kỳ 2 | PRO192, MAD101, NWC203c, OSG202 | Qua 4 môn |
| 1 | 1/8 – 6/9/2026 | nghỉ | — | Nền REST API/CRUD Java + Git flow |
| 2 | 7/9 – 29/11/2026 | kỳ 3 | DBI202, LAB211 | SQL sâu, Spring Boot mở rộng, CLB, đọc code người khác |
| — | 30/11 – 12/2026 | nghỉ | — | Chuẩn bị CSD201 trước kỳ nghẽn |
| 3 | ~11/1 – 4/2027 | kỳ 4 | CSD201, PRJ301, SWR302 | DSA + LeetCode nặng, dự án #1, mock interview |
| 4 | ~5 – 8/2027 | kỳ 5 | SWP391, SWT301, SE-0001 | Dự án #2, internship part-time, hồ sơ OJT |
| 5 | ~9 – 12/2027 | kỳ 6 | OJT202 | **OJT** |
| 6 | ~1 – 8/2028 | kỳ 7-8 | SWD392, SE-0002/3/4 | Architecture, design pattern, chuyên sâu 1 nhánh |
| 7 | ~9 – 12/2028 | kỳ 9 | SE_GRA_ELE | Đồ án tốt nghiệp như sản phẩm thật |

---

## GIAI ĐOẠN 0 — 2/7 → 1/8/2026: QUA MÔN BẰNG MỌI GIÁ

**Đã xong.** Thi hết 4 môn ngày 1/8/2026: PRO192, MAD101, NWC203c, OSG202.

Tự chấm 3 câu, cần đạt ≥2/3:
- [ ] Giải thích được từng dòng project PRO192 mà không nhìn tài liệu?
- [ ] Chỉ ra chính xác OSG202 đã học phần nào liên quan memory/process/file system?
- [ ] Điểm 4 môn còn margin an toàn, không chỉ "vừa qua"?

---

## GIAI ĐOẠN 1 — 1/8 → 6/9/2026: NỀN REST API/CRUD + GIT FLOW

Chi tiết theo ngày nằm ở file lịch riêng. Tóm tắt khối:

- **Tuần 1 (1–7/8):** Client/server, HTTP, REST, CRUD, database. Git flow: branch, PR, merge conflict, revert. Cài JDK, IntelliJ, Postman, PostgreSQL. **Đã xong.**
- **Tuần 2 (9–14/8):** Spring Boot + JPA + PostgreSQL. Entity → Repository → Service → Controller, gõ tay. Thêm exception handling, validation, DTO. **Đã xong.**
- **Tuần 3 (15–20/8):** project #1 hoàn chỉnh 4 tầng + exception + DTO + validation.
- **21–25/8:** đóng nốt project #1 (mã trạng thái 201/204, handler cho lỗi validation), tách cấu hình nhạy cảm khỏi repo, JUnit lần đầu — học công cụ mới trên code đã quen, không học hai thứ mới cùng lúc.
- **25/8 — checkpoint**, chạy **trước** khi mở project mới: không đạt thì cần biết ngay, không phải phát hiện giữa chừng.
- **26/8 – 6/9: Project #2**, viết **không có hướng dẫn từng bước** — AI chỉ giảng khái niệm mới (quan hệ 1-n), phần còn lại tự dựng. Đây là phép thử duy nhất xem đã tự viết được chưa.
- **Đuôi nhẹ đẩy sang tuần đầu kỳ 3 (7–11/9):** README tiếng Anh, SQL tay ngày 1 + 2, đọc đề cương 4 môn kỳ 3, block phỏng vấn 5 câu.

> **Bài học về quỹ thời gian:** bản kế hoạch đầu dành 14 ngày cho Project #2, nhưng các việc phát sinh ở project #1 (sửa mã trạng thái, gỡ bug, học JUnit) ăn mất phần lớn quãng đó. Cách xử lý: **bỏ hẳn một hạng mục** thay vì bóp nhỏ mọi thứ. Cụ thể là bỏ việc chép lại project #1 để luyện trí nhớ, dồn quỹ cho Project #2 — vì viết lại thứ đã có chỉ đo được trí nhớ, còn dựng một project mới đo được năng lực thật và tạo ra thứ dùng được.
>
> Thứ tự cắt nếu vẫn trượt: rebase/cherry-pick → bài tập debug ngược → JUnit của project #2 (giữ JUnit ở project #1) → rút Project #2 còn **2 entity quan hệ 1-n + CRUD**. **Không cắt** bản thân quan hệ 1-n — đó là thứ duy nhất Project #2 dạy mà project #1 không có.

**Bổ sung mới — 2 ngày SQL thuần trước khi vào kỳ 3:** trong Giai đoạn 1, Hibernate tự sinh bảng qua `ddl-auto`, nên chưa từng viết một câu SQL nào bằng tay. DBI202 (10/10) mở đầu kỳ 3 sẽ hỏi đúng thứ đó. Chèn vào 2 ngày buffer: tự viết `CREATE TABLE`, `INSERT`, `SELECT` có `WHERE`, `JOIN` hai bảng, `GROUP BY` — chạy trực tiếp trên `todo_db` và database project 2 đã có.

**Checkpoint 25/8 — tự chấm 4 câu, cần đạt ≥3/4:**
- [ ] Tự giải thích luồng request → server → database → response bằng lời mình?
- [ ] Tự viết được CRUD API Spring Boot không nhìn tutorial?
- [ ] Biết tạo branch, mở PR, và tự giải quyết một merge conflict?
- [ ] Repo có commit đều theo từng bước, không phải 1 commit "done" duy nhất?

---

## GIAI ĐOẠN 2 — Kỳ 3, 7/9 → 29/11/2026: DBI202 + LAB211 + MỞ RỘNG SỚM

**Môn trong kỳ:** DBI202 (10/10), LAB211 (10/10), MAS291 (5/10), SWE202c (5/10), JPD113 (2/10).
**Không có CSD201 trong kỳ này** — DSA để dành kỳ 4. Kỳ 3 chỉ giữ LeetCode ở mức làm quen, không chạy chỉ tiêu nặng.

**Nhịp thật của kỳ:** học 10 tuần **7/9 – 13/11**, thi **14/11 – 29/11**. Nghĩa là quỹ thời gian tự học chỉ có **tháng 9, tháng 10 và 2 tuần đầu tháng 11**. Đây là chỗ bản kế hoạch đầu tính sai gần một tháng: nó xếp việc tự học mới vào tháng 11-12 như thể còn học bình thường, trong khi nửa sau tháng 11 đã là mùa thi và tháng 12 không còn thuộc kỳ. Mọi việc "để dành cuối kỳ" phải dồn lên sớm hoặc đẩy sang kỳ nghỉ.

### Tháng 9 (từ 7/9)
- **DBI202:** đây là môn quan trọng nhất kỳ. Học SQL nghiêm túc từ đầu, không dựa vào JPA sinh câu lệnh hộ. Viết tay mọi truy vấn trước khi để Hibernate làm.
- **LAB211:** 100% tự làm. Đây là nối tiếp trực tiếp của PRO192 — lợi thế sẵn có, tận dụng để lấy điểm cao mà không tốn nhiều giờ.
- **SWE202c:** Agile/Scrum/SDLC. Học đủ qua môn, nhưng ghi lại thuật ngữ quy trình (sprint, backlog, standup) — dùng thật khi vào SWP391 và OJT.
- **MAS291:** học đủ qua môn.
- LeetCode Easy 3-5 bài/tuần, chủ đề array và string. Chỉ để giữ nhịp.
- Tham gia một CLB lập trình/công nghệ.
- AI chuyển sang **Nấc 2**.
- Bắt đầu 1h/tuần đọc code người khác.
- **Việc ngoài file, làm trong tháng này:**
  - [ ] Xác minh cơ chế thực tập doanh nghiệp của trường: deadline nộp hồ sơ, quy trình chọn công ty, có được tự apply ra ngoài không. Mọi mốc của giai đoạn sau đang dựa trên giả định chưa kiểm chứng.
  - [ ] Tìm sinh viên khóa trên vừa đi thực tập về, hỏi 30 phút về quy trình thật và kỳ vọng thực tế.

> **Nguyên tắc chung:** lộ trình viết trên giấy chỉ đúng đến giới hạn thông tin mình có. Những lỗ hổng còn lại **chỉ xác minh được bằng hành động ngoài file** — hỏi người thật, đọc quy định thật. Đừng để AI hay tài liệu thay thế bước đó.

### Tháng 10
- **DBI202:** JOIN nâng cao, GROUP BY, HAVING, subquery, PK/FK. Làm lại toàn bộ truy vấn trên database của 2 project Giai đoạn 1.
- Spring Security (auth cơ bản), JPA quan hệ 1-n và n-n.
- Bảo mật cơ bản: OWASP Top 10 tổng quan, PreparedStatement/JPA chống SQL injection, hash password (BCrypt).
- LeetCode duy trì nhịp nhẹ.

### Tháng 11 — chia làm hai nửa khác hẳn nhau

**1/11 – 13/11 (còn học):**
- **DBI202:** index (đọc hiểu B-tree ở mức khái niệm, không tự cài), transaction, ACID, chuẩn hóa 1NF-3NF. Đây là phần cuối và cũng là phần hay ra thi — học xong trước 13/11, không để dây sang mùa thi.
- Testing: unit test JUnit cho service đã viết. Chuẩn bị sớm cho SWT301 ở kỳ 5.

**14/11 – 29/11 (thi):**
- **Chỉ ôn thi.** Không nhận việc tự học mới, không LeetCode chỉ tiêu, không đụng CSD201. Nguyên tắc mục 0.4 — trượt môn lùi toàn bộ lộ trình.

---

## KỲ NGHỈ — 30/11 → đầu 1/2027: CHUẨN BỊ CHO KỲ NGHẼN

Kỳ 3 hết ngày 29/11, kỳ 4 bắt đầu khoảng **11/1/2027**. Quãng nghỉ này khoảng 6 tuần và **không có môn nào** — đây là chỗ tốt nhất toàn lộ trình để đi trước kỳ nghẽn.

- Nghỉ hẳn 3-5 ngày trước, không mở máy.
- **Chuẩn bị CSD201:** tự cài linked list, stack, queue bằng Java thuần, không dùng thư viện. CSD201 là môn 10/10 của kỳ 4 và là môn khó nhất chương trình — vào kỳ 4 với ba cấu trúc này đã tự cài được thì đỡ hẳn tháng đầu.
- Ôn lại PRO192: PRJ301 kỳ 4 dạy Servlet/JSP, nền Java OOP phải chắc.
- LeetCode Easy giữ nhịp nhẹ, chưa chạy chỉ tiêu.
- **Checkpoint cuối kỳ 3 — tự chấm 5 câu, cần đạt ≥4/5:**
  - [ ] Tự build REST API CRUD Spring Boot + PostgreSQL trong một cuối tuần, AI chỉ review?
  - [ ] API có auth cơ bản chạy được?
  - [ ] Có ≥5 unit test pass?
  - [ ] Viết được truy vấn JOIN 3 bảng + GROUP BY bằng tay, không tra cú pháp?
  - [ ] Hai môn trọng tâm của kỳ đều đạt mức đã đặt ra?

---

## GIAI ĐOẠN 3 — Kỳ 4, ~11/1 → 4/2027: CSD201 + PRJ301 + DỰ ÁN #1

**Môn trong kỳ:** CSD201 (10/10), PRJ301 (9/10), SWR302 (7/10), JPD123 (2/10), IOT102 (2/10).

**Đây là kỳ nặng nhất toàn khóa** — hai môn 10 và 9 điểm backend cùng lúc, cộng dự án cá nhân #1. Kế hoạch phải tính đến việc CSD201 chiếm phần lớn quỹ thời gian tự học, không phải dự án.

**Lưu ý độ vênh công nghệ:** PRJ301 dạy Servlet/JSP, không phải Spring Boot. Đây là học song song 2 mô hình Java web, không phải mâu thuẫn (Servlet/JSP là nền để hiểu Spring hoạt động ra sao bên dưới), nhưng tính thêm **~2-3h/tuần**.

- **CSD201 (ưu tiên số 1):** Array, LinkedList, Tree, HashMap, Stack, Queue, sorting. Tự cài bằng Java trước khi dùng thư viện. LeetCode chạy chỉ tiêu thật từ đây: Easy → Medium, 5-8 bài/tuần, bám đúng chủ đề đang học trên lớp. Mục tiêu cuối kỳ 4: lũy kế ~60-80 bài.
- **PRJ301:** chủ động nhận phần backend; PR/code review thật với đồng team.
- **SWR302 (7/10, mới đưa vào):** biết đọc và phân tích requirement thì thiết kế API đúng ngay từ đầu. Áp dụng ngay: viết đặc tả requirement cho dự án cá nhân #1 trước khi code, không code trước rồi mới nghĩ.
- **Dự án cá nhân #1** (AI Nấc 2): backend hoàn chỉnh — đăng nhập, phân quyền (Spring Security), CRUD, PostgreSQL, deploy thật. Chọn bài toán có người dùng thật. README tiếng Anh chuẩn. Mọi endpoint có unit test.
- Bắt đầu 1 buổi mock technical interview tiếng Anh / 2 tuần.
- **Nhịp đề xuất:** tháng 1-2 dồn cho CSD201 + PRJ301, dự án #1 chỉ dựng khung; tháng 3 CRUD lõi + test; tháng 4 auth + deploy + README.
- **Cuối tháng 4:** nộp hồ sơ internship part-time (xem Giai đoạn 4).

**Checkpoint cuối kỳ 4 — tự chấm 5 câu, cần đạt ≥4/5:**
- [ ] Hai môn trọng tâm của kỳ đều đạt mức đã đặt ra?
- [ ] Dự án cá nhân #1 deploy thành công, chạy được từ URL công khai?
- [ ] Mọi endpoint có ít nhất 1 unit test?
- [ ] Tự cài lại được LinkedList và HashMap từ đầu, không nhìn?

---

## GIAI ĐOẠN 4 — Kỳ 5, ~5 – 8/2027: PROJECT NHÓM + TESTING + DỰ ÁN #2 + HỒ SƠ THỰC TẬP

**Môn trong kỳ:** SWP391 (8/10), SWT301 (7/10), SE-0001 Elective 1 (6/10), WDU203c (3/10), SSG105 (3/10).

Không có kỳ hè trống giữa kỳ 4 và kỳ 5 — kỳ 5 chạy full-time. Internship part-time là **lựa chọn có điều kiện song song**, không phải khoản thêm miễn phí: nhận nó thì phải cắt bớt chỗ khác.

- **SWP391:** nhận vai backend + database. Đây là project theo nhóm gần nhất với công việc thật.
- **SWT301 (mới đưa vào rõ ràng):** Software Testing — unit test, integration test, mock. Trùng khớp với phần testing đã tự học từ kỳ 3. Tận dụng: dùng chính dự án cá nhân làm bài tập môn, không làm hai việc riêng.
- **SE-0001:** áp dụng chiến lược elective ở mục 0.8. Nếu chọn được Cloud/DevOps thì Docker/CI của dự án #2 vừa là bài tập môn vừa là CV.
- **Dự án cá nhân #2 (chủ lực CV):** Spring Boot + JPA + Spring Security + Docker + CI đơn giản, test coverage tử tế, tài liệu API (Swagger/OpenAPI). Nếu không có internship, thêm caching (Redis). Một dự án sâu bị hỏi kỹ đáng giá hơn nhiều chủ đề học lướt.
- **Internship part-time:** chỉ nộp ở nơi chấp nhận lịch sinh viên (2-3 buổi/tuần hoặc remote linh hoạt). Không nộp full-time khi còn đi học. **Nếu đậu:** cắt hoạt động ngoại khoá, dự án #2 giảm phạm vi còn CRUD + test + auth + tài liệu API, AI chuyển **Nấc 3 ngay ngày đi làm đầu tiên**. **Nếu không đậu:** kỳ 5 chạy đúng kế hoạch trên.
- LeetCode lũy kế ~120-150 bài.
- **Hồ sơ thực tập nhắm có chủ đích:** nêu rõ năng lực tiếng Anh và kinh nghiệm internship nếu có; ưu tiên nhóm dự án có khách hàng nước ngoài; mở rộng sang công ty quốc tế có vòng phỏng vấn tiếng Anh — số ứng viên qua được vòng đó nhỏ hơn nhiều, đây là lợi thế đáng khai thác nếu có nền ngoại ngữ.

**Checkpoint cuối kỳ 5 — tự chấm 5 câu, cần đạt ≥4/5:**
- [ ] Hai môn trọng tâm của kỳ đều đạt mức đã đặt ra?
- [ ] Dự án #2 có Docker + CI chạy được?
- [ ] Hồ sơ thực tập đã nộp đúng deadline đã xác minh?
- [ ] LeetCode lũy kế ≥120 bài?

---

## GIAI ĐOẠN 5 — Kỳ 6, ~9 → 12/2027: THỰC TẬP DOANH NGHIỆP

**Môn trong kỳ:** OJT202 (10/10), ENW493c (2/10).

- Không có cú sốc "bật AI" (đã ở Nấc 3 từ trước). Nếu đã có internship part-time ở kỳ 5 thì cũng không còn cú sốc môi trường công ty; nếu chưa, đây là lần đầu — bù bằng Git flow và code review thật đã luyện qua PRJ301 và SWP391.
- Quan sát quy trình team thật, chủ động xin feedback định kỳ.
- Mục tiêu thật của kỳ này không phải điểm số mà là **chuyển CV từ sinh viên sang junior dev**: xin được thư giới thiệu, giữ liên hệ với mentor, ghi lại cụ thể mình đã làm phần nào trong hệ thống nào.
- ENW493c: học đủ qua môn.

---

## GIAI ĐOẠN 6 — Kỳ 7-8, ~1 → 8/2028: KIẾN TRÚC + CHUYÊN SÂU

**Kỳ 7:** SWD392 (10/10), SE-0002 (6/10), SE-0003 (6/10), PMG201c (5/10), EXE101 (1/10).
**Kỳ 8:** SE-0004 (6/10), ITE302c (3/10), PRM392 (2/10), EXE201 (1/10), MLN111, MLN122 (1/10).

- **SWD392 là môn quan trọng nhất của cả hai kỳ này** (10/10, ngang DBI202 và CSD201). Clean Architecture, design pattern (Singleton, Factory, Observer...), microservices, SOLID. Đây là thứ phân biệt junior với senior. Không học để qua môn — học để dùng lại ngay trong đồ án tốt nghiệp kỳ 9.
- **Ba elective SE-0002/0003/0004:** đây là cơ hội cuối để nạp Kafka, Docker, Kubernetes, Cloud, Security vào CV. Áp dụng mục 0.8 nghiêm túc, đừng chọn môn dễ điểm.
- **PMG201c (5/10):** học hiểu, không đào sâu. Có ích khi lên lead nhưng chưa cần ngay.
- **Chuyên sâu 1 nhánh, chọn 1 trong 3:** DevOps, bảo mật, hoặc AI engineering. Chọn theo elective đã học được, không chọn theo trend.
- db_tutorial hoàn thành 15/15 phần — làm vì đam mê hiểu sâu, không áp lực deadline.
- System design cơ bản: caching, message queue, scaling. Nối trực tiếp với SWD392.
- Các môn ≤3 điểm (ITE302c, PRM392, EXE, MLN): học đủ qua, không stress.

---

## GIAI ĐOẠN 7 — Kỳ 9, ~9 → 12/2028: ĐỒ ÁN TỐT NGHIỆP

**Môn trong kỳ:** SE_GRA_ELE (9/10), MLN131, HCM202, VNR202 (1/10).

- Đồ án tốt nghiệp là cơ hội showcase toàn bộ kỹ năng backend. Làm thứ gì thật: microservices, Kafka, Docker, CI/CD. Đây là thứ nhà tuyển dụng sẽ hỏi kỹ nhất.
- Áp dụng trực tiếp SWD392 đã học kỳ 7 — không thiết kế lại từ đầu bằng cảm tính.
- **Có thể tính đến:** với nền công ty quốc tế qua internship và thực tập, đánh giá khả năng làm remote hoặc cho công ty nước ngoài — nhưng đây là bước sau 1-2 năm kinh nghiệm, không phải mục tiêu ngay khi ra trường.
- 3 môn chính trị: học đủ qua.

---

## 8. HỆ THỐNG TỰ KIỂM TRA (từ Giai đoạn 2, ≥1 bài/tuần)

1. **Test trang trắng:** 24h sau, viết lại phần lõi từ đầu.
2. **Test giải thích từng dòng:** mở file cũ, giải thích to bằng tiếng Anh. Kẹt >2-3 dòng là cờ đỏ.
3. **Test biến thể:** tự đổi 1 yêu cầu, tự cài đặt.
4. **Test debug ngược:** nhờ AI cấy bug ẩn, tự tìm không dùng AI.
5. **AI làm giám khảo:** nhờ AI hỏi 5 câu như interviewer, tự chấm.
6. **Test giải thích test:** với mỗi unit test, tự hỏi "test này chứng minh gì, xóa dòng nào thì test vẫn pass sai?"

---

## 9. LƯU Ý RỦI RO

- Trượt môn luôn thắng lộ trình tự học.
- **Kỳ 4 là điểm nghẽn của toàn lộ trình** — CSD201 và PRJ301 cùng lúc, cộng dự án #1, cộng bắt đầu mock interview. Nếu có kỳ nào phải hy sinh dự án cá nhân để giữ điểm môn, đó là kỳ 4. Chuẩn bị trong **kỳ nghỉ 12/2026** là cách giảm rủi ro rẻ nhất — và giờ là cách duy nhất, vì tháng 11 kỳ 3 đã bị mùa thi chiếm mất.
- Không có buffer nghỉ hoàn toàn ngoài cuối mỗi kỳ — tự thêm 2-3 ngày nghỉ hẳn sau mỗi kỳ thi.
- **Không đổi hướng sang "nhắm remote quốc tế ngay khi ra trường"** — vị trí remote cho fresher gần như không tồn tại. Nếu có lợi thế ngoại ngữ thì dùng đúng cách: công ty quốc tế trong nước trước → tích kinh nghiệm → remote sau.
- Phòng hộ dài hạn đáng tin: nền tảng, khả năng phán đoán/debug, khả năng đọc code người khác, hiểu nghiệp vụ, dùng AI có thẩm định.
- Hoạt động ngoại khoá là phần cắt **cuối cùng**, không phải đầu tiên — nó là nơi gặp người, thứ không tự học thay được. Internship là biến số linh hoạt.
- 10-15h tự học/tuần ngoài giờ chính khóa, kéo dài hơn 1 năm đến OJT. Tự đánh giá mỗi 2-3 tháng.

---

## 10. GHI CHÚ VỀ CÁCH LỘ TRÌNH NÀY ĐƯỢC XÂY

Bản này là kết quả của nhiều vòng tự phản biện. Bốn lỗi lớn từng mắc, ghi lại vì chúng là loại lỗi dễ lặp:

1. **Xếp môn sai kỳ.** Bản đầu đặt môn cấu trúc dữ liệu vào kỳ 3, kéo theo toàn bộ kế hoạch LeetCode và checkpoint của kỳ đó dựa trên một giả định sai. Bài học: **đối chiếu với bản đồ môn học thật trước khi lên kế hoạch**, đừng nhớ theo cảm tính.

2. **Bỏ sót môn quan trọng.** Vài môn có liên quan trực tiếp tới backend bị bỏ hoàn toàn khỏi bản đầu chỉ vì tên môn không gợi ra điều đó. Bài học: đọc **mô tả môn**, không đọc tên môn.

3. **Sai mốc thời gian của kỳ.** Lệch vài ngày ở đầu kỳ và gần một tháng ở cuối kỳ — đủ để xếp việc tự học mới vào đúng mùa thi. Bài học: **lấy lịch thật từ trường**, và kiểm lại cả ngày kết thúc chứ không chỉ ngày bắt đầu.

4. **Gộp nhiều kỳ thành một khối.** Bản đầu gộp hai năm cuối thành "2028 → tốt nghiệp", làm mất hai môn quan trọng nhất giai đoạn đó. Bài học: khối càng dài thì càng dễ giấu đi thứ đáng lẽ phải nổi bật.

**Điểm dừng của việc lập kế hoạch:** đến một lúc, mọi lỗ hổng còn lại đều thuộc loại **không thể sửa bằng cách viết lại file**. Chúng chỉ xác minh được bằng hành động thật — hỏi phòng ban của trường, hỏi người đã đi qua, đọc quy định gốc. Nhận ra điểm dừng đó và đi làm việc thật, thay vì lập kế hoạch vòng thứ năm, cũng là một phần của kế hoạch.
