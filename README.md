#  Xây dựng Dashboard phân tích dữ liệu Nhân Sự & Vận Hành (HR Turnover & Operations Analytics)

## 1. TỔNG QUAN (OVERVIEW)

* **Loại Dashboard:** Operational & Analytical Dashboard (Báo cáo Vận hành & Phân tích chuyên sâu).
* **Mục đích sử dụng:** Theo dõi tình hình biến động nhân sự (nghỉ việc, tuyển mới), đánh giá mức độ cam kết và kỷ luật của nhân viên, áp lực vận hành đối với nhân viên từ đó tối ưu hóa các quyết định quản trị nhân sự (HRM).
* **Đối tượng sử dụng:** Giám đốc Nhân sự (HR Manager), Trưởng phòng ban (Department Heads), Ban Giám đốc (C-level), Quản lý chuỗi cửa hảng (Chain Store Manager).
* **Các câu hỏi nghiệp vụ cần giải quyết:**
    1. Tỷ lệ biến động nhân sự (Turnover Rate) hiện tại là bao nhiêu? Số lượng ra/vào biến động qua các tháng như thế nào?
    2. Lý do nào khiến nhân sự nghỉ việc?
    3. Thời gian mà nhân sự cống hiến cho công ty là bao lâu?
    4. Tính kỷ luật của các cửa hàng đang ở mức nào? Đơn vị nào có tỷ lệ tuân thủ kỷ luật tốt?
    5. Áp lực vận hàng cửa từng cửa hàng đối với nhân viên?
* **Các chỉ số đo lường (KPIs):**
    * *Opening/Closing Headcount:* Tổng số nhân sự đầu kỳ và cuối kỳ.
    * *Turnover Rate (%):* Tỷ lệ nghỉ việc so với nhân sự trung bình.
    * *Punctuality Rate Rate (%):* Tỷ lệ tuân thủ giờ giấc.
    * *Late/Early Rate (%):* Tỷ lệ lượt đi muộn/đi sớm.
    * *Average Monthly Working Hours:* Mức lương trung bình của mỗi nhân viên được nhận.
    * *Salary Budget*: Quỹ lương
* **Tính năng nổi bật:**
    * *Tooltip*: Cho phép xem Thông tin cửa hàng khi trỏ chuột vào bong bóng cửa hàng trên bản đồ.
    * *Drillthrough*: Đi sâu vào phân tích chi tiết lý do nghỉ của nhân sự theo từng phòng ban.
    * *Dynamic titles*: Tiêu để tự động chuyển đổi theo các kỳ báo cáo.
    * *Bookmark*: Thay đổi Dashboad theo như cầu xem (Nhân Sự - Vận Hành).
    * *Filed parameters*: Thay đổi biểu đồ theo chỉ số mong muốn.
   
---

## 2. INSIGHTS TỪ DỮ LIỆU (KEY FINDINGS)

**Insight 1: Tốc độ gia tăng tỷ lệ nghỉ việc và Sự thất thoát nhân lực chất lượng**
* **Phân tích:** Số liệu thực tế: Tỷ lệ nghỉ việc của công ty đang có xu hướng tăng tốc rõ rệt qua 3 năm: 21.88% (2016) --> 29.69% (2017) ----> 37.96% (2018). Đáng chú ý, lý do nghỉ việc lớn nhất có sự chuyển dịch: Năm 2016 đa phần nghỉ vì "Không phù hợp". Nhưng đến năm 2018, số ca nghỉ tăng mạnh lên 26 người, và nguyên nhân hàng đầu lại là "Tuyển dụng bởi khách hàng" (7 ca) và "Yêu cầu tăng lương/Thay đổi định hướng".
* **Giả thuyết:** Chất lượng tuyển dụng đầu vào đã được cải thiện (nhân sự làm được việc thay vì nghỉ do yếu kém - không phù hợp), nhưng hệ thống đãi ngộ và chính sách giữ chân (Retention Policy) lại đang bị "đóng băng", không theo kịp giá trị thị trường của chính nhân viên đó.
*  **Kết nối:** Nguyên nhân: Lớp nhân sự được tuyển ồ ạt từ đợt mở rộng quy mô đã tích luỹ đủ kinh nghiệm về mặt chuyên môn. Tuy nhiên, cơ cấu tổ chức hiện tại có thể đang thiếu các vị trí Quản lý bậc trung (Middle Management), Trưởng nhóm, hoặc Cửa hàng trưởng để họ có cơ hội thăng tiến lên. --> Hệ quả: Thay vì thải lọc những người mới thử việc thất bại (ít thiệt hại), công ty đang để tuột mất những nhân sự ở thời kỳ đỉnh cao năng suất (ROI cao nhất) có kinh nghiệm với công việc. Không có lộ trình thăng tiên, vị trí mới trong 2 năm dẫn đến việc nhân sự đồng loạt rời đi để tìm bến đỗ mới có chức danh tốt hơn, để lại một lỗ hổng vận hành cực kỳ lớn và đột ngột cho hệ thống cửa hàng.

**Insight 2: Nghịch lý "Thâm niên" – Cảnh báo nhân sự ở mốc 1.5 đến 2 năm**
* **Phân tích:** Dù số lượng người nghỉ tăng lên, nhưng thâm niên trung bình của những người rời đi trong năm 2017-2018 lại dài hơn hẳn: dao động từ 638 đến 692 ngày (tương đương gần 2 năm) so với mức chỉ khoảng 500 ngày của năm 2016.
* **Giả thuyết & Hệ quả:** Doanh nghiệp đang gặp phải nút thắt trong lộ trình thăng tiến. Mốc 2 năm chính là "điểm tới hạn" để một nhân sự lâu năm kỳ vọng một bước nhảy vọt về chức vụ hoặc thu nhập.
*  **Kết nối:** Nguyên nhân: Công ty đã đẩy mạnh mở rộng quy mô (tuyển thêm hơn 50 người trong 2 năm 2017-2018) nhằm thúc đẩy doanh thu, nhưng có thể đã bỏ quên việc cập nhật khung năng lực và nới rộng dải lương nội bộ. --> Hệ quả: Nhân viên được rèn luyện thực tế nên trở nên "có giá" hơn. Việc chảy máu chất xám tăng vọt vào 2018 minh chứng cho việc công ty đang trở thành bệ phóng đào tạo miễn phí. Điều đang quan ngại, khi sales cứng bị chính tệp khách ruột "săn" đi, công ty không chỉ tốn chi phí tuyển mới mà còn đối mặt với rủi ro mất luôn tệp khách hàng do nhân sự đó quản lý.

**Insight 3: "Sự bình đẳng của sự kiệt sức và Nghịch lý đánh đổi thu nhập"**
* **Phân tích:** Hệ số tương quan (Pearson Correlation) giữa Thời gian làm trung bình và Số ca đi muộn lên tới 0.996 (mức gần như tuyệt đối). Nghĩa là, nhân sự không tự nhiên đi muộn, mà cứ hễ tổng thời gian gánh ca tăng lên, số ca đi muộn chắc chắn sẽ tăng theo tỷ lệ thuận. Các nhân viên Phòng Bán Hàng có mức lương trung bình thấp nhất (khoảng 8 triệu VNĐ/tháng), nhưng họ lại có thời gian làm việc trung bình lên tới ~174.7 giờ/tháng (tương đương gánh ~44 ca làm/tháng) và bị ghi nhận đi muộn ~23.5 ca/tháng. Điều kinh ngạc là các phòng ban cấp cao như Phòng Dịch Vụ (lương ~14 triệu), Quản Lý (lương ~9.3 triệu) và thậm chí là Founder (lương 40 triệu) cũng có mức thời gian làm việc y hệt (~174.5 - 174.8 giờ/tháng) và số ca đi muộn cũng tương đương (23.1 - 23.8 ca/tháng). "Chỉ số chịu đựng" (Late-to-Hours Ratio) của các phòng ban tương đương nhau chứng tỏ nguyên nhân nằm ở hệ thông phân ca, không hoàn toàn thuộc về lỗi của nhân sự. 
* **Giả thuyết:** Việc đi muộn ở công ty này hoàn toàn là hệ quả vật lý của việc lên lịch làm việc quá tải – trung bình 1 người phải gánh 44.3 ca một tháng (khoảng gần 2 ca/ngày), chứ không xuất phát từ thái độ làm việc kém.
*  **Kết nối:** Nguyên nhân: Công ty đang áp dụng một khung thời gian làm việc "cào bằng" cho toàn bộ nhân sự Full-time, không phân biệt khối Back-office (Quản lý/Dịch vụ) hay Front-office (Bán hàng). --> Hệ quả: Khối Phòng Bán Hàng đang chịu áp lực tồi tệ nhất. Dù cường độ bào mòn sức khỏe (174.7 giờ) và số ca đi muộn (23.5 ca) ngang bằng với cấp Quản lý hay Founder, nhưng lương của họ chỉ bằng 1/5. Nếu bộ phận HR dùng biến số "Số ca đi muộn" này để phạt tiền cứng (ví dụ phạt 50k/lần muộn), thì nhân viên bán hàng sẽ bị trừ mất một tỷ trọng cực lớn trong quỹ lương 8 triệu ít ỏi của họ, dẫn tới bất mãn.
---

## 3. QUY TRÌNH XÂY DỰNG DASHBOARD

1. **Khảo sát & Xác định mục tiêu:** Khảo sát các HR, xác định loại Dashboard cần xây dựng - KPI cần có - vai trò, phác thảo mockup - demo của trang Dashboard.
2. **Kiểm tra & Làm sạch dữ liệu (Power Query):** Xử lý lỗi logic ('Ngày Bắt Đầu' > 'Ngày Kết Thúc') tạo ra 2 cột mới 'Ngày Vào Làm' và 'Ngày Kết Thúc' chuẩn hoá, gán giá trị "Chuyển Công Tác" trường Trạng Thái cho Missing Value trường Lý Do Nghỉ vì Trạng Thái "Chuyển Công Tác" đều bị Missing lý do nghỉ, tách dữ liệu ca làm việc để lấy dữ liệu giờ bắt đầu ca và giờ kết thúc ca, dùng điều kiện để tạo cột 'Is_Late' đánh dấy nhân sự đến muộn gán là 1 ngược lại nhận giá trị là 0 dựa trên thời gian bắt đầu ca việc < thời gian chấm công, tương tự tạo cột 'Is_Early' đánh dấu nhân sự về sớm gán giá trị là 1 và ngược lại. Chỉnh sửa định dạng các cột cho phù hợp. 
3. **Xây dựng Mô hình dữ liệu (Data Modeling):** Thiết lập Star Schema, dùng bảng 'Dim_Date' xử lý các bài toán Time Intelligence. 
4. **Trực quan hóa dữ liệu (Visualization):**  Xây dựng luồng phân tích Top-down bằng Drill-through.
5. **Trích xuất Insights:** 
