# Homework 01

## Define the term essential difficulties as it is used by Brooks. Provide background and context with your answer and at least one example of an essential difficulty.
According to the definition from Brook's article, the essential difficulties results from the fast progress of hardware and the irreducible essence of modern software system. Essential difficulties reflects the difficulties from nature of software.\
Take China's great firewall as an example, it blocking some websites like Facebook, Youtube, Twitter, etc. Some applications is related to accounts authentication of these websites while cannot be used in China, but Chinese people want to use similar apps' authentication, so they must have different versions to avoid this problem. Also, take Evernote as another example, it runs on a different server in China so the version of the app is different when you download with different countries settings although they actually is 'the same' app. Therefore, Apple store deals with this by specifing user's regions which sell different applications.

## Define the term accidental difficulties as it is used by Brooks. Provide background and context with your answer and at least one example of an accidental difficulty.
Accidental difficulties means the difficulties that attacked by those three steps of software technology development, it reflects the problems of the production of software.\
A web application is developed with Groovy using Ember as front-end framework a few years ago. The development team decided to switch to Django framework because of it has some built in feature they need which grails doesn't have, the admin system, for example. However, during the development process, it brought new problems such as Django's CSRF protection while making post requests.

## List and briefly describe the four essential difficulties of developing software systems that Brooks identifies. Provide additional examples of each type of the four essential difficulties.
1. complexity
    * Software entities are more complex than their size.
    * Digital computers have a huge number of states so themselves are more complex than things built by people.
    * As the size of a system increases, both number and types of parts increases exponentially.
    * The application domain can't be abstract away
    * These domains are intrinsically complex and this complexity will appear in the software system as designers attempt to model the domain.
2. conformity
    * Comformity means software must be conform to arbitrary changes such as the environment or user requirements.
3. changeability
    * Software is frequently asked to change. A successful software must survival from such changes and is able to extends with newly added functionality.
4. invisibility
    * Software can't be represent by graph or any other visualization methods. A single kind of diagram can only convey some aspects of the software instead of all. They are actually unreadable binaries running on computers.

- complexity: 
    - Railway system: A railway system has elements of trains, passengers, stations, railways, schedules, etc. The rules between these elements can be, how many trains can run on a specific railway, how long shoud it be when a train left and the next train comes to a station, how many cars should a train has in differernt period of a year to meet the number of passengers and so on, which is very complicated.

- conformity
    - A new version of operating system, windows for example is released, software must changed in order to be compatible with different versions of operating system.

- changeability
    - An example of this would be WeChat, a chatting app widely used in China. When this application is first released, it mainly supports the functionaility of adding friends and sending messages to each other. As user sends their feedback to the development team, it gradually extends with more and more features such as quickpay, self-made stickers, voice messages, location sharing, video chatting and so on.

- invisibility
    - Take class diagram as an example, which I think contains the most parts of structures of a software. It shows the elements that made up the logic, the relationship between elements, the methods under each class. Nevertheless, it only visualize the structure of software. It is not able to show the sequence of a use case, the use cases that a software has, or the workflow which is shown in activitity diagram.
## Define what Brooks means by a silver bullet and reconstruct his argument as to why he believes there is no silver bullet for software engineering.
Technical developments to make software costs drop as rapidly as computer hardware costs do.\
Based on the definition of silver bullet, to improve software development, two arguments must be satisfied.
- Accidents of software engineering must account for 90% of the overall effort
- The technique would have to reduce accidental problems to zero.

However, Brooks thinks the domainted part of overall effort results from essential difficulties rather than accidental ones. Secondly, although we might have such tool that solve current problems, it would bring new problems simultaneously.

## In lecture, software engineering's relationship to computer science was described by analogy by discussing the differences between a chemist (chemistry) and a chemical engineer (chemical engineering). Define software engineering and its relationship to computer science; make use of the chemist vs. chemical engineer analogy when answering this question.
Software engineering is to develop the application of computer programs. It usually follows the steps: design, implement, complie, debug and test. A software is designed with use cases, UML diagrams, user requirements and so on. Then software engineers use software techniques, such as frameworks, tools, programming languages to code the program and debug it so that the program can be implemented. Then, they write test cases to to test the program and verification progrmas so that the product can be put into pratical use. To apply computer programs to real world usage, software engineers need to consider the budget and efficiency. Therefore, they borrow knowledge including algorithms, data structure, frameworks which have been proved by computer scientists. Just like chemists think of an idea of converting salt water into drinkable water, computer scientists specialize in different areas think of a well performance machine learning algorithm with high accuracy, an effcient search algorithm, a new distribut system, detection shortcomings of current programming languages or frameworks etc., and develop a new version to improve it. Their work is done after prove their method is correct and applicable. Then software engineers pick up what they need from existing methods to build up the real tool or application which can be used by other people in many fields as well as computer science. This is just like chemical engineer considers how to implement the conversion and the budgets or potential problems.

## In lecture, we discussed the importance of the following concepts to software engineers: abstractions, conversations, specification, translation, and iteration. Define each of these concepts as they are related to software engineering and discuss their importance.
#### Abstractions
This is one of the way of software engineers solve problem, they split the whole problem into some smaller problems that is understandable or using abstractions developed by others.\
This is important because usually a general problems is hard to solve within a short time and a simple step, however, it contains several parts which can be solved one by one. For example, the problem of designing a social graph, which can be break down into three detailed parts: a list of user ids and the ids that they follow, a list of user ids and ids that following them and a list of ids and the information objects corresponds to that id. This makes solution is clear at a data structure level which can make coding easier. By building up these small problems the original problem is solved.

#### Conversations
Conversations refers to the interaction between not only the developers but documentations, abstractions and testing cases as well.\
Conversations are evitable especially when you are in a team. For example, you need to communicate with others to know their progress, the problem that the team met to make sure members are working synchronized. We need conversations on-line to have a better understanding of documentations written by other developers. Also, we need conversations with test cases to make sure abstractions is working. You are never alone during software development so conversations are important.

#### Specification
The specification of software engineering refers to provide the detail of everything of software development. That is, list the exact requirements (user requirements, business requirements, project requirements, functional and non-functional requirements), design diagrams of a project in order to solve a problem, choose specific languages based on the goals to achieve, write test plans for each potential bugs, make a schedule of what you achieve today and what you can deliver this week.
Specification is important since a good design makes implementation much more efficient. You list all kinds of requiremnts so that the final product meets all of them which can satisfy clients. When consider the whole class diagrams, you form a whole picture of the structure and reduce refactor as well. When start implementing, specify the same version of framework, programming languages and anything else to make the code more organized especially working in a team. Specify test plans make the product robust to as much as possible problems and help developers to improve it. Make a plan of development life cycle helps developer to build up the program step by step so that they won't lost direction or waste time on unnecessary trival things.

#### Translation
The process of moving from one specification to another, from one set of structures to another and from one level of abstraction to another. This will forms a pipeline like of work that you convey until the final finished version. This makes the development more organized.

#### Iteration
The development can't be done at one time. Instead, there are a bunch of versions which is the result after discussing with clients in order to meet the requirements and help them think more specific about the logic of design and what they want exactly. So we need to iterate this process to modify the current version and meet the next goal, this is the definition of iteration.
Iteration is important because even clients don't know exactly what they want in the beginning, usually they describe a high level of expectation of the product's functionality and software developers needs to discuss with them when designing the logic of data model, UI design, algorithms needed, etc. So the work needs to be iterate and iterate to reach the requirements and full functionality.
