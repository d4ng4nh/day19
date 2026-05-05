PITCH MEMO — CodeCompass

1. THE PROBLEM (1-2 câu)
Các công ty công nghệ đang đốt trung bình $10,000 năng suất cho mỗi nhân sự mới chỉ để họ ngồi "bơi" trong codebase lạ. GitHub Copilot không giải quyết được vấn đề này vì nó chỉ là công cụ gợi ý code cục bộ (local context), không thể giúp developer hiểu được bức tranh kiến trúc toàn cảnh của các hệ thống khổng lồ.

2. THE INSIGHT (1 câu)
Nút thắt thực sự trong việc onboard không phải là "đọc code", mà là hiểu những "quyết định thiết kế ngầm" (invisible decisions) và context lịch sử; các developer không cần một cuốn từ điển giải thích syntax, họ cần một hệ thống "GPS kiến trúc" (Architectural GPS).

3. THE SOLUTION & DIFFERENTIATOR (3 câu)
- CodeCompass là hệ thống Architectural GPS tự động biến bất kỳ codebase phức tạp nào thành Knowledge Graph trực quan và lộ trình đọc hiểu (Reading Path).
- **Differentiator:** Nếu chỉ ném hàng vạn files vào LLM, AI sẽ bị ảo giác (hallucinate) và rất chậm. CodeCompass sở hữu một *parsing engine độc quyền*, nén toàn bộ codebase thành semantic graph để định tuyến chính xác cho LLM, giúp loại bỏ hoàn toàn hallucination và đạt thời gian phản hồi (TTFB) dưới 3 giây—điều mà RAG truyền thống hay GitHub chưa làm được.
- Sản phẩm được thiết kế để tích hợp sâu vào enterprise workflow (Jira, Confluence) nhằm gắn kết trực tiếp dòng code với mục tiêu kinh doanh thực tế.

4. WHY NOW (1-2 câu)
Khi các hệ thống phần mềm ngày càng phình to và các doanh nghiệp nhận ra giới hạn ảo giác của Large Context Models, đây là thời điểm vàng cho một kiến trúc lai (Hybrid Architecture) kết hợp phân tích code truyền thống và LLM để giải quyết bài toán context một cách chính xác và kinh tế.

5. TRACTION / PROOF (số cụ thể)
- Đã hoàn thiện core engine tích hợp React Flow và pipeline lai (Parser + LLM).
- Pilot thành công trên 50 early-adopter developers từ các công ty outsource lớn.
- **Metrics:** Giảm "Time-to-first-PR" (thời gian push commit đầu tiên) từ 14 ngày xuống chỉ còn 3 ngày, đồng thời giảm 60% số giờ senior developers phải dành ra để support người mới.

6. THE ASK (1-2 câu)
Chúng tôi đang gọi $500K vòng Seed để xây dựng các deep integrations trực tiếp vào Enterprise CI/CD pipelines (GitHub Actions, GitLab CI), nhằm tạo lợi thế độc quyền và đạt mốc 10,000 daily active developers trong 12 tháng tới.