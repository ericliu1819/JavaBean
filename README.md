# JavaBean
# Introduction
Visual Programming Languages (such as Visual Basic and Delphi) have been very popular in building GUI applications. In visual programming, you can drag and drop a visual component into a Application Builder and attach event handler to the component. Visual programming is ideal for rapid prototyping of GUI applications. Visual programming relies on component and event-driven technology. Components are reusable software units that can be assembled into an application via an application building tool (e.g., Visual Studio, JBuilder, NetBeans, Eclipse).
In Java, visual programming is supported via the "Javabean" API. The application builder tool loads the beans into a "toolbox" or "palette". You can select a bean from the toolbox, drop it into a "form", modify its appearance or properties, and define its interaction with other beans. Using the JavaBeans component technology, you can compose (or assemble) an application with just a few lines of codes.

"A Javabean is a reusable software component that can be manipulated visually in an application builder tool."

"A Javabean is an independent, reusable software component. Beans may be visual object, like Swing components (e.g. JButton, JTextField) that you can drag and drop using a GUI builder tool to assemble your GUI application. Beans may also be invisible object, like queues or stacks. Again, you can use these components to assemble your application using a builder tool."

Javabeans expose their features (such as properties, methods, events) to the application builder tools for visual manipulation. These feature names must adhere to a strict naming convention in order for them to be examined automatically. In other words, an application builder tool relies on these naming conventions to discover the exposed features, in a process known as introspection. For examples,

# Writing Your Own Javabeans
The JavaBeans APIs covers five aspects:

1.Properties: represent the attributes of a component.
2.Event Handling: allows beans to communicate with each others (JavaBean uses JDK 1.1 AWT event-delegation model).
3.Persistence: allows beans' internal states to be stored and later restored.
4.Introspection: allows Application Builder tool to analyze beans.
5.Application Builder Tool: for composing applications from Javabeans components.
# Property:
A bean has properties, which define the attributes of the bean, and can be manipulated by an application builder tool.
Javabean Property Naming Convention: For a property called propertyName of type PropertyType, a getter and a setter method must be defined as follows:

private PropertyType PropertyName               // declare
public PropertyType getPropertyName()           // getter
public void setPropertyName(PropertyType value) // setter

For properties of boolean type, the getter shall be:

private boolean PropertyName
public boolean isPropertyName()                 // getter for boolean property
public void setPropertyName(boolean value)      // setter

# javac -d target/classes src\elect\*.java
