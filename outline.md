The Algebra of Types
--------------------

1. What is an Algebra
   - Symbols, Operations and Laws
   - What is Cardinality?
   - Calculating Cardinality for various types
2. Sum types
   - Calculating the cardinality of a Sum type
3. Product types
   - Calculating the cardinality of a Product type
4. Functions
   - Calculating the cardinality of a Function type
5. Converting between types
   - Isomorphism (non-lossy conversions)
   - Lossy conversions
6. Discoveries
   - Composition
7. Caveats
   - When you have large cardinalities it is hard to reason about a solution. Eg. Having two Int values.


Thoughts

- Speak more about Laws and the derivations they lead to


Questions

- What is the cardinality of a function with more than one parameter?

  TrafficLight -> Directions -> Bool
   1                    2        2

   (2 ^ (2)) ^ 1

   RED NORTH TRUE
   RED SOUTH TRUE
   RED EAST  TRUE
   RED WEST  TRUE
   RED NORTH FALSE
   RED SOUTH FALSE
   RED EAST  FALSE
   RED WEST  FALSE

   4 ^ 3 = 64

   params = add cardinality of all params together
   cardinality for function = result ^ params

Optional

1. Recursive types
