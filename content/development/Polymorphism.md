“Polymorphism” comes from a Greek word meaning “many-shaped”, it has two distinct aspects:

1. At run time, objects of a derived class may be treated as objects of a base class (in method parameters and collections or arrays). When polymorphism occurs, the object's declared type is no longer identical to its run-time type.
2. Base classes may define and implement virtual methods and derived classes can override them (they provide their own definition and implementation).

Polymorphism is exemplified in Dart by the presence of the `@override` meta tag. With it, the subclasses can implement an inherited behaviour in a specialised way that is more appropriate to its specific subtype.
> The `@override` meta tag helps you identify inherited methods or variables that are being overridden (replaced) in your subclass.

