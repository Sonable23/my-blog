+++
title = "Giới thiệu về Java và JavaScript"
date = "2024-12-18T10:00:00+07:00"
description = "Tổng quan về hai ngôn ngữ lập trình Java và JavaScript, bao gồm lịch sử, đặc điểm, ứng dụng và ví dụ cơ bản."
tags = ["java", "javascript", "gioi-thieu", "lap-trinh"]
categories = ["Lập trình", "Công nghệ"]
authors = ["Hai Son"]
+++

## Giới thiệu

Java và JavaScript là hai ngôn ngữ lập trình phổ biến trong thế giới công nghệ thông tin. Mặc dù có tên gọi khá giống nhau, chúng là hai ngôn ngữ hoàn toàn khác biệt với mục đích sử dụng và đặc điểm riêng. Bài viết này sẽ cung cấp cái nhìn tổng quan về cả hai ngôn ngữ này.

## Java

### Lịch sử

Java được phát triển bởi James Gosling và các đồng nghiệp tại Sun Microsystems (sau này được Oracle mua lại) vào đầu những năm 1990. Ban đầu được gọi là "Oak", Java được thiết kế với mục tiêu "Write Once, Run Anywhere" (WORA - Viết một lần, chạy mọi nơi), cho phép ứng dụng chạy trên nhiều nền tảng khác nhau mà không cần biên dịch lại.

### Đặc điểm

*   **Hướng đối tượng (Object-Oriented):** Java tuân theo mô hình lập trình hướng đối tượng, với các khái niệm như lớp (class), đối tượng (object), kế thừa (inheritance), đa hình (polymorphism).
*   **Đa nền tảng (Platform Independent):** Nhờ Máy ảo Java (JVM), code Java được biên dịch thành bytecode và có thể chạy trên bất kỳ hệ điều hành nào có cài đặt JVM.
*   **Kiểu dữ liệu tĩnh (Static Typing):** Kiểu dữ liệu của biến được kiểm tra tại thời điểm biên dịch, giúp phát hiện lỗi sớm.
*   **Quản lý bộ nhớ tự động (Garbage Collection):** JVM tự động quản lý bộ nhớ, giúp lập trình viên không cần lo lắng về việc cấp phát và giải phóng bộ nhớ.
*   **Hiệu năng cao:** Java được biên dịch thành bytecode và chạy trên JVM, mang lại hiệu năng tốt, đặc biệt cho các ứng dụng phức tạp.

### Ứng dụng

*   Ứng dụng doanh nghiệp (ERP, CRM).
*   Ứng dụng di động Android.
*   Ứng dụng web (backend).
*   Game.
*   Ứng dụng khoa học và tài chính.

### Ví dụ

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}