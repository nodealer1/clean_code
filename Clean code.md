Even bad code can function. But if code isn't clean, it can bring a development organization to its knees. 

Code is clean if it can be understood easily – by everyone on the team. Clean code can be read and enhanced by a developer other than its original author. With understandability comes readability, changeability, extensibility and maintainability.
_____________________________________

## General rules
1. Follow standard conventions.
2. Keep it simple stupid. Simpler is always better. Reduce complexity as much as possible.
3. Boy scout rule. Leave the campground cleaner than you found it.
4. Always find root cause. Always look for the root cause of a problem.
5. The code should be the coding standard

## Names rules
1. Choose descriptive and unambiguous names.
2. Make meaningful distinction.
3. Use pronounceable and searchable names.
4. Avoid acronyms and confusing names.
5. Replace magic numbers with named constants.
6. Avoid encodings. Don't append prefixes or type information.
7. Choose names at the appropriate level of abstraction.
8. Use long names for long scopes.
9. Names should describe side effects.

## Functions rules
1. Small.
2. Do one thing and (Exception is one thing).
3. Use descriptive names.
4. Prefer fewer arguments(max 3).
5. No arguments should be used as output
6. Don't use flag/boolean arguments. Split method into several independent methods that can be called from the client without the flag.
7. Use less switch statments, Instead use enums and polymorphism.
8. The method that changes state should return void or throw exception(setters).
9. The method that doesnt changes state should return a value(getters/pure functions).
10. Avoid duplication.
11. Long methods means a class is hidden inside that method, refactor it.
12. Public method names are short and private are usually long and descriptive.

## Comment rules   
	 -- One of the most common reasons for the comments is because the code is bad.  
1. If you're thinking about writing a comment, then the code should be refactored.
2. Comments can be useful when placed in certain places
3. Should be rare
4. Only by reading the code the programmer should know what the code does
5. Every comment you write is failure to express your code
6. Comment lies and misinformation
7. Good Comments:
	* Legal comments at top of the file (license).
	* Informative comments: eg what a regex do.
	* Warning and consequences.
	* Public API document.
8. Bad Comments:
	* Dont talk to yourself in the comment, life situation, about coworkers.
	* Redundant explanation.
	* Journal Comments.
	* Noise Comments, Banner comments .
	* Closing brace comments.
	* Attribution.
	* HTML comments.
	* Commented out code, Remove it.

## Formatting / Source code structure
1. First impression for professional work.
2. It is a form of communication and it should indicate importance.
3. File Size: smaller is better maximum of 500 lines.
4. Use spaces between operators, parameters, and commas and to separate unrelated code.
5. No horizontal alignment/scroll bar (character limit max 120).
6. Indentation standard across all project and team in your company.
7. Organise methods as step down rule (public on top private down the hierarchy).
8. Dependent and similar functions should be close.
9. Declare variables close to their usage.

## Classes and Objects
Objects hide the data abstraction and expose methods that operate the data.
1. The class name should represent its responsibility.
2. Should be small and do one thing.
3. Tell dont ask - It should tell what it does and should not ask how.
4. Less getter and setters 
5. Hide internal structure.
6. More cohesive methods (one method changing state of many instance variables)
7. Expose less implementation so that we can use more OOPs and independent deploymentablility
8. Classes and Polymorphism are related (less switch statements)
9. Make good abstraction and encapsulation.
10. Prefer non-static methods to static methods.
11. Abstract should not know about concrete.
12. Object should have small number of instance variables.
13. Base class should know nothing about their derivatives.

## Objects/Data structures/POJO  
Data structures expose your data and do not have significant methods(POJO).  
1. Prefer data structures.
2. Has more getter setters.
3. Avoid hybrids structures (half object and half data).
4. It should do one thing.
5. Opposite to classes.
6. Better to have many functions than to pass some code into a function to select a behavior.
7. POJO asks and dont tell.
8. POJO and switch are related.
9. No buisness rules .
10. Less new methods but can have many types.

## Exceptions/ Error Handling 
1. It should be scoped to our classes and dont resuse the java ones.
2. Error handling first then logic.
3. Prefer throw an Exception (unchecked exceptions).
4. Try block should have one line.
5. Look at separate business rules for errors and error handling.
6. Avoid returning a NULL, prefer to return an empty object or throw an exception.
7. Avoid passing NULL to the methods; this can generate NullPointerExceptions.
8. Null is not empty and not an error, instead Null is a value.

## Tests
1. One assert per test.
2. Readable.
4. Follow TDD
5. Keep your test clean.
6. The tests must undergo changes in the same way that the code.
7. Use the F.I.R.S.T rule for testing:
	* Fast-running.
	* Independent
	* Repeatable in various environments.
	* Self-validating.
	* Timely.

## Design rules
1. Keep configurable data at high levels.
2. Prefer polymorphism to if/else or switch/case.
3. Separate multi-threading code.
4. Prevent over-configurability.
5. Use dependency injection.
6. Follow Law of Demeter. A class should know only its direct dependencies.
7. Recognize and separate the responsibilities of a system.

## Understandability tips
1. Be consistent. If you do something a certain way, do all similar things in the same way.
2. Use explanatory variables.
3. Encapsulate boundary conditions. Boundary conditions are hard to keep track of. Put the processing for them in one place.
4. Prefer dedicated value objects to primitive type.
5. Avoid logical dependency. Don't write methods which works correctly depending on something else in the same class.
6. Avoid negative conditionals.
7. Look to cover tests each line of code
8. No code is immune to improvement, refactor and make it better
9. Try not to let the code rot. It is much cheaper to create a clean code than cleaning a rotten code
10. There is always time to refactor then to refactor after getting rot or finding some issue in it.

## Refactor
* Write test that fails
* Make the test pass
* (Refactor) Make the code better
1. Before making any kind of refactoring, it is important to have good coverage tests.
2. After increasing or creating test coverage, you can begin to leave the clearest code and fix some bugs.
3. Now, after leaving the code clearer, someone else can probably clean it even more.
4. Follow TDD whenever wherever possible.

## Code smells
1. Rigidity. The software is difficult to change. A small change causes a cascade of subsequent changes.
2. Fragility. The software breaks in many places due to a single change.
3. Immobility. You cannot reuse parts of the code in other projects because of involved risks and high effort.
4. Needless Complexity.
5. Needless Repetition.
6. Opacity. The code is hard to understand.

References:
https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29  
https://dzone.com/articles/clean-code-summary-and-key-points  
https://kingadesign.com/clean-code-poster-free-download  
https://amzn.to/2ZQyX22  
https://www.oreilly.com/library/view/clean-code/9780134661742/  

Feedback and suggestions are always welcomed.