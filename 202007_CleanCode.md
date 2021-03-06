# Clean Code: A Handbook of Agile Software Craftsmanship
> In about 1951, a quality approach called Total Productive Maintenance(TPM) came on the Japanesse scene. Its focus is on maintenance rather than on production. One of the major pillars of TPM is the set of so-called 5S principles. 

> Seiri, or organization (think "sort" in English). Knowing where things are -- using approaches such as suitable naming -- is crucial.

> Seiton, or tidiness (think "systematize" in English). There is an old American saying: *A place for everything, and everything in its place.* A piece of code should be where you expect to find it -- and, if not, you should re-factor to get it htere. 

> Seiso, or cleaning (think "shine" in English): Keep the workplace free of hanging wires, grease, scraps, and waster. What do the authors here say about littering you code with comments and commented-out code lines that capture history or wishes for the future? Get rid of them. 

> Seiketsu, or standardization: The group agrees about how to keep the workplace clean. Do you think this book says anythin about having a consistent coding style and set of practices within the group? Where do those standards come from? Read on. 

> Shutsuke, or discipline (self-discipline). This means having the discipline to follow the practices and to frequently reflect on one's work and be willing to change.

> As we maintain automobiles and other machines under TPM, breaking-down maintenance -- waiting for bugs to surface -- is the exception. Instead, we go up a level: inspect the machiens every day and fix wearing parts before they break, or do the equivalent of the proverbial 10,000-mile oil change to forestall wear and tear. 

> In code, refactor mercilessly. You can improve yet one level further, as the TMP movement innovated over 50 years ago: build machines that are more maintainable in the first place. Making your code readable is as important as making it executable. 

### References: 

#### SRP: The Single Responsibility Principle 
#### DIP: Dependency Inversion Principle

- High-level classes must not depend on low-level classes, but both on interfaces.
- Interfaces must not depend on details, but details on interfaces.
#### OCP: Open Closed Principle
A class is open for enhancements but closed against modifications.
#### LSP: Liskov Substitution Principle
A subtype behaves same as its base type.
#### ISP: Interface Segregation Principle
Clients shall be not confused with details which they do not need.
#### TDD: Test Driven Development
Three laws:
1. You are not allowed to write any production code unless it is to make a failing unit test pass.
2. You are not allowed to write any more of a unit test than is sufficient to fail, and compilation failures are failures.
3. You are not allowed to write any more production code than is sufficient to pass the one failing unit test.

## Chapter 1: Clean Code 
### There Will Be Code 
### Bad Code 
### The Total Cost of Owning a Mess 
  #### The Grand Redesign in the Sky 
  #### Attitude 
  #### The Primal Conundrum 
  #### The Art of Clean Code? 
  ### What Is Clean Code? 
### Schools of Thought 
### We Are Authors 
### The Boy Scout Rule 
### Prequel and Principles 
### Conclusion 

## Chapter 2: Meaningful Names 
### Introduction 
### Use Intention-Revealing Names 
### Avoid Disinformation 
### Make Meaningful Distinctions 
### Use Pronounceable Names 
### Use Searchable Names 
### Avoid Encodings 
#### Hungarian Notation 
#### Member Prefixes 
#### Interfaces and Implementations 
### Avoid Mental Mapping 
### Class Names 
### Methods Names 
### Don't Be Cute 
### Pick One Word per Concept 
### Don't Pun
### Use Solution Domain Names 
### Use Problem Domain Names 
### Add Meaningful Context 
### Don't Add Gratuitous Context 
### Final Words 


## Chpater 3: Functions 
### Small! 
#### Blocks and Indenting 
### Do One Thing
#### Sections within Functions 
### One Level of Abstraction per FUnction 
#### Reading Code from Top to Bottom: The Stepdown Rule 
### Swithc Statements 
### Use Descriptive Names 
### Function Arguments 
#### Common Monadic Forms 
#### Flag Argument 
#### Dyadic Funtions
#### Triads 
#### Argument Objects 
#### Argument Lists 
#### Verbs and Keywords 
### Have No Side Effects 
#### Output Arguments 
### Command Query Separation 
### Prefer Exceptions to Returning Error Codes 
#### Extract Try/Catch Blocks 
#### Error Handling Is One Thing
#### The ERror.java Dependency Magnet 
### Don't Repeat Yourself 
### Structured Programming 
### How Do You Write Functions Like This? 
### Conclusion 
#### SetupTeardownIncluder 

## Chapter 4: Comments 
### Comments Do Not Make Up for Bad Code 
### Explain Yourself in Code 
### Good Comments 
#### Legal Comments 
#### Informative COmments 
#### Explanation of Intent 
#### Clarification 
#### Warning of Consequences 
#### TODO Comments 
#### Amplification 
#### Javadocs in Public APIs
### Bad Comments 
#### Mumbling 
#### Redundant Comments 
#### Misleading Comments 
#### Mandated Comments 
#### Journal Comments 
#### Noise Comments 
#### Scary Noise 
#### Don't Use a Comment When You Can Use a Function of a Variable 
#### Function or a Variable 
#### Position Markers 
#### Closing Brace Comments 
#### Attributions and Bylines 
#### Commented-Out Code 
#### HTML Comments 
#### Nonlocal Information 
#### Too Much Information 
#### Inobvious Connection 
#### Function Headers 
#### Javadocs in Nonpublic Code 
#### Example 

## Chapter 5: Formatting 
### The Purpose of Formatting 
### Vertical Formatting 
#### The Newspaper Metaphor 
#### Vertical Openness Between Concepts 
#### Vertical Density 
#### Vertical Distance 
#### Vertical Ordering 
### Horizontal Formatting 
#### Horizontal Openness and Density 
#### Horizontal Alignment 
#### Indentation 
#### Dummy Scopes 
### Team Rules 
### Uncle Bob's Formatting Rules 

## Chapter 6: Objects and Data Structure 
### Data Abstraction 
### Data/Object Anti-Symmetry 
- Complimentary natures of theses two definitions; They are virtual opposites! 
- Objects expose behavior and hide data. This makes it easy to add new kinds of objects without changing existing behaviors. It also makes it hard to add new behaviors to existing objects. 
- Data structures expose data and have no significant behavior. This makes it easy to add new behaviors to existing data structures but makes it hard to add new data structures to existing functions. 
- the idea that everything is an object is a myth. Sometimes you really do want simple data structures with procedures operatin g on them. 
### The Law of Demeter 
- Methods should NOT invoke methods on objects that are returned by any of the allowed functions. 
- Talk to frinds, not to strangers. 
#### Train Wrecks 
#### Hybrids 
- Doom of hybrids: it's hard to add new functions and hard to add new data structures. Worst of both worlds. AVOID! 
#### Hiding Structure 
### Data Transfer Objects 
#### Active Record 
### Conclusion 

## Chapter 7: Error Handling 
### Use Exceptions Rather Than Return Codes 
### Write Your Try-Catch-Finally Statemnet First 
### Use Unchecked Exceptions 
### Provide Context with Exceptions 
### Define Exception Classes in Terms of a Caller's Needs 
### Define the Normal Flow
### Don't Return Null
### Don't Pass Null
### Conclusion 

## Chapter 8: Boundaries 
### Using Third-Party Code
### Exploring and Learning Boundaries 
### Learning log4j
### Learning Tests Are Better Than Free
### Using Code That Does Not Yet Exist 
### Clean Boundaries 

## Chapter 9: Unit Tests 
### The Three Laws of TDD
- First Law: You may not write production code until you have written a failing unit test. 
- Second Law: You may not write mroe of a unit test than is sufficient to fail, and not compiling is failing. 
- Third Law: You may not write more production code than is sufficient to pass the currently failing test. 
### Keeping Tests Clean 
#### Tests Enable the -ilities 
### Clean Tests 
Readability 

The BUILD-OPERATE-CHECK pattern 
#### Domain-Specific Testing Language 
- Build up a set of functions and utilities that make use of those APIs and that make the tests more convenient to write and easier to read. 
- This testing API is not designed up front; rather it evolves from the continues refactoring of test code that has gotten too tainted by obfuscating detail. 
#### A Dual Standard 
### One Assert per Test 
#### Single Concept per Test 
### F.I.R.S.T. 
### Conclusion 

## Chapter 10: Classes 
### Class Organization 
#### Encapsulation 
### Classes Should Be Small! 
#### The Single Responsibility Principle 
SRP states that a class or module should have one, and only one, reason to change. This principle gives us both a definition of responsibility, and a guidelines for class size. Classes should have one responsibility -- one reason to change. 

SRP is one of the more important concept in OO design. 
#### Cohesion 
#### Maintaining Cohesion Results in Many Small Classes 
### Organizing for Change 
#### Isolating from Change 

## Chapter 11 Systems
### How Would You Build a City?
### Separate Constructing a System from Using It
#### Separation of Martin 
#### Factories 
#### Dependency Injection 
### Scaling Up 
#### Cross-Cutting Concerns 
### Java Proxies 
### Pure Java AOP Frameworks 
### AspectJ Aspects 
### Test Drive the System Architecture
### Optimize Decision Making 
### Use Standards Wisely, When They Add Demonstratable Value 
### Systems Need Domain-Specific Languages

## Chapter 12: Emergence 
### Getting Clean vis Emergent Design
### Simple Design Rule 1: Runs All the Tests
### Simple Design Rule 2-4: Refactoring
### Simple Design Rule 
#### No Duplication 
#### Expressive 
#### Minimal Classes and Methods 

## Chapter 13: Concurrency
### Why Concurrency? 
#### Myths and Misconceptions 
### Challenges 
### Concurrency Defense Principles 
#### Single Responsibility Principle 
#### Corollary: Limit the Scope of Data
#### Corollary: Use Copies of Data
#### Corollary: Threads Should Be as Independent as Possible 
### Know Your Library
#### Thread-Safe Collections 
### Know Your Execution Models 
- Producer-Consumer
- Readers-Writers 
- Dining Philosophers 
Most concurrent problems you will likely encounter will be some variation of these three problems. Study these algos and write solutions using them on your own so that when you come across concurrent problems, you'll be more prepared to solve the problem.
#### Producer-Consumer 
#### Readers-Writers 
#### Dining Philosophers 
### Beware Dependencies Between Synchronized Methods 
### Keep Synchronized Sections Small
### Writing Correct Shut-Down Code Is Hard 
### Testing Threaded Code 
#### Treat Spurious Failures as Candidate Threading Issues 
#### Get Your Nonthreaded Code Working First 
#### Make Your Threaded Code Pluggable 
#### Run with More Threads Than Processors 
#### Run on Different Platforms 
#### Instrument Your Code to Try and Force Failures 
#### Hand-Coded
#### Automated 
### Conclusion 
### Bibliography

## Chapter 14: Successive Refinement 
