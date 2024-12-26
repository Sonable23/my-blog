+++
title = "Giới thiệu chi tiết về JavaScript"
date = "2024-12-21T11:00:00+07:00"
description = "Tìm hiểu chi tiết về ngôn ngữ lập trình JavaScript, từ lịch sử hình thành đến các khái niệm cốt lõi và ứng dụng đa dạng trong phát triển web và hơn thế nữa."
tags = ["javascript", "lap-trinh", "web", "frontend", "backend", "nodejs"]
categories = ["Lập trình", "JavaScript", "Web"]
authors = ["Hai Son"]
+++

## Giới thiệu chi tiết về JavaScript

JavaScript là một ngôn ngữ lập trình thông dịch, đa năng, chủ yếu được sử dụng để tạo ra các trang web động và tương tác. Tuy có tên gọi gần giống Java, nhưng JavaScript là một ngôn ngữ hoàn toàn khác biệt.

### Lịch sử hình thành

*   **1995:** Brendan Eich phát triển JavaScript tại Netscape Communications với tên ban đầu là "Mocha", sau đó đổi thành "LiveScript" và cuối cùng là "JavaScript".
*   **Ban đầu:** JavaScript được thiết kế để chạy trên trình duyệt web, giúp tạo ra các trang web động và tương tác.
*   **Hiện tại:** JavaScript đã phát triển mạnh mẽ và được sử dụng rộng rãi trong cả front-end (giao diện người dùng) và back-end (phía máy chủ) với Node.js, cũng như trong phát triển ứng dụng di động (React Native, Ionic) và nhiều lĩnh vực khác.

### Đặc điểm của JavaScript

*   **Thông dịch (Interpreted):** Mã JavaScript được thông dịch trực tiếp bởi trình duyệt web (hoặc môi trường Node.js), không cần biên dịch trước.
*   **Kiểu dữ liệu động (Dynamic Typing):** Kiểu dữ liệu của biến được xác định tại thời điểm chạy, không cần khai báo kiểu dữ liệu rõ ràng.
*   **Hướng đối tượng dựa trên Prototype (Prototype-based OOP):** JavaScript sử dụng prototype để kế thừa, khác với class-based OOP của Java.
*   **Client-side scripting:** Chạy trên trình duyệt web, giúp tạo ra các trang web tương tác và động.
*   **Server-side scripting (Node.js):** Cho phép JavaScript chạy trên máy chủ, mở rộng khả năng ứng dụng của JavaScript sang backend.
*   **Đa nền tảng:** Có thể chạy trên nhiều hệ điều hành và thiết bị.

### Cú pháp cơ bản

```javascript
// Khai báo biến
let message = "Hello, World!";

// In ra console
console.log(message);

// Hàm
function greet(name) {
  return "Hello, " + name + "!";
}

console.log(greet("JavaScript"));

// Câu điều kiện
let x = 10;
if (x > 5) {
  console.log("x lớn hơn 5");
}

// Vòng lặp
for (let i = 0; i < 5; i++) {
  console.log(i);
}