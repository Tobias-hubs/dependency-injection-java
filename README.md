# 🚀 Exercise 5: Dependency Injection with Java

## ✨ Summary
This PR completes all three parts of Exercise 5, moving step by step from manual dependency wiring to a fully working CDI setup with Weld.

## 🔧 Changes by Part
- **Part 1 – Manual Constructor Injection**
  - Created interfaces and implementations (service + persistence layer)
  - Manually instantiated dependencies in `Main` and verified wiring

- **Part 2 – Minimal DI Container**
  - Implemented a simple reflection-based container
  - Container recursively resolved constructor dependencies
  - Demonstrated automatic creation of the full dependency graph

- **Part 3 – Using Weld (CDI)**
  - Added `weld-se-core` dependency and `beans.xml`
  - Annotated implementation classes with `@ApplicationScoped` and `@Inject`
  - Refactored `App.java` to start Weld and retrieve the top-level service
  - Verified correct behavior with CDI-managed injection

## ✅ Result
- All three approaches (manual, custom container, Weld) produce the same functional output
- Weld now handles dependency injection automatically
- Console output confirms services and repositories are wired correctly

## Linked School Issue 
[Exercise 5 - Dependency Injection](https://github.com/fungover/exercise2025/issues/95)
