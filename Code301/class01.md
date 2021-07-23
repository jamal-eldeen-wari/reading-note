# Component Based Architecture:
It is a modular, portable, replaceable and reusable set of functionality that encapsulates its own Implementation  and exporting it as a higher-level interface. Also it known as a **Software Object**. What makes components unique is that they have an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

## Views For Component:
 1. Object-oriented View: It is viewed as a set of one or more cooperating classes. Where each problem domain class  and infrastructure class are explained to identify all **attributes and operations** that apply to its implementation.So combining domain class and infrastructure class will result of all attributes and operations.

 2. Conventional View: It is a viewed as a functional element or a module of a program that integrates the *processing logic*, the internal data structures that are required to implement the processing logic.

 3. Process-Related View: This view focuses on building from existing components maintained in a library rather than creating each component from scratch. As the software architecture is formulated, components are selected from the library and used to populate the architecture.

## Important Charateristics for Component Based Architecture:
1. Reusability: Components are usually designed to be reused in different situations in different applications. 
2. Replaceable: Components may be freely substituted with other similar components.
3. Extensible: A component can be extended from existing components to provide new behavior.
4. Encapsulated: Where it allows the user to use the functionality but not having the ability to access the internal processes or any internal variables or state.
5. Independent: Components are designed to have minimal dependencies on other components.

## Advantages of using component based architecture: 
 1. Ease of deployment.
 2. Reduced cost.
 3. Ease of development. 
 4. Reusable.
 5. Modification of technical complexity.
 6. Reliability.
 7. System maintenance and evolution.
 8. Independent.

 # Props Stands for:
 It is a special keyword used in React and stands for **Properties** that are used *passing data from one component to another*. The data in the props are read only that means that data comming from the parent could not be altered by the child.

 # How to use Props in React:
  1.  By defining an attribute and its value(data).
  2. Then pass it to child component(s) by using Props
  3. Render the Props Data

# Data flow in Props:
Most important note here is that the data flow in the Props is **a uni-directional flow** which means from parent to child.

### Things I Want To Know More About:
* Data flow in props how does it work exactly