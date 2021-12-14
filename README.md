# clean_code

Even bad code can function. But if code isn't clean, it can bring a development organization to its knees.

Code is clean if it can be understood easily – by everyone on the team. Clean code can be read and enhanced by a developer other than its original author. With understandability comes readability, changeability, extensibility and maintainability.

General rules
Follow standard conventions.
Keep it simple stupid. Simpler is always better. Reduce complexity as much as possible.
Boy scout rule. Leave the campground cleaner than you found it.
Always find root cause. Always look for the root cause of a problem.
The code should be the coding standard
Names rules
Choose descriptive and unambiguous names.
Make meaningful distinction.
Use pronounceable and searchable names.
Avoid acronyms and confusing names.
Replace magic numbers with named constants.
Avoid encodings. Don't append prefixes or type information.
Choose names at the appropriate level of abstraction.
Use long names for long scopes.
Names should describe side effects.
Functions rules
Small.
Do one thing and (Exception is one thing).
Use descriptive names.
Prefer fewer arguments(max 3).
No arguments should be used as output
Don't use flag/boolean arguments. Split method into several independent methods that can be called from the client without the flag.
Use less switch statments, Instead use enums and polymorphism.
The method that changes state should return void or throw exception(setters).
The method that doesnt changes state should return a value(getters/pure functions).
Avoid duplication.
Long methods means a class is hidden inside that method, refactor it.
Public method names are short and private are usually long and descriptive.
Comment rules
 -- One of the most common reasons for the comments is because the code is bad.  
If you're thinking about writing a comment, then the code should be refactored.
Comments can be useful when placed in certain places
Should be rare
Only by reading the code the programmer should know what the code does
Every comment you write is failure to express your code
Comment lies and misinformation
Good Comments:
Legal comments at top of the file (license).
Informative comments: eg what a regex do.
Warning and consequences.
Public API document.
Bad Comments:
Dont talk to yourself in the comment, life situation, about coworkers.
Redundant explanation.
Journal Comments.
Noise Comments, Banner comments .
Closing brace comments.
Attribution.
HTML comments.
Commented out code, Remove it.
Formatting / Source code structure
First impression for professional work.
It is a form of communication and it should indicate importance.
File Size: smaller is better maximum of 500 lines.
Use spaces between operators, parameters, and commas and to separate unrelated code.
No horizontal alignment/scroll bar (character limit max 120).
Indentation standard across all project and team in your company.
Organise methods as step down rule (public on top private down the hierarchy).
Dependent and similar functions should be close.
Declare variables close to their usage.
Classes and Objects
Objects hide the data abstraction and expose methods that operate the data.

The class name should represent its responsibility.
Should be small and do one thing.
Tell dont ask - It should tell what it does and should not ask how.
Less getter and setters
Hide internal structure.
More cohesive methods (one method changing state of many instance variables)
Expose less implementation so that we can use more OOPs and independent deploymentablility
Classes and Polymorphism are related (less switch statements)
Make good abstraction and encapsulation.
Prefer non-static methods to static methods.
Abstract should not know about concrete.
Object should have small number of instance variables.
Base class should know nothing about their derivatives.
Objects/Data structures/POJO
Data structures expose your data and do not have significant methods(POJO).

Prefer data structures.
Has more getter setters.
Avoid hybrids structures (half object and half data).
It should do one thing.
Opposite to classes.
Better to have many functions than to pass some code into a function to select a behavior.
POJO asks and dont tell.
POJO and switch are related.
No buisness rules .
Less new methods but can have many types.
Exceptions/ Error Handling
It should be scoped to our classes and dont resuse the java ones.
Error handling first then logic.
Prefer throw an Exception (unchecked exceptions).
Try block should have one line.
Look at separate business rules for errors and error handling.
Avoid returning a NULL, prefer to return an empty object or throw an exception.
Avoid passing NULL to the methods; this can generate NullPointerExceptions.
Null is not empty and not an error, instead Null is a value.
Tests
One assert per test.
Readable.
Follow TDD
Keep your test clean.
The tests must undergo changes in the same way that the code.
Use the F.I.R.S.T rule for testing:
Fast-running.
Independent
Repeatable in various environments.
Self-validating.
Timely.
Design rules
Keep configurable data at high levels.
Prefer polymorphism to if/else or switch/case.
Separate multi-threading code.
Prevent over-configurability.
Use dependency injection.
Follow Law of Demeter. A class should know only its direct dependencies.
Recognize and separate the responsibilities of a system.
Understandability tips
Be consistent. If you do something a certain way, do all similar things in the same way.
Use explanatory variables.
Encapsulate boundary conditions. Boundary conditions are hard to keep track of. Put the processing for them in one place.
Prefer dedicated value objects to primitive type.
Avoid logical dependency. Don't write methods which works correctly depending on something else in the same class.
Avoid negative conditionals.
Look to cover tests each line of code
No code is immune to improvement, refactor and make it better
Try not to let the code rot. It is much cheaper to create a clean code than cleaning a rotten code
There is always time to refactor then to refactor after getting rot or finding some issue in it.
Refactor
Write test that fails
Make the test pass
(Refactor) Make the code better
Before making any kind of refactoring, it is important to have good coverage tests.
After increasing or creating test coverage, you can begin to leave the clearest code and fix some bugs.
Now, after leaving the code clearer, someone else can probably clean it even more.
Follow TDD whenever wherever possible.
Code smells
Rigidity. The software is difficult to change. A small change causes a cascade of subsequent changes.
Fragility. The software breaks in many places due to a single change.
Immobility. You cannot reuse parts of the code in other projects because of involved risks and high effort.
Needless Complexity.
Needless Repetition.
Opacity. The code is hard to understand.
References: https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29
https://dzone.com/articles/clean-code-summary-and-key-points
https://kingadesign.com/clean-code-poster-free-download
https://amzn.to/2ZQyX22
https://www.oreilly.com/library/view/clean-code/9780134661742/

Feedback and suggestions are always welcomed.
