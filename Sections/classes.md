# 4. Main Classes

## 4.1 Student
* **Purpose:** Representing the person borrowing the book.
* **Attributes:**
    * `Name: String`
    * `FacultyID: int`
    * `Email: String`
    * `BorrowedBooksList: List<Book>`

## 4.2 Book
* **Purpose:** Representing the resource / item being borrowed.
* **Attributes:**
    * `Title: String`
    * `Author: String`
    * `Subject: String`
    * `isAvailable: Boolean`
    * `isDamaged: Boolean`

## 4.3 Librarian
* **Purpose:** Representing the library keeper and organizer.
* **Attributes:**
    * `Name: String`
    * `EmployeeID: int`
    * `WorkingHours: int`
    * `Email: String`

## 4.4 Borrows
* **Purpose:** Representing the event of borrowing a book by a student.
* **Attributes:**
    * `Book: Book`
    * `Borrower: Student`
    * `BorrowDate: Date`
    * `ReturnDate: Date`

## 4.5 Fine
* **Purpose:** Representing the penalty fee required of student damaged a borrowed resource.
* **Attributes:**
    * `Price: Double`
    * `Reason: String`
    * `isPaid: Boolean`
    * `dmgCount: int` *(representing the number of times a student returned a damaged resource)*