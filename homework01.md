# Homework 01
###### Yue ZHANG

### Question 1
### Define the term essential difficulties as it is used by Brooks. Provide background and context with your answer and at least one example of an essential difficulty.

The essential difficulties results from the fast progress of hardware and the irreducible essence of modern software system, which can be elaborated from four aspects: complexity, conformity, changeability and invisibility. Essential difficulties are caused by the properties of software itself.

> Following Aristotle, I divide them into essence, the difficulties inherent in the nature of software, ...
> -Frederick P. Brooks, Jr. \[[1](#ref1)\]

**Example:** Take China's great firewall as an example, it blocking some websites like Facebook, Youtube, Twitter, etc and thus coming with some essential difficulties. Some applications is related to accounts authentication of these websites while cannot be used in China, but Chinese people want to use other apps' authentication, so they must have different versions to avoid this problem. Also, take Evernote as another example, it runs on a different server in China so the version of the app is different when you download with different countries settings although they actually is *'the same'* app. Therefore, there must be some bug-fix process when applications are using in different regions.

### Question 2
### Define the term accidental difficulties as it is used by Brooks. Provide background and context with your answer and at least one example of an accidental difficulty.

Accidental difficulties means the difficulties that attacked by those three steps of software technology development, it reflects the problems of the production of software. The problem is generated because of a new tool is picked rather than the nature of software.

> Following Aristotle, ..., and accidents, those difficulties that today attend its production but are not inherent.
> -Frederick P. Brooks, Jr.

**Example:** A web application is developed with Groovy as back-end and Ember as front-end framework a few years ago. The development team decided to switch to Django framework because of it has some built in feature they need which grails doesn't have, the admin system, for example. However, during the development process, it brought new problems such as Django's CSRF protection while making post requests.

### Question 3
### List and briefly describe the four essential difficulties of developing software systems that Brooks identifies. Provide additional examples of each type of the four essential difficulties.
1. complexity
    * Software entities are complex.
    * Digital computers have a huge number of states so themselves are more complex than things built by people.
    * As the size of a system increases, problems increases exponentially and different elements interact in a non-linear fashion.
    * The application domain can't be abstract away due to complexity is an essential property.

2. conformity
    * Comformity means software must be conform to **arbitrary changes** such as the environment or user requirements.

3. changeability
    * Software is frequently asked to change since the cost of changing hardware is much more expensive, which causes the pressure on changing. A successful software must survival from such changes and is able to extends with newly added functionality.

4. invisibility
    * Software can't be represent by graph or any other visualization methods. A single kind of diagram can only convey some aspects of the software instead of all. They are actually unreadable binaries running on computers.

#### Examples:
- complexity: 
    - Railway system: A railway system has elements of trains, passengers, stations, railways, schedules, etc. The rules between these elements can be, how many trains can run on a specific railway, how long should it be when a train left and the next train comes to a station, how many cars should a train has in different period of a year to meet the number of passengers and so on, which is very complicated. Instead of touch everything, a software engineer must use abstraction to select the problems they need to solve, and break down them into smaller aspects.

- conformity
    - A new version of operating system, windows for example, is released, software must changed easily in order to be compatible with different versions of operating system.

- changeability
    - An example of this would be [WeChat](https://en.wikipedia.org/wiki/WeChat), a chatting app widely used in China. When this application is first released, it mainly supports the functionality of adding friends and sending messages to each other. As user sends their feedback to the development team, it gradually extends with more and more features such as quickpay, self-made stickers, voice messages, location sharing, video chatting and so on.

- invisibility
    - Take class diagram as an example, which I think contains the most parts of structures of a software. It shows the elements that made up the logic of software, the relationship between elements, the attributes and methods under each class. Nevertheless, it is only able to visualize the structure of software. It is not able to show the sequence of a use case, the use cases that a software has, or the workflow which is shown in activity diagram.
![Class Diagram of Social Media](http://i.stack.imgur.com/PrK90.jpg "Class Diagram of Social Media")

### Question 4
### Define what Brooks means by a silver bullet and reconstruct his argument as to why he believes there is no silver bullet for software engineering.
A silver bullet refers to technical developments to make software costs drop as rapidly as computer hardware costs do. In other words, to improve the development by a factor of 10.

Based on the definition of silver bullet, two arguments must be satisfied to support proving the existence of silver bullet:
- **Accidents** of software engineering must account for the domain part of the overall effort
- The technique would have to **completely** reduce accidental problems.

However, Brooks thinks the domainted part of overall effort results from essential difficulties rather than accidental ones. Secondly, although we might have such tool that solve current problems, it would bring new problems simultaneously. Therefore, Brooks belives there is no silver bullet.

### Question 5
### In lecture, software engineering's relationship to computer science was described by analogy by discussing the differences between a chemist (chemistry) and a chemical engineer (chemical engineering). Define software engineering and its relationship to computer science; make use of the chemist vs. chemical engineer analogy when answering this question.
Software engineering is to develop the application of computer programs. It usually follows the steps: design, implement, compile, debug and test. A software is designed with use cases, UML diagrams, user requirements and so on. Then software engineers use software techniques, such as frameworks, tools, programming languages to code the program and debug it so that the program can be implemented. Then, they write test cases to to test the program and verification progrmas so that the product can be put into pratical use. To apply computer programs to real world usage, *software engineers need to consider the budget and efficiency*. Therefore, they borrow knowledge including *algorithms, data structure, frameworks which have been proved by computer scientists*. 

Just like chemists think of an idea of converting salt water into drinkable water, *computer scientists* specialize in different areas think of a well performance machine learning algorithm with high accuracy, an effcient search algorithm, a new distribut system, detection shortcomings of current programming languages or frameworks etc., and develop a new version to improve it. Their work is done after prove their method is correct and applicable. Then *software engineers* pick up what they need from existing methods to build up the real tool or application which can be used by other people in many fields as well as computer science. This is just like chemical engineer considers how to implement the conversion and the budgets or potential problems.

### Question 6
#### In lecture, we discussed the importance of the following concepts to software engineers: abstractions, conversations, specification, translation, and iteration. Define each of these concepts as they are related to software engineering and discuss their importance.
#### Abstractions
This is one of the way of software engineers solve problem, they split a high level problem into some smaller problems that is understandable or using abstractions developed by others.

This is important because usually a general problems is abstract and hard to solve within a short time and a simple step, however, it contains several parts which can be solved one by one. For example, the problem of designing a social graph, which can be break down into three detailed parts: a list of user ids and the ids that they follow, a list of user ids and ids that following them and a list of ids and the information objects corresponds to that id. This makes solution is clear at a data structure level which can make coding easier. By building up these small problems the original problem is solved.

#### Conversations
Conversations refers to the interaction between not only the developers but documentations, abstractions and testing cases as well.

Conversations are everywhere especially when you are in a team. For example, you need to communicate with others to know their progress, the problem that the team met to make sure members are working synchronized. We need conversations on-line to have a better understanding of documentations written by other developers. Also, we need conversations with test cases to make sure abstractions is working. You are never alone during software development so conversations are important.

#### Specification
The specification of software engineering refers to provide the detail of everything of software development. That is, list the exact requirements *(user requirements, business requirements, project requirements, functional and non-functional requirements)*, design diagrams of a project in order to solve a problem, choose specific languages based on the goals to achieve, write test plans for each potential bugs, make a schedule of what you achieve today and what you can deliver this week.

Specification is important since a good design makes implementation much more efficient. You list all kinds of requirements so that the final product meets all of them which can satisfy clients. When consider the whole class diagrams, you form a whole picture of the structure and reduce refactor as well. When start implementing, specify the same version of framework, programming languages and anything else to make the code more organized especially working in a team. Specify test plans make the product robust to as much as possible problems and help developers to improve it. Make a plan of development life cycle helps developer to build up the program step by step so that they won't lost direction or waste time on unnecessary trivial things.

#### Translation
Translation happens from the start till the end of developing software. To view the process horizontally, it moves from one specification to another, from one set of structures to another and from one level of abstraction to another.\[[2](#ref2)\] For example, when one use case is done, move to the next. On the other hand, to view translation vertically, we move from write up requirements to deisgn diagrams, data models, algorithms. After this, it moves to implementation, then testing and debugging. This will forms a pipeline like of work that you convey until the final finished version.

This makes the development more organized and efficient.

#### Iteration
The development can't be done at one time. Instead, there are a bunch of versions which is the result after discussing with clients in order to meet the requirements and help them think more specific about the logic of design and what they want exactly. So we need to iterate this process to modify the current version and meet the next goal, this is the definition of iteration.

Iteration is important because even clients don't know exactly what they want in the beginning, usually they describe a high level of expectation of the product's functionality and software developers needs to discuss with them when designing the logic of data model, UI design, algorithms needed, etc. So the work needs to be iterate and iterate to reach the requirements and full functionality.

### References
1. <a name="ref1">Brooks, F. P. , J. (1987).</a>, D.L., <q>No Silver Bullet—Essence and Accidents of Software Engineering<q>
2. <a name="ref2">Kenneth Anderson</a>, D.L., <q>Lecture 01 slides<q>
