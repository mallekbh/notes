# Modularity
95% of words about software architecture are spent extolling the benefits of "modularity" and that little, if anything, is said about how to achieve it.<br>
different platforms offer different reuse mechanisms for code, but all support some way of grouping related code together into modules.<br>
modularity is an organizing principle. if an architect designs a system without paying attention to how the peices wire together, they end up creating a system that presents a myriad of difficulties. software systems model complex systems which tend toward entropy. (or disorder).<br>
preserving good modularity exemplifies our definition of implicit architecture characteristic: sustainable code bases require order and consistency.<br>
## Definition
dictionary defines it as: each of a set of standardized parts of independant units that can be used to construct a more complex structure.<br>
we use modularity to describe a logical grouping of related code, which could be a group of classes in an object-oriented language or functions in a structured or functional language.<br>
architects must be aware of how developers package things because it has important implications in architecture.<br>

## Measuring Modularity
researchers created a variety of language-agnostic metrics to help architects understand modularity. we focus on three key concepts: **cohesion, coupling and connascence.**<br>

### Cohesion
refers to what extent the parts of a module should be contained within a module. it is a measure of how related parts are to one another. ideally a cohesive module is one where all the parts should be packaged together, because breaking them into smaller pieces would require coupling the parts together via calls between modules to achieve useful results.<br>
<br>
**attempting to divide a cohesive module would only result in increased coupling and decreased readability.**<br>
<br>

computer scientists have defined a range of cohesion measures:<br>
- **Functional Cohesion:**<br>
every part of a module is related to the other, and the module contains everything essential to function.<br>
<br>
- **Sequential Cohesion:**<br>
two modules interact, where one output data that becomes the input for the other.<br>
<br>
- **Communicational Cohesion:**<br>
two modules form a communication chain, where each operates on infomation and/or contributes to some output.<br>
<br>
- **Procedural Cohesion:**<br>
two modules must execute code in a particular order.<br>
<br>
- **Temporal Cohesion:**<br>
modules are related based on timing dependencies.<br>
<br>
- **Logical Cohesion:**<br>
the data within modules is related logically but not functionally.<br>
<br>
- **Coincidental Cohesion:**<br>
elements in a module are not related other than being in the same source file, this represents the most negative form of cohesion.<br>
<br>
given the subjectivness of cohesion, computer scientists have developed a good structural metric to determine cohesion (or more specifically the lack of cohesion). a well known set of metrics named the Chidamber and Kemerer Object Oriented metrics suite.<br>
