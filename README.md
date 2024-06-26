Kiểm tra hiệu năng trang web
 ![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/7df61f9d-7a71-4138-b0cf-b0ca6b703a72)

 ![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/8f8f3d57-f1a4-4617-ae10-99e89438bbcf)

![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/e520255b-bb19-4328-a437-a79a922e8a94)

 
 
Mục tiêu:
•	Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web: https://tiki.vn/
•	Chạy kịch bản kiểm tra và ghi lại kết quả.
•	Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
•	Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
Kịch bản kiểm tra:
  Thread Group:
•	Số lượng thread: 100
•	Thời gian chạy: 60 giây = Ramp-up period: 10 giây HTTP Request:
•	URL: https://tiki.vn/
•	Method: GET
•	Content encoding: UTF-8 Listeners:
•	View Results Tree
•	Aggregate Report  
Kết quả kiểm tra:
![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/35c46d32-f02b-4151-855c-8abd99dc5b10)
![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/f519e382-b632-4652-be5e-2d32b2a3ed2b)
![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/fd3970bb-c880-46a4-967e-2b8c61b715d6)



 
 
 
Kết luận:
	Trang web https://tiki.vn/ có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (100%), số lượng yêu cầu thất bại rất thấp (0,00%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web cũng khá cao (12 yêu cầu/giây).
Kiểm tra hiệu năng API
Mục tiêu:
•	Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập https://pokeapi.co/
•	Chạy kịch bản kiểm tra và ghi lại kết quả.
•	Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
•	Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
Kịch bản kiểm tra:
•	Thread Group:
•	Số lượng thread: 100
•	Thời gian chạy: 60 giây
•	Ramp-up period: 10 giây HTTP Request:
•	URL: https://pokeapi.co/
•	Method: GET
•	Content encoding: UTF-8 Listeners:
•	View Results Tree
•	Aggregate Report
Kết quả kiểm tra:
![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/8ae844a2-baf7-495d-8deb-3c254be552d0)
![image](https://github.com/HIDR00/bt_JMeter_test/assets/115889838/a2c497f6-cbdf-4d33-8050-428cf494a292)


 
 
Kết luận:
Trang web  https://pokeapi.co/ có hiệu năng tốt. Số lượng yêu cầu thành công trung bình (99,63%), số lượng yêu cầu thất bại thấp (0,37%). Thời gian phản hồi trung bình, trung vị đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web trung bình(5 yêu cầu/giây).
So Sánh :
Với 2 trang web https://tiki.vn/ và https://pokeapi.co/ thì trang web https://tiki.vn/ có hiệu năng tốt hơn khi có thể phản hồi số lượng request lớn hơn, tỉ lệ lỗi nhỏ hơn, thời gian phản hồi nhanh hơn
