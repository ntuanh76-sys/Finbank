# Finbank Credit Risk Analysis Dashboard
Dashboard Power BI phân tích hoạt động tín dụng, tiền gửi và rủi ro nợ xấu của FinBank (dữ liệu giả định), tập trung vào tăng trưởng dư nợ, chất lượng tín dụng theo vùng, bộ đệm rủi ro và kiểm soát nợ xấu.

## Tổng Quan Dữ Liệu

Bộ dữ liệu ghi nhận hoạt động tín dụng và huy động của FinBank theo tháng, trải dài từ 01/2024 đến 07/2025 (19 tháng), phân theo 3 vùng kinh doanh: Miền Bắc (MB), Miền Nam (MN), Miền Trung (MT). Dữ liệu bao gồm thông tin về dư nợ vay, giải ngân mới, tiền gửi, khách hàng hoạt động, nợ xấu (NPL), nợ nhóm 2 (Stage 2) và dự phòng rủi ro.

**Phạm vi dữ liệu:** giai đoạn 01/2024 - 07/2025, dữ liệu giả định phục vụ mục đích phân tích và trình bày.

## Mục Tiêu Phân Tích

- Theo dõi tăng trưởng dư nợ tín dụng và tiền gửi theo thời gian.
- Đánh giá chất lượng tín dụng qua tỷ lệ nợ xấu (NPL Ratio) so với mục tiêu đề ra.
- So sánh hiệu quả hoạt động và mức độ rủi ro giữa các vùng kinh doanh.
- Đánh giá mức độ đầy đủ của bộ đệm rủi ro (dự phòng) so với tổng rủi ro tín dụng.
- Phát hiện sớm xu hướng nợ xấu và nợ nhóm 2 để cảnh báo trước khi chuyển nhóm nợ xấu chính thức.

## Chỉ Số Chính

| Nhóm phân tích | Chỉ số |
|---|---|
| Kinh doanh | Dư Nợ Vay, Giải Ngân Mới, Tổng Tiền Gửi, Khách Hàng Hoạt Động |
| Tăng trưởng | Loan Growth, Deposit Growth, Active Customer Achievement |
| Chất lượng tín dụng | NPL Ratio, NPL Balance, Nợ Xấu Phát Sinh Mới, Stage 2 Ratio |
| Theo vùng | Dư Nợ theo Vùng, Giải Ngân theo Vùng, Tỷ Lệ Đạt Kế Hoạch, NPL theo Vùng |
| Bộ đệm rủi ro | Dự Phòng Hiện Tại, Risk Multiple, Tỷ Lệ Bao Phủ Nợ Xấu, Tổng Rủi Ro Tín Dụng |

## Insight Chính

**1. Tăng trưởng ổn định nhưng chất lượng tín dụng đang đi xuống**

Tính đến 07/2025, dư nợ vay đạt 20.40T (tăng 8.97% so với 01/2024) và tổng tiền gửi đạt 18.85T (tăng 8.83%). Khách hàng hoạt động đạt 208.74M, vượt nhẹ kế hoạch (100.62%).

Tuy nhiên, NPL Ratio đã tăng lên 2.33%, vượt mục tiêu 1.89% đề ra từ đầu kỳ. Xu hướng dư nợ tín dụng và nợ xấu cho thấy chỉ số nợ xấu tăng nhanh hơn tốc độ tăng dư nợ trong giai đoạn gần đây, đặc biệt là đầu năm 2025.

**2. Bộ đệm rủi ro chưa đủ để bù đắp rủi ro tín dụng**

Dự phòng hiện tại của FinBank là 4.58T, trong khi tổng rủi ro tín dụng (NPL + Stage 2) lên đến 1.43T riêng phần dư nợ có vấn đề, và giá trị Stage 2 Balance lên tới 16.1T — cao gấp nhiều lần Provision Balance (4.6T) và NPL Balance (0.5T).

Tỷ lệ bao phủ nợ xấu (Provision Coverage) chỉ đạt 60%, thấp hơn đáng kể so với ngưỡng an toàn 100%. Điều này cho thấy nếu nợ xấu tiếp tục tăng, dự phòng hiện tại sẽ không đủ để hấp thụ rủi ro phát sinh.

**3. Rủi ro tín dụng phân bổ không đều giữa các vùng**

So sánh 3 vùng kinh doanh:

- **MN** dẫn đầu quy mô dư nợ (8.0T) và giải ngân (vượt kế hoạch 100.32%), đồng thời là vùng duy nhất đạt mục tiêu NPL (1.82% < 1.89%), dù tăng trưởng YoY thấp nhất (5.57%). Đây là vùng cân bằng tốt nhất giữa hiệu quả và kiểm soát rủi ro.
- **MB** có tốc độ tăng trưởng nhanh nhất (YoY 6.39%) nhưng NPL 2.02% đã vượt mục tiêu, cho thấy tăng trưởng đang đánh đổi bằng chất lượng tín dụng.
- **MT** là vùng rủi ro cao nhất: chưa đạt kế hoạch giải ngân (99.88%) và có NPL cao nhất hệ thống (2.30%), cần được ưu tiên xử lý.

**4. Nợ xấu phát sinh mới có tính chu kỳ và đang tăng tốc**

Nợ xấu phát sinh mới biến động theo chu kỳ trong năm, thường tăng mạnh vào đầu năm và giữa năm (tháng 1, tháng 7), sau đó giảm ở các tháng còn lại. Đáng chú ý, tháng 07/2025 ghi nhận nợ xấu phát sinh mới 50.32bn, cao hơn đáng kể so với nhiều tháng liền trước, đưa dư nợ xấu lũy kế lên 474.42bn (so với 358.78bn tại 01/2024).

**5. Nợ nhóm 2 (Stage 2) đang tích lũy áp lực nợ xấu tiềm ẩn**

Stage 2 Ratio tăng đều đặn qua từng tháng, từ 4.15% (01/2024) lên 4.69% (07/2025), trong khi NPL Ratio cũng tăng song song lên 2.33%. Xu hướng này cho thấy một lượng đáng kể dư nợ đang ở ranh giới chuyển nhóm, tiềm ẩn nguy cơ NPL tiếp tục tăng trong các kỳ tới nếu không được kiểm soát kịp thời.

## Kết Luận Và Đề Xuất

FinBank đang tăng trưởng ổn định về quy mô dư nợ và huy động, nhưng chất lượng tín dụng có dấu hiệu suy giảm rõ rệt, thể hiện qua NPL vượt mục tiêu, bộ đệm dự phòng chưa đủ và Stage 2 Ratio tăng liên tục.

**Đề xuất ưu tiên:**

- Tăng trích lập dự phòng để đưa tỷ lệ bao phủ nợ xấu về gần hoặc vượt ngưỡng an toàn 100%.
- Ưu tiên rà soát và kiểm soát chất lượng tín dụng tại vùng **MT** (NPL cao nhất, chưa đạt kế hoạch).
- Kiểm soát tốc độ tăng trưởng tín dụng tại **MB** song song với chất lượng, tránh đánh đổi rủi ro lấy tăng trưởng.
- Xây dựng cảnh báo sớm cho nhóm nợ Stage 2 để ngăn chuyển nhóm sang nợ xấu chính thức.
- Theo dõi sát các tháng có tính chu kỳ phát sinh nợ xấu cao (đầu năm, giữa năm) để chủ động phân bổ nguồn lực xử lý.
- Dùng mô hình vận hành của vùng **MN** (cân bằng tăng trưởng - rủi ro tốt nhất) làm tham chiếu để cải thiện MB và MT.

## Công cụ sử dụng

- Power BI Desktop
- DAX, Power Query
- Bookmarks & Buttons để điều hướng giữa các trang

## Cách sử dụng

1. Tải file `.pbix` về máy
2. Mở bằng Power BI Desktop
3. Dùng bộ lọc **Vùng** (MB/MN/MT) và **Thời gian** để xem chi tiết theo từng khu vực/giai đoạn
