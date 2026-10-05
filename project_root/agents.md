# AI Agent Guidelines & Instructions

## Project Context
This project is a CLI Quiz Application built in Java strictly adhering to structured / procedural programming principles.

## Allowed Constructs
* **Language Features:** Primitives (`int`, `boolean`, `char`, etc.), standard 1D/2D arrays (`Quiz[]`, `String[]`).
* **Data Types:** Java `record` types or simple data classes with public fields (e.g., `record Question(String prompt, String[] options, int correctIdx) {}`).
* **Control Flow:** `if / else`, `switch`, `for`, `while`, `do-while`.
* **Architecture:** Static procedural methods (`public static`) grouped inside utility/main classes.

## Strict Restrictions (Do NOT Use)
* **No Java Collections:** No `ArrayList`, `HashMap`, `HashSet`, `List`, `Map`, `Set`, etc.
* **No OOP Abstractions:** No `interface`, `abstract class`, custom inheritance (`extends`), or polymorphism (`implements`, `super`, `@Override`).
* **No High-Level Java Paradigms:** No `Streams`, `Lambdas` (`->`), `Optional`, or Generics (`<T>`).

## Code Style & Rules for AI Agents
1. **Array Sizing:** Always use fixed-size primitive arrays with explicit tracking counters (e.g., `Question[] questions = new Question[50]; int questionCount = 0;`).
2. **Procedural Logic:** Keep game loops and user interface logic in static procedural methods.
3. **Data Immutability/Simplicity:** Use simple `record` types as passive data containers, avoiding internal complex domain logic or behavior inside records.