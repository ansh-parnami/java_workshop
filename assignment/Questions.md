# Java Practice Questions

---

## Q1. 
You have an interface **NotificationService** used by many classes.
```java
interface NotificationService {
    void send(String message);
}
```
Add retry support to an existing interface without breaking implementations.
**Tasks**
- Add a default method `sendWithRetry(String message, int retries)`
- Existing implementations must continue working
- Retry logic should internally call `send()`

---

## Q2.
Create a utility to validate strings using custom rules.

**Tasks**
- Create a functional interface `StringValidator`
- Method should accept a `String` and return `boolean`
- Write a method `validate(String value, StringValidator validator)`
- Use lambdas to validate:
  - non-empty string
  - string length > 5
  - string starts with a capital letter

---

## Q3.
Given a list of users:

```java
class User {
    String name;
    int age;
}
```

**Tasks**
- Filter users with age ≥ 18
- Convert names to uppercase
- Sort by name
- Collect into a list

---

## Q4.
Given:
```java
List<Integer> numbers
```

**Tasks**
- Create predicates for positive numbers and even numbers
- Combine them using `and()`
- Print only positive even numbers

---

## Q5.
Method:
```java
Optional<User> findUser(String id);
```

**Tasks**
- Print username if present
- Ignore inactive users
- Print "User not found" otherwise
- No null checks allowed

---

## Q6.
Create a record `Employee`.

**Tasks**
- Fields: `id`, `salary`
- Validate salary > 0
- Add method `isHighEarner()` (salary > 100000)
- Demonstrate immutability

---

## Q7.
Model a payment system.

**Tasks**
- Create sealed interface `Payment`
- Permit `CardPayment` and `UpiPayment`
- Implement a `process(Payment p)` method using pattern matching

---

## Q8.

**Tasks**
- Build a multi-line SQL query using text blocks
- Inject `userId` using `.formatted()`
- Keep formatting readable

---

## End of Questions

