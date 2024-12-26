+++
title = "Giới thiệu về Lập trình Hướng đối tượng (OOP) trong Java"
date = "2024-12-11T10:00:00+07:00" # Định dạng thời gian ISO 8601
description = "Tìm hiểu các khái niệm cơ bản của Lập trình Hướng đối tượng trong Java: Tính đóng gói, Kế thừa và Đa hình."
tags = ["java", "oop", "object-oriented programming", "lap trinh huong doi tuong"]
categories = ["Java", "OOP"]
authors = ["Hai Son"] # Thay bằng tên của bạn
series = ["Java Cơ bản"] # Nếu bài viết thuộc một chuỗi bài viết
+++

## Lập trình Hướng đối tượng (OOP) là gì?

Lập trình Hướng đối tượng (OOP) là một mô hình lập trình dựa trên khái niệm "đối tượng", có thể chứa dữ liệu, dưới dạng các trường, thường được gọi là thuộc tính; và mã, dưới dạng các thủ tục, thường được gọi là phương thức.

### Các nguyên tắc cơ bản của OOP

OOP dựa trên bốn nguyên tắc chính:

*   **Tính đóng gói (Encapsulation):** Giấu dữ liệu bên trong lớp và chỉ cho phép truy cập thông qua các phương thức.
*   **Tính kế thừa (Inheritance):** Cho phép một lớp kế thừa các thuộc tính và phương thức từ một lớp khác.
*   **Tính đa hình (Polymorphism):** Cho phép một đối tượng có nhiều hình dạng hoặc hành vi khác nhau.
*   **Tính trừu tượng (Abstraction):** Ẩn các chi tiết phức tạp và chỉ hiển thị các thông tin cần thiết.

### Ví dụ về Class và Object trong Java

```java
public class Dog {
    String name;
    String breed;

    public Dog(String name, String breed) {
        this.name = name;
        this.breed = breed;
    }

    public void bark() {
        System.out.println("Woof!");
    }

    public static void main(String[] args) {
        Dog myDog = new Dog("Buddy", "Golden Retriever");
        myDog.bark(); // In ra "Woof!"
    }
}