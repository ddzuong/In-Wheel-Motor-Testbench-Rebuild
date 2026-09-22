# CAN Classic trên STM32F103 Resources

## Knowledge

- [ST RM0008 - STM32F10xxx reference manual](https://www.st.com/resource/en/reference_manual/rm0008-stm32f103xx-advanced-armbased-32bit-mcus-stmicroelectronics.pdf)
  Nguồn chính cho kiến trúc bxCAN, thanh ghi, mailbox, FIFO, filter, interrupt và bit timing của STM32F103. Dùng từ bài cấu hình bxCAN trở đi.
- [TI SN65HVD230 datasheet](https://www.ti.com/lit/ds/symlink/sn65hvd230.pdf)
  Nguồn chính cho lớp vật lý của WCMCU-230: nguồn 3.3 V, chân D/R, CANH/CANL, chế độ của chân RS và đặc tính điện.
- [Bosch CAN Protocols - CAN Specification 2.0B](https://www.bosch-semiconductors.com/products/ip-modules/can-protocols/)
  Nguồn gốc cho frame, arbitration, ACK, error handling và bit timing của CAN Classic.
- [ST STM32F103 documentation](https://www.st.com/en/microcontrollers-microprocessors/stm32f103/documentation.html)
  Trang tập hợp datasheet, reference manual và errata chính thức cho đúng họ STM32F103.

## Wisdom (Communities)

- [STMicroelectronics Community](https://community.st.com/)
  Dùng để đối chiếu các tình huống bxCAN thực tế; luôn kiểm tra lại kết luận bằng RM0008 hoặc errata.
- [CAN in Automation - CAN knowledge](https://www.can-cia.org/can-knowledge/)
  Cộng đồng chuyên ngành CAN; hữu ích khi tiến tới CANopen, topology và thực hành mạng CAN.

## Gaps

- Chưa xác nhận người học có một hay hai node CAN, và module WCMCU-230 có gắn sẵn điện trở 120 ohm hay không.
