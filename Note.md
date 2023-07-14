# JavaScript Basic
***
1. Khai báo biến
    * `var`: Khai báo biến toàn cục
    * `let`: Khai báo biến cục bộ

2. Kiểm tra kiểu dữ liệu: `typeof + biến`

3. Toán tử so sánh tuyệt đối: ` === ` -> So sánh cả giá trị và kiểu dữ liệu

4. Toán tử trải: `...`

5. Built-in function
    * `alert`: Hộp thoại cảnh báo
    * `console`: Tương tác với cửa sổ console
    * `confirm`: Hộp thoại xác nhận
    * `prompt`: Kết hợp giữa confirm và alert
    * `setTimeout`: Chạy code sau 1 khoảng thời gian
        ```php
        setTimeout(function() {
			...
		}, 1000)```
    * `setInterval`: Chạy liên tục trong 1 khoảng thời gian, mỗi lần chạy cách nhau 1s

6. String method
    * `.length()`: lấy độ dài chuỗi
	* `.indexOf()`: trả về vị trí đầu tiên của chuỗi truyền vào
	* `.slice()`: Cắt chuỗi
	* `.replace()`: Thay thế một chuỗi bằng một chuỗi truyền vào
	* `.toUpperCase()`: Viết hoa tất cả
	* `.toLowerCase()`: Viết thường tất cả
	* `.trim()`: Loại bỏ khoảng trắng thừa
	* `.split()`: Chuyển chuỗi thành array theo điểm chung truyền vào
	* `.charAt()`: Lấy vị trí của ký tự

7. Array method
    * `.toString()`: Chuyển mảng thành chuỗi
	* `.join()`: Nối mảng
	* `.pop()`: Xóa phần tử ở cuối mảng và trả về phần tử đó
	* `.shift()`: Xóa phần tử đầu mảng và trả về phần tử đó
	* `.push()`: Thêm phần tử vào cuối mảng
	* `.unshift()`: Thêm phần tử vào đầu mảng và trả về độ dài của mảng
	* `.splice()`: Xóa phần tử theo index và có thể chèn phần tử
		* VD: `myArray.splice(1,2) -> xóa 2 phần từ từ index 1`
		* VD: `myArray.splice(1,2, 'value') -> xóa 2 phần từ từ index 1 và chèn value vào`
	* `.concat()`: Nối 2 mảng
	* `.slice()`: Cắt phần tử của mảng và trả về phần tử đó
		* VD: `array.slice(1,2) -> Cắt từ phần tử 1 đến 2`
		* VD: `array.slice(0) -> Copy mảng`
	* `.forEach()`: Duyệt qua từng phần tử của mảng, trả về phần tử và index
		* VD: `myArray.forEach(function(val){...});`
	* `.every()`: Kiểm tra tất cả phần tử trong mảng thỏa mãn 1 điều kiện, kiểu trả về boolean
		* VD: `myArray.every(function(val){return ...});`
	* `.some()`: Kiểm tra 1 phần tử trong mảng có thỏa mãn 1 điều kiện không
	* `.find()`: Tìm kiếm trong array có phần tử truyền vào không
	* `.filter()`: Giống find nhưng trả về tất cả phần tử thỏa mãn
	* `.map()`: Trả về một mảng mới với số lượng phần tử bằng mảng cũ, giá trị phần tử được quyết định bởi lệnh return
	    * VD: `newArray = myArray.map(myFunction);`
	* `.reduce()`: Nhận về 1 giá trị duy nhất sau khi tính toán trên array
    * Cách tự định nghĩa phương thức của Array:
        * VD: `array.prototype.tenPhuongThuc = function(){...}`
8. Function
    * Declaration function: `var myFunction = function(){...}`
	* Expression function: `myFunction = function(){...}`
9. Loop
    * `for in`: Lặp qua key
    * `for of`: Lặp qua value

10. Math Object
    * `Math.PI`: Lấy số PI
	* `Math.round()`: Làm tròn số thập phân -> số nguyên
	* `Math.abs()`: Giá trị tuyệt đối
	* `Math.ceil()`: Làm tròn lên
	* `Math.floor()`: Làm tròn xuống
	* `Math.random()`: Giá trị ngẫu nhiên
	* `Math.min()`: Giá trị nhỏ nhất
	* `Math.max()`: Giá trị lớn nhất
11. Object
    * `delete`: Xóa một key trong object
        * VD: `delete myObj.key1`
    * `constructor`: Hàm khởi tạo
12. Một số phương thức khác
    * `${variable}`: Cách đưa biến vào trong một chuỗi (Template String)
    * `.hasOwnProperty(variable)`: Kiểm tra tham số truyền vào có phải phần tử con không
    * `[...(new Set(array))]`: Cách loại bỏ phần tử lặp trong tham số truyền vào
    * `.includes()`: Tìm kiếm chuỗi truyền vào trong 1 chuỗi/mảng, có thể truyền thêm tham số index
        * VD: 
            ```php
            var myString = '......';
	        myString.includes('something');
            ```

	    * VD: 
            ```php
            var myArray = ['...', '...', '...'];
	        myArray.includes('something');
            ```
