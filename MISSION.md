# Mission: CAN Classic trên STM32F103

## Why
Tự xây dựng giao tiếp CAN Classic bằng thanh ghi trên STM32F103CBT6, hiểu được dữ liệu đi từ ngoại vi bxCAN qua module WCMCU-230 ra cặp dây CANH/CANL, và có khả năng tự tìm lỗi trên bus thật.

## Success looks like
- Giải thích đúng vai trò riêng của bxCAN, transceiver và đường bus vi sai.
- Tự tính bit timing từ clock APB1 cho các tốc độ CAN thông dụng.
- Tự cấu hình GPIO, bxCAN, filter, mailbox, FIFO và interrupt bằng thanh ghi.
- Truyền nhận một CAN data frame ổn định và chẩn đoán được lỗi ACK, bit timing và termination.

## Constraints
- Học bằng tiếng Việt, giải thích từ nguyên lý rồi mới viết code.
- Ưu tiên code thanh ghi; HAL chỉ dùng để đối chiếu khi thật sự hữu ích.
- Phần cứng hiện tại: STM32F103CBT6 WeAct Studio và module WCMCU-230 dùng transceiver họ SN65HVD230.
- Clock dự kiến của project là 8 MHz; phải xác nhận PCLK1 trước bài bit timing.
- Không sửa source project KeilC khi chưa được yêu cầu rõ ràng.

## Out of scope
- CAN FD, CAN XL và các giao thức tầng cao như CANopen/J1939 trong giai đoạn đầu.
- Thiết kế phần cứng CAN chịu nhiễu cấp ô tô hoặc công nghiệp hoàn chỉnh.
