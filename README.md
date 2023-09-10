# clean-coding-typescript
This repo talks about the clean coding principles mentioned in "Clean Coding by Robert C Martin" all the examples in this repository are in typescript.

# What is Clean Code?
> Clean code is simple and direct. Clean code reads like well-written prose. Clean code never obscures the designer’s intent but rather is full of crisp abstractions and straightforward linesof control. **- Grady Booch**

> Clean code can be read, and enhanced by a developer other than its original author. It has unit and acceptance tests. It has meaningful names. It provides one way rather than many ways for doing one thing. It has minimal dependencies, which are explicitly defined, and provides a clear and minimal API. Code should be literate since depending on the language, not all necessary information can be expressed clearly in code alone **- Dave Thomas**

Clean code is a well structured, simple to understand, easy to maintain and thoroughly tested code. It should make sense for others in the team at a first glance. 

I really like one quote by the author on maintaining the application by infering the boy scout rule. ***Leave the campgrounds cleaner than you found it***. This perfectly fits in maintaining the application. Always make sure to make the existing code cleaner than before.

Below are some principles mentioned in the book.
## 1. Meaningful Names

Naming is the integral part of coding, as a developers we come up with at least one new name everytime we code. We name variables, functions, classes, arguments, packages and so on. Since most of our code starts with naming, it should be done well to make the code readable. Let us see few simple ways to name different things in our code.

### Use of meaningful and intention revealing names

Names we use in code should be self explanatory, they should provide the context of what that variable, function or class is supposed to do without any comments.

**Bad:**
```ts
class A;
function a(x: string);
const x;
```

**Good:**
```ts
class Employee;
function getRole(employeeId: string): string {};
const dateOfJoining;
```

### Use pronounceable and searchable names 

Using pronounceable names will help developers understand the context easily and will be easier for someone new to use those variables or functions while coding and it will be easier for them to search them from anywhere in the codebase.

**Bad:**
```ts
function dte2mth(dt: Date) {
  return dt.getMonth();
}
const mnth;
```

**Good:**
```ts
function dateToMonth(date: Date) {
  return date.getMonth();
}
const month;
```










