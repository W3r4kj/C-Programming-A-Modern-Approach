1. Viết một chương trình tìm số lớn nhất trong một dãy số được nhập bởi người dùng. 
Chương trình phải nhắc người dùng nhập từng số một. Khi người dùng nhập 0 hoặc một số âm, 
chương trình phải hiển thị số không âm lớn nhất đã được nhập:
Enter a number: 60
Enter a number: 38.3
Enter a number: 4.89
Enter a number: 100.62
Enter a number: 75.2295
Enter a number: 0
The largest number entered was 100.62
Lưu ý rằng các số không nhất thiết phải là số nguyên. 
2. Viết một chương trình yêu cầu người dùng nhập 2 số nguyên, sau đó tính và hiển thị ước chung lớn nhất:
Enter two integers: 12 28
Greatest common divisor: 4
Gợi ý: Thuật toán cổ điển để tính ước chung lớn nhất được biết đến là thuật toán của Euclid, 
theo cách sau: m và n là các biến chứa 2 số. Nếu n bằng 0, sau đó dừng lại: m chứa ước chung lớn nhất. 
Mặt khác, tính phần dư khi m chia cho n. Sao chép n vào m và sao chép phần dư vào n. 
Sau đó lặp lại quá trình đó cho đến khi n = 0.
3. Viết một chương trình yêu cầu người dùng nhập một phân số, sau đó tìm phân số tối giản:
Enter a fraction: 6/12
In lowest terms: 1/2
Gợi ý : Để tìm phân số tối giản, đầu tiên tính ước chung lớn nhất của tử số và mẫu số. 
Sau đó chia cả 2 cho ước chung lớn nhất
4. Thêm một vòng lặp cho chương trình broker.c của phần 5.2 để người dùng có thể nhập hơn 1 
giao dịch và chương trình sẽ tính hoa hồng của mỗi giao dịch. Chương trình nên dừng khi người dùng nhập 0 
như giá trị giao dịch:
Enter value of trade: 30000
Commission: $166.00

Enter value of trade: 20000
Commission: $144.00

Enter value of trade: 0

5. Bài 1 chương 4 yêu cầu bạn viết chương trình hiển thị số có 2 chữ số theo thứ tự đảo ngược. Hãy khái quát 
chương trình đó sao cho người dùng có thể nhập vào số có độ dài tùy ý: một, hai, ba hoặc nhiều hơn.
Gợi ý: Lặp chia số cho 10 và dừng khi chạm 0.
6. Viết chương trình hỏi người dùng nhập một số n, sau đó in các giá trị bình phương chẵn giữa 1 và n. 
Ví dụ, nếu người dùng nhập 100 thì chương trình phải in ra:
4
16
36
64
100

7. Bố cục lại chương trình square3.c sao cho vòng lặp for khởi tạo i, kiểm tra i, và tăng i. 
Không viết lại chương trình và không sử dụng phép nhân nào.
8. Viết chương trình in lịch cho một tháng. Người dùng nhập số ngày trong tháng và ngày trong tuần của ngày bắt đầu tháng.
Ví dụ:
Enter number of days in month: 31
Enter starting day of week (1 = Sun, 7 = Sat): 3
         1   2   3   4   5
 6   7   8   9  10  11  12
13  14  15  16  17  18  19
20  21  22  23  24  25  26
27  28  29  30  31
Gợi ý: Sử dụng một vòng lặp để duyệt các giá trị từ 1 tới n, trong đó n là số ngày trong tháng, 
in ra các giá trị của i. Trong vòng lặp kiểm tra xem i có phải ngày cuối cùng trong tuần hay không; 
nếu có thì in một ký tự xuống dòng.
9. Bài 8 trong chương 2 yêu cầu bạn viết chương trình tính dư nợ còn lại sau khi thanh toán hàng tháng lần một, 
lần hai, và lần ba. Điều chỉnh chương trình sao cho nó hỏi người dùng nhập số lần thanh toán và hiển thị dư nợ 
còn lại sau mỗi lần thanh toán.

10. Bài 9 chương 5 yêu cầu bạn xác định ngày sớm hơn trong hai ngày được nhập vào. 
Hãy khái quát hóa chương trình sao cho người dùng có thể nhập vào số ngày bất kỳ. Người dùng nhập 0/0/0 để dừng.

Ví dụ:
Enter a date (mm/dd/yy): 3/6/08
Enter a date (mm/dd/yy): 5/17/07
Enter a date (mm/dd/yy): 6/3/07
Enter a date (mm/dd/yy): 0/0/0
5/17/07 is the earliest date.

11. Giá trị của hằng số toán học e có thể được biểu diễn như một dãy vô hạn:
e = 1 + 1/1! + 1/2! + 1/3! + ....
Hãy viết chương trình ước lượng e bằng cách tính biểu thức
1 + 1/1! + 1/2! + 1/3! + ... + 1/n!
trong đó n là số nguyên được người dùng nhập vào.

12. Điều chỉnh chương trình trong bài 11 sao cho nó tiếp tục cộng thêm các thành phần mới 
cho tới khi thành phần hiện tại nhỏ hơn eps (ε), trong đó eps là một số (thực) rất nhỏ được nhập bởi người dùng.