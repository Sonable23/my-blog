+++
title = "Xử lý Bất đồng bộ trong JavaScript: Callbacks, Promises và Async/Await"
date = "2024-12-26T11:00:00+07:00"
description = "Hướng dẫn chi tiết về cách xử lý các hoạt động bất đồng bộ trong JavaScript, từ Callbacks truyền thống đến Promises và cú pháp hiện đại async/await."
tags = ["javascript", "asynchronous", "callback", "promise", "async/await", "lập trình bất đồng bộ"] # Thêm tag tiếng Việt
categories = ["JavaScript", "Lập trình Bất đồng bộ"] # Thêm category tiếng Việt
authors = ["Hai Son"]
+++

## Giới thiệu về Bất đồng bộ trong JavaScript

JavaScript là một ngôn ngữ đơn luồng, nghĩa là nó chỉ thực thi một tác vụ tại một thời điểm. Điều này có nghĩa là nếu một tác vụ mất nhiều thời gian để hoàn thành (ví dụ: yêu cầu mạng, đọc/ghi file), luồng chính sẽ bị "chặn" và ứng dụng sẽ ngừng phản hồi. Để giải quyết vấn đề này, JavaScript sử dụng cơ chế *bất đồng bộ*.

Bất đồng bộ cho phép chương trình tiếp tục thực thi các tác vụ khác trong khi chờ một tác vụ tốn thời gian hoàn thành. Khi tác vụ đó hoàn thành, một callback function (hàm gọi lại) sẽ được thực thi để xử lý kết quả.

## 1. Callbacks: Cách tiếp cận truyền thống

Callbacks là cách tiếp cận đầu tiên và đơn giản nhất để xử lý bất đồng bộ. Một callback là một hàm được truyền vào như một đối số cho một hàm khác và sẽ được gọi sau khi hàm đó hoàn thành việc thực thi.

### Ví dụ về Callback với `setTimeout`

Hàm `setTimeout` là một ví dụ điển hình về việc sử dụng callback:

```javascript
console.log("Bắt đầu");

setTimeout(() => {
  console.log("Kết thúc sau 2 giây");
}, 2000);

console.log("Tiếp tục thực thi");

// Kết quả in ra:
// Bắt đầu
// Tiếp tục thực thi
// Kết thúc sau 2 giây (sau 2 giây chờ đợi)

## 2. Promises: Giải pháp cho Callback Hell

Promises được giới thiệu trong ES6 (ECMAScript 2015) để giải quyết vấn đề của Callback Hell và cung cấp một cách tiếp cận rõ ràng và dễ quản lý hơn cho lập trình bất đồng bộ. Một Promise đại diện cho kết quả của một thao tác bất đồng bộ, mà kết quả này có thể chưa có tại thời điểm hiện tại, nhưng sẽ có trong tương lai.

### Các trạng thái của Promise

Một Promise có thể ở một trong ba trạng thái:

*   **Pending (Đang chờ):** Trạng thái ban đầu. Thao tác bất đồng bộ đang được thực hiện.
*   **Fulfilled (Đã hoàn thành/Thành công):** Thao tác bất đồng bộ đã hoàn thành thành công và có một giá trị kết quả.
*   **Rejected (Đã bị từ chối/Thất bại):** Thao tác bất đồng bộ gặp lỗi.

### Tạo một Promise

Một Promise được tạo bằng cách sử dụng constructor `Promise`:

```javascript
const myPromise = new Promise((resolve, reject) => {
  // Thực hiện thao tác bất đồng bộ ở đây
  setTimeout(() => {
    const success = true; // Giả sử thao tác thành công
    if (success) {
      resolve("Dữ liệu đã được lấy thành công!"); // Chuyển Promise sang trạng thái Fulfilled
    } else {
      reject("Đã có lỗi xảy ra!"); // Chuyển Promise sang trạng thái Rejected
    }
  }, 1000);
});


## 3. Async/Await: Cú pháp hiện đại và dễ đọc

`async/await` được giới thiệu trong ES8 (ECMAScript 2017) và được xây dựng dựa trên Promises. Nó cung cấp một cú pháp gọn gàng và dễ đọc hơn rất nhiều so với việc sử dụng `.then()` và `.catch()` liên tục, giúp code bất đồng bộ trông giống như code đồng bộ.

### `async`

Từ khóa `async` được đặt trước một hàm để biến nó thành một *hàm bất đồng bộ*. Một hàm `async` luôn trả về một Promise. Nếu hàm trả về một giá trị không phải là Promise, JavaScript sẽ tự động bọc giá trị đó trong một Promise đã được resolve.

```javascript
async function myAsyncFunction() {
  return "Hello from async function!"; // Trả về một giá trị
}

myAsyncFunction().then(value => console.log(value)); // In ra: Hello from async function!