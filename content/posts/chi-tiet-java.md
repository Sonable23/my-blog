+++
title = "Giới thiệu chi tiết về Java"
date = "2024-12-24T10:00:00+07:00"
description = "Tìm hiểu chi tiết về ngôn ngữ lập trình Java, từ lịch sử hình thành đến các khái niệm cốt lõi và ứng dụng thực tế."
tags = ["java", "lap-trinh", "oop", "jvm", "jdk"]
categories = ["Lập trình", "Java"]
authors = ["Hai Son"]
+++

## Giới thiệu chi tiết về Java

Java là một ngôn ngữ lập trình đa nền tảng, hướng đối tượng và được sử dụng rộng rãi trên toàn thế giới. Được phát triển bởi James Gosling và các đồng nghiệp tại Sun Microsystems (sau này được Oracle mua lại), Java ra đời với mục tiêu "Write Once, Run Anywhere" (WORA - Viết một lần, chạy mọi nơi).

### Lịch sử hình thành

*   **Đầu những năm 1990:** Dự án "Green" được khởi xướng tại Sun Microsystems với mục tiêu phát triển một ngôn ngữ cho các thiết bị điện tử tiêu dùng.
*   **1995:** Ngôn ngữ "Oak" được đổi tên thành "Java" và chính thức ra mắt.
*   **1996:** Phiên bản Java Development Kit (JDK) 1.0 được phát hành.
*   **Hiện tại:** Java tiếp tục được phát triển và cập nhật bởi Oracle với các phiên bản JDK mới, mang lại nhiều tính năng và cải tiến.

### Đặc điểm của Java

*   **Hướng đối tượng (Object-Oriented):** Java tuân theo mô hình lập trình hướng đối tượng, với các khái niệm như lớp (class), đối tượng (object), kế thừa (inheritance), đa hình (polymorphism), trừu tượng (abstraction) và đóng gói (encapsulation).
*   **Đa nền tảng (Platform Independent):** Nhờ Máy ảo Java (JVM), mã Java được biên dịch thành bytecode và có thể chạy trên bất kỳ hệ điều hành nào có cài đặt JVM.
*   **Kiểu dữ liệu tĩnh (Static Typing):** Kiểu dữ liệu của biến được kiểm tra tại thời điểm biên dịch, giúp phát hiện lỗi sớm.
*   **Quản lý bộ nhớ tự động (Garbage Collection):** JVM tự động quản lý bộ nhớ, giúp lập trình viên không cần lo lắng về việc cấp phát và giải phóng bộ nhớ.
*   **Bảo mật:** Java được thiết kế với nhiều tính năng bảo mật, giúp ngăn chặn các cuộc tấn công.
*   **Hiệu năng cao:** Java được biên dịch thành bytecode và chạy trên JVM, mang lại hiệu năng tốt, đặc biệt cho các ứng dụng phức tạp.
*   **Đa luồng (Multithreading):** Hỗ trợ lập trình đa luồng, cho phép thực hiện nhiều tác vụ đồng thời.

### Các thành phần quan trọng

*   **JDK (Java Development Kit):** Bộ công cụ phát triển Java, bao gồm trình biên dịch (javac), JVM, và các thư viện.
*   **JRE (Java Runtime Environment):** Môi trường thực thi Java, bao gồm JVM và các thư viện cần thiết để chạy ứng dụng Java.
*   **JVM (Java Virtual Machine):** Máy ảo Java, chịu trách nhiệm thực thi bytecode Java.

### Cú pháp cơ bản

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}