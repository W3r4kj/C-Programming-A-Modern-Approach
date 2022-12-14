1. Điều chỉnh ví dụ ngăn xếp (stack.c) sao cho nó lưu các ký tự thay vì các số nguyên. Sau đó thêm hàm main 
và hỏi người dùng nhập vào một dãy các dấu ngoặc tròn hoặc ngoặc nhọn, sau đó thông báo các cặp ngoặc đã được 
đặt đúng hoặc chưa đúng:

Enter parentheses and/or braces : ((){}{()})
Parentheses/braces are nested properly

Gợi ý: Khi đọc các ký tự, lưu dấu mở ngoặc vào ngăn xếp. Khi đọc được một dấu đóng ngoặc thì lấy một ký tự 
từ ngăn xếp và kiểm tra xem nó có khớp với dấu vừa đọc được hay không (nếu không thì chứng tỏ các ngoặc 
lồng nhau bị đặt sai) Khi chương trình đọc được dấu xuống dòng, kiểm tra xem ngăn xếp rỗng hay không: 
Nếu rỗng thì chứng tỏ các cặp ngoặc được đặt đúng. Nếu không rỗng (hoặc ngăn xếp bị tràn dưới), thì chứng tỏ 
các cặp ngoặc lồng nhau bị đặt sai. Nếu ngăn xếp bị tràn trên thì in ra thông báo Tràn bộ nhớ và kết thúc 
chương trình.

2. Điều chỉnh chương trình poker.c - chuyển các mảng num_in_rank và num_in_suit vào trong hàm main, sau đó 
hàm main sẽ truyền các mảng này như các tham số cho read_cards và analyze_hand.

3. Xóa các mảng num_in_rank, num_in_suit, và card_exists khỏi poker.c, thay vào đó lưu các quân bài trong mảng 
5 x 2. Mỗi dòng của  mảng biểu diễn một quân bài. Ví dụ, nếu tên mảng là hand, thì hand[0][0] sẽ lưu hạng của 
quân bài đầu tiên và hand[0][1] sẽ lưu chất của quân bài đầu tiên.

4. Điều chỉnh chương trình poker.c sao cho nó nhận diện thêm một trường hợp - "royal flush" 
(ace, king, queen, jack, ten of the same suit). Bộ royal flush là bộ bài mạnh nhất.

5. Điều chỉnh chương trình poker.c sao cho nó cho nhận diện thêm một trường hợp - "ace-low"  
(ace,two, three, four, five).

6. Một số máy tính (ví dụ một số dòng máy của Hewlett-Packard) sử dụng hệ hậu tố để viết các biểu thức toán học
(RPN - Reverse Polish Notation). Trong hệ này, các toán tử được đặt sau các toán hạng thay vì ở giữa các 
toán hạng như trong hệ trung tố. Ví dụ, 1 + 2 phải được viết là 1 2 + theo RPN, và 1 + 2 * 3 cần được viết là 
1 2 3 * +. Có thể dễ dàng tính giá trị biểu thức RPN với ngăn xếp. Giải thuật yêu cầu đọc các toán tử và các 
toán hạng trong biểu thức từ trái sang phải, và thực hiện các thao tác sau:
  Khi gặp một toán hạng thì đưa nó vào ngăn xếp.
  Khi gặp một toán tử thì lấy các toán hạng của nó từ ngăn xếp, thực hiện phép toán trên các toán hạng, 
  và đưa kết quả ngược vào ngăn xếp.
Viết chương trình tính các biểu thức RPN. Các toán hạng là các số nguyên một chữ số. Các toán tử là 
+, -, *, /, và =. Khi gặp toán tử = chương trình in giá trị trên cùng của ngăn xếp, sau đó làm rỗng ngăn xếp 
và hỏi người dùng nhập vào một biểu thức khác. Tiến trình tiếp tục cho tới khi người dùng nhập một ký tự không 
phải toán tử hoặc toán hạng.

Enter an RPN expression: 1 2 3 * + =
Value of expression: 7
Enter an RPN expression: 5 8 * 4 9 - / =
Value of expression: -8
Enter an RPN expression: q
Nếu ngăn xếp bị tràn trên thì chương trình hiển thị thông báo Biểu thức quá phức tạp và dừng lại. Nếu tràn dưới 
(ví dụ khi tính biểu thức 1 2 + +), chương trình hiển thị thông báo Không đủ toán hạng trong biểu thức và 
dừng lại.
Gợi ý: Đưa mã nguồn stack.c vào chương trình. Đọc các toán tử và toán hạng như những ký tự (có thể sử dụng 
scanf(" %c", &ch)).

7. Viết chương trình hỏi người dùng nhập vào một số và hiển thị số đó bằng các ký tự mô phỏng màn hình 7 đoạn.

Enter a number: 491-9014
     _       _   _
|_| |_|   | |_| | |   | |_|
  |  _|   |  _| |_|   |   |
Bỏ qua các ký tự không phải là chữ số. Viết chương trình sao cho số chữ số tối đa được kiểm soát bởi macro 
tên là MAX_DIGITS, có giá trị bằng 10. Nếu số được nhập vào chứa nhiều chữ số hơn, thì các chữ số vượt giới hạn
sẽ bị bỏ qua. Gợi ý: Sử dụng hai mảng bên ngoài. hai mảng bên ngoài. Một là mảng phân đoạn (xem Bài tập 6 
trong Chương 8), lưu trữ dữ liệu đại diện cho sự tương ứng giữa các chữ số và phân đoạn. Mảng khác, các chữ số, 
sẽ là một mảng các ký tự có 4 hàng (vì mỗi chữ số được phân đoạn cao 4 kí tự) và MAX_DIGITS * 4 cột 
(chữ số rộng ba ký tự, nhưng cần một khoảng trống giữa các chữ số để đọc). Viết chương trình của bạn dưới 
dạng bốn chức năng: Main, clear_digits_array, process_digit, và print_digits_array. Đây là nguyên mẫu 
của 3 hàm cuối cùng:
void clear_digits_array(void);
void process_digit(int digit, int position);
void print_digits_array(void);
Hàm clear_digits_array sẽ khởi tạo mảng digits bằng những khoảng trắng, hàm process_digit sẽ lưu biểu diễn
7 đoạn của chữ số vào các vị trí thích hợp trong mảng digits (các vị trí trong khoảng từ 0 tới MAX_DIGITS - 1). 
print_digits_array sẽ hiển thị các dòng của mảng digits, mỗi dòng của mảng trên một dòng màn hình, để có đầu ra 
tương tự như trong ví dụ.