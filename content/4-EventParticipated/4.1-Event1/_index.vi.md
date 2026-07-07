---
title: "Event 1: FCAJ Community Day"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

{{% notice info %}}
💡 **Tổng quan:** Buổi sinh hoạt cộng đồng AWS FCAJ Community Day là chuỗi 6 phiên chia sẻ chuyên sâu từ các chuyên gia đầu ngành. Nội dung tập trung vào tư duy dịch chuyển từ kỹ thuật thuần túy sang bài toán kinh doanh, tối ưu hóa kiến trúc Cloud/CDN và chiến lược xây dựng Multi-Agent bảo mật trong môi trường doanh nghiệp lớn (Enterprise).
{{% /notice %}}

# Bài thu hoạch “FCAJ Community Day 2026”

### Mục Đích Của Sự Kiện

- Định hình tư duy (Mindset) và kỹ năng thực chiến cho kỹ sư công nghệ trong kỷ nguyên trí tuệ nhân tạo.
- Khai thác các phương pháp quản lý ngữ cảnh (Context Engineering) và kiến trúc đa tác tử (Multi-Agent System).
- Giới thiệu các giải pháp tối ưu hóa chi phí vận hành và nâng cao năng lực bảo mật hạ tầng Cloud/CDN.
- Đúc kết kinh nghiệm từ các dự án thực tế, các cuộc thi Hackathon và quy trình triển khai sản phẩm lên môi trường Production.

### Danh Sách Diễn Giả

- **Anh Nguyễn Gia Hưng** - Solution Architect tại AWS Việt Nam & Founder FCAJ.
- **Anh Tịnh Trương** - Platform Engineer tại Gotamic.
- **Bạn Hải Anh** - Engineer tại Pacific Việt Nam (AWS Speaker tại Singapore & Silicon Valley).
- **Anh Nguyễn Hữu Thịnh** - DevOps Engineer.
- **Bạn Uyển & Bạn Thảo** - Kỹ sư phần mềm tại Gotamic (Winner Hackathon).
- **Chuyên gia Công nghệ** - Đại diện Khối Công nghệ & Khối Quản trị Rủi ro từ VPBank.

---

### Nội Dung Nổi Bật

#### 1. Nghịch Lý AI Và Chuyển Dịch Thị Trường Lao Động (Diễn giả: Nguyễn Gia Hưng)
- **Hiệu ứng giá rẻ của AI:** AI đang tối ưu hóa chi phí và thời gian viết mã (coding), khiến việc tạo ra phần mềm trở nên dễ dàng hơn. Hệ quả là số lượng ứng dụng/sản phẩm công nghệ sẽ bùng nổ trong tương lai gần.
- **Sự trỗi dậy của luồng công việc mới:** Thị trường sẽ dịch chuyển mạnh mẽ sang nhu cầu tuyển dụng các vị trí vận hành hệ thống phức tạp (*Platform Engineering*) và kỹ sư chuyên sửa chữa, tối ưu hóa (*Fixing Software Engineering*) để đưa các sản phẩm MVP (do người không chuyên tự build bằng AI) lên môi trường Production.
- **Yêu cầu khắt khe của doanh nghiệp:** Ứng viên không chỉ dựa vào bằng cấp mà phải có năng lực giải quyết nghiệp vụ thực tế, có sản phẩm Demo hoàn chỉnh thay vì các bài tập lý thuyết.

#### 2. Kỹ Nghệ Ngữ Cảnh Và Nền Tảng Tự Phục Vụ (Diễn giả: Tịnh Trương)
- **Tư duy Platform Engineering:** Thay vì DevOps xử lý thủ công từng yêu cầu (Ticket), Platform Engineer tập trung xây dựng nền tảng IDP (Internal Developer Platform) để các nhà phát triển tự cấp phát tài nguyên trong ranh giới an toàn.
- **Tối ưu hóa Context cho AI:** Phân tích lỗi "Chat lan man" làm phân rã bộ nhớ của LLM. Phương pháp cô đọng ngữ cảnh bằng cách chỉ cung cấp mục tiêu (Goal), vai trò (Role) và các quy tắc (Blueprints) đặc thù nội bộ mà AI không thể tự tìm kiếm trên Internet.

#### 3. Sức Mạnh Hành Động Của Trợ Lý Thông Minh (Diễn giả: Hải Anh)
- **Từ LLM truyền thống đến Agent:** Khắc phục nhược điểm "chỉ biết nói, không biết làm" của AI cũ. Hệ thống Agent sử dụng LLM làm bộ não kết hợp với các công cụ hành động (Action/MCP) để tương tác trực tiếp với các hệ thống doanh nghiệp (Jira, Gmail, Teams).
- **Ứng dụng Amazon Q:** Demo thực tế cách tích hợp Amazon Q Business và Q QuickSight để người dùng không biết về BI vẫn có thể import dữ liệu Excel, tự động tạo Dashboard phân tích và xuất biên bản họp tự động gửi qua Email.

#### 4. Chiến Lược Kiểm Soát Chi Phí CDN Mới (Diễn giả: Nguyễn Hữu Thịnh)
- **Rủi ro hóa đơn từ Pay-as-you-go:** Mô hình tính tiền theo lưu lượng thông thường dễ khiến doanh nghiệp phá sản khi bị tấn công DDoS hoặc hệ thống tăng trưởng đột biến (Build Spike).
- **Cơ chế Flat-rate Pricing trên CloudFront:** Giải pháp đóng gói chi phí cố định tích hợp sẵn WAF và Route 53. Khi vượt ngưỡng usage, hệ thống chỉ bóp băng thông (thay vì tính thêm tiền), bảo vệ an toàn tài chính cho doanh nghiệp.
- **Bảo mật nâng cao:** Ứng dụng mTLS (Mutual TLS) yêu cầu xác thực hai chiều và tính năng VPC Origin tạo đường hầm ẩn hoàn toàn máy chủ gốc khỏi mạng Internet công cộng.

#### 5. Mô Hình Multi-Agent Thực Chiến Từ Hackathon (Diễn giả: Uyển & Thảo)
- **Case study dự án UTMorpho:** Giải quyết bài toán chỉnh sửa giao diện (UI) bằng AI mà không cần sinh lại toàn bộ mã nguồn để tiết kiệm Token.
- **Kiến trúc phối hợp:** Chia nhỏ công việc cho 3 Agent chuyên biệt (Vision Agent phân tích ảnh -> Layout Agent xử lý CSS -> Design Agent tối ưu hóa cấu trúc) giúp tăng tốc độ sinh mã và cho phép người dùng tương tác kéo thả trực tiếp trên UI.

#### 6. Hệ Thống Đa Tác Tử Cấp Doanh Nghiệp (Diễn giả: Chuyên gia VPBank)
- **Tính bất định của LLM trên Production:** Phân tích sâu về lý do tại sao `Temperature = 0` kết quả vẫn bị sai lệch do cơ chế tối ưu hóa phần cứng (Parallel GPU Computing) và gộp Prom của các Provider. Chiến lược giảm thiểu bằng cách tự host hoặc bọc tầng kiểm soát (Downstream handling).
- **Bài toán Tín dụng Startup:** Ứng dụng hệ thống Multi-Agent để bốc tách tri thức chuyên gia (Context Engineering), phân tích dữ liệu đa chiều (Thị trường Tam/Sam/Som, dữ liệu Founder) để chấm điểm tín dụng thay thế cho báo cáo tài chính truyền thống.
- **Ranh giới an toàn (Guardrails):** Chống Prompt Injection, rà soát Standard Coding khi dùng AI và nhấn mạnh tính pháp lý: Con người luôn là bên cuối cùng chịu trách nhiệm trước cơ quan quản lý (Ngân hàng Nhà nước), AI chỉ đóng vai trò hỗ trợ.

---

### Những Gì Học Được

#### Tư Duy Thiết Kế & Nghiệp Vụ
- **Tư duy hướng sản phẩm (Product-first):** Công nghệ hay AI tinh vi đến đâu cũng chỉ là công cụ, điều cốt lõi là sản phẩm phải giải quyết được bài toán cụ thể và mang lại giá trị cho người dùng cuối.
- **Knowledge Transfer & Context Engineering:** Hiểu rằng không phải cứ "nhồi nhét" toàn bộ tài liệu vào AI là tốt (Garbage in, Garbage out). Việc hiện đại hóa ứng dụng cần có sự chắt lọc tinh túy từ các chuyên gia nghiệp vụ để định hình các Guardrails (rào chắn) an toàn.
- **Kiến trúc cô lập trách nhiệm:** Thiết kế hệ thống Multi-Agent tương tự như tư duy Solution Architect. Mỗi Agent chỉ nên đảm nhận một vai trò chuyên biệt (Specialized Expertise) để tối ưu cửa sổ ngữ cảnh (Context Window) và tránh hiện tượng AI bị quá tải hoặc phản hồi sai lệch.

#### Kiến Trúc Kỹ Thuật & Vận Hành
- **Làm chủ sự bất định của AI:** Ý thức được bản chất toán học của LLM là mô hình xác suất. Do đó, các hệ thống hạ tầng nhận dữ liệu phía sau (downstream services) luôn phải được thiết kế để xử lý các tình huống AI trả về sai format hoặc lỗi cấu trúc (Production-ready).
- **An toàn thông tin doanh nghiệp:** Nâng cao nhận thức về các vector tấn công mới (MCP attack vector, Prompt Injection) và tầm quan trọng của việc bảo mật dữ liệu nội bộ bằng các giải pháp Cloud Native (VPC Origin, mTLS, Token Filtering).
- **Hạ tầng tự động hóa:** Hiểu sâu hơn về vai trò của Infrastructure as Code (IaC) thông qua Terraform để quản lý và tái cấu trúc hạ tầng Cloud một cách minh bạch, có lưu vết lịch sử (Reproduce).

---

### Ứng Dụng Vào Công Việc

- **Ứng dụng AI Mindset vào Workflow:** Triển khai quy tắc phân chia Session chat với AI một cách khoa học; cấu hình rõ ràng Role, Goal và Style của dự án trước khi truy vấn để nâng cao chất lượng code đầu ra.
- **Tái cấu trúc Prompt và tham số:** Áp dụng bài học thực tế về việc điều chỉnh `Temperature` linh hoạt (sử dụng 0.1 thay vì 0 cho các tác vụ cần tính nhất quán nhưng tránh lặp từ) và nghiên cứu tích hợp JSON Mode khi làm việc với API của LLM.
- **Thử nghiệm kiến trúc Agent cơ bản:** Tìm hiểu và xây dựng thử nghiệm các con Bot nội bộ có sử dụng Action/Function Calling (các cánh tay nối dài) để tự động hóa một số tác vụ lặp đi lặp lại như tóm tắt log hệ thống hoặc tạo báo cáo tự động.
- **Tuân thủ quy trình Security chuẩn doanh nghiệp:** Thực hiện nghiêm túc việc bảo mật API Key, cấu hình Security Group chặt chẽ và luôn rà soát thủ công (Review) mã nguồn do AI tạo ra trước khi Commit, tuyệt đối không "Copy-Paste" mù quáng để tránh phá vỡ Coding Standard của đội ngũ.

---

### Trải nghiệm trong event

Tham gia **FCAJ Community Day** mang lại một trải nghiệm công nghệ bùng nổ, giúp kết nối khoảng cách giữa lý thuyết học thuật và thực trạng khắc nghiệt của môi trường doanh nghiệp lớn.

#### Tiếp cận góc nhìn thực chiến từ chuyên gia
- Không đi vào các slide lý thuyết suông, các diễn giả từ AWS, Gotamic và VPBank đã phơi bày những "nỗi đau" thực tế như rủi ro nợ hóa đơn Cloud, lỗi ngớ ngẩn do lạm dụng AI, hay áp lực pháp lý trước Ngân hàng Nhà nước. Điều này giúp tôi kéo bản thân về thực tại và hiểu rõ doanh nghiệp thực sự cần gì ở một kỹ sư.

#### Trải nghiệm trực quan qua các phiên Demo & Case Study
- Các phiên Demo sống động về Amazon Q, quy trình kéo thả trực tiếp trên giao diện do AI tạo ra từ Hackathon, và các công thức tính toán chỉ số ROI (Return on Investment) giúp tôi hình dung rõ nét cách một dự án AI được khai sinh, kiểm thử và chứng minh giá trị với ban lãnh đạo.

#### Giao lưu và kết nối cộng đồng
- Bầu không khí sôi động tại hội trường và sự kết nối với các anh em ở tầng 36 đã truyền tải đúng tinh thần của FCAJ: không chỉ đi nghe hội thảo mà là nơi để truyền cảm hứng, chủ động bắt chuyện và tìm kiếm những người đồng đội, những đối tác tiềm năng trong tương lai.

#### Khơi dậy tinh thần tự học và cọ xát
- Câu chuyện vượt qua giới hạn của nhóm bạn trẻ tham gia Hackathon hay những kỹ sư trẻ trình bày tại Silicon Valley đã kích thích mạnh mẽ tinh thần dấn thân. Tôi nhận ra mình cần phải chấm dứt sự trì hoãn, liên tục cập nhật các công nghệ mới (như mTLS, IaC Terraform, MCP) và sẵn sàng tham gia các sân chơi lớn để rèn luyện sự tự tin trước đám đông.

#### Một số hình ảnh khi tham gia sự kiện
(/images/4-Event/4.1-Event1/event1-1.png)
(/images/4-Event/4.1-Event1/event1-2.png)

> Sự kiện là một bước đệm hoàn hảo về mặt tư duy, giúp tôi hiểu rằng một kỹ sư giỏi trong thời đại GenAI không chỉ là người biết viết code, mà phải là người biết dùng công nghệ để giải quyết bài toán kinh doanh một cách an toàn, tiết kiệm và đáng tin cậy.