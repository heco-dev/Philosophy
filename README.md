# Our Guiding Philosophy

## Who we are
- So what are we doing here?
  - Creating solutions for HECO business problems related to the user interface

- What part of the app do we work on?
  - The portion of the application that a user interacts with directly

- What are the underlying technologies we work with?
  - TypeScript, JavaScript, CSS, HTML, REST, DOM, Angular, ???

## 1st Principles
- KISS – Keep It Simple Stupid
- YAGNI – You Ain’t Gonna Need It
- T-DRY – Try to be DRY(Don’t Repeat Yourself)
- Testable code
- ??? 

## External Guidance
- Angular (https://angular.io/guide/styleguide )
- JavaScript:
  - Google’s = https://google.github.io/styleguide/jsguide.html
  - Airbnb’s = https://github.com/airbnb/javascript 
- TypeScript:
  - Google’s https://github.com/google/gts
  - TypeScript team’s = https://github.com/microsoft/TypeScript/wiki/Coding-guidelines
- Google's Engineering Philosophy (http://googlesystem.blogspot.com/2008/03/googles-engineering-philosophy.html )
- ???

## Code Reviews and testing
- When we point out an issue we should be able to cite a styleguide, agreed-to standard, or principle
- During code review we can reference our github page and see real world code in StackBlitz
  - https://stackblitz.com/@heco-dev

## Standards to agree on
- Error handling
- Promises vs Observables vs async/await
- Code formatting – (e.g. Prettier)
- TsLint rules
- Editing another author’s code
  - Do we need to notify
- Direct DOM manipulation
- Design Specs?
- prefer changeDetection: ChangeDetectionStrategy.OnPush
- method order... alphabetically or by order of use?

## Standards
- Do NOT:
  1. #### Don't test private methods directly

---

- Do:
  1. #### Return from functions, try not to have side-effects
  2. #### Prefer built-in Array Iteration methods (map, filter, forEach)
  3. #### Test the component template, especially when there is not much to test in the class controller
  4. #### Try to make presentation components (minimize code in the class controller)
  5. #### Injected services should be private and readonly then make public internal methods to expose them when needed
  6. #### Method order should be: Angular's public lifecycle methods first, then our public methods then our private methods
