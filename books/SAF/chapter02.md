# Architectural Thinking
There are four main aspects of thinking like an architect:<br>
- understanding the differences between architecture and design and knowing how to collaborate with development to make architecture work.<br>
- having a wide **breadth** of technical knowledge while still maintaining a certain level of technical **debth** allowing the architect to see solutions others cant see.<br>
- understanding, analyzing and reconciling trade-offs between difference solutions and technologies.<br>
- understanding the importance of business drivers and how they drive architectural concerns.<br>
<br>

## Architecture vs Design

traditionally: architect is responsible of things like analyzing business requirements to extract and define the architectural characteristics (-ilities). selecting which artitecture patterns and styles would fit the problem domain.<br>
the artifacts created from these activites are then handled to development which is responsible for creating class diagrams for each component, creating user interfaces, and developing and testing source code.<br>
several issues arise with this: decisions an architect makes sometimes never make it to development, and decisions made by development that change the architecture rarely get back to the architect.<br>
design and architecture are both part of the circle of life within a software project and must always be kept in synchronisation with each other in order to succeed.<br>

## Technical Breadth
an individual can partition all their knowledge into three sections: stuff you know, stuff you know you don't know and stuffs you don't know you don't know.<br>
- **stuffs you know** includes tools a technologist uses on the daily basis to do their job.<br>
- **stuffs you know you don't know** are technologies you heard of but have little or no exprience with. for example closure language.<br>
- **stuffs you don't know you don't know** the largest part of the knowledge triangle, includes the intire host of technologies, tools, frameworks and languages that would a perfect solution to a problem a technologist is trying to solve. but the technologist does not even know they exist.<br>

the most important parts of the pyramid to the architect are the top and middle sections, the more the middle section penetrates into the bototm section defines the technical breadth of the architect.<br>
as an architect, breadth is more important than depth, because an architect has to make decisions that match capabilities to technical constraints, a broad understanding of a variety of solutions is valuable.<br>

## Understanding Business Drivers
understand business drivers that are required for the success of the system and translating those requirements into architecture characteristics. (scalability, performance and availability).<br>

## Balancing Architecture and Handson Coding
a software architect should be able to code and maintain a certain level of technical depth.<br>
the architect must avoid becoming a bottlenech to team. that occurs when the architect has taken ownership of code within the critical part of the system (usually the underlying code of the framework).<br>
to avoid this the architect should delegate the critical framework code to the team and focus on coding a piece of business functionality. three positive things happend by doing this:<br>
- architect is gaining hands-on experience writing production code.<br>
- the ownership of the ciritcal framework code is given to the team, where it belongs.<br>
- the architect is writing the same business code as the development team and is therefore better able to identify with them in terms of pains they might be going through with processes, procedures, and the dev environment.<br>
<br>

- doing frequent proof of concept helps validate architecture decisions by taking the implmenetation details into account.<br>
- takle some of the technical debt stories or architecture stories freeing up the team to work on critical functional user stories.<br>
- working on bug fixes is another way of maintaining hands-on coding while helping the dev team.<br>
- leverageing automation by writing simple command line tools to help the dev team with their day to day tasks is another great way to keep hands-on coding.<br>
- another way is to do frequent code reviews, it adds the benefit of ensuring compliance with the architecture and seek out mentoring and coaching opportunities on the team.<br>
