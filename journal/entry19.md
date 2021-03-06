# Entry 19

## May 1

# Exam Two Explorations

Going over the second exam was extremely helpful for building my knowledge of Haskell more deeply, especially with the complex Monad and Co. classes, and their laws. I also learned more about the record syntax, and the conception of a Stack in Haskell using that record syntax.

The Stack question initially frustrated me because it was framed like there must only be one data constructor. I thought I had to come up with a single data constructor that encompassed all of the functionality of the Stack recursively, which immediately confused me because I thought there had to have been a base case in order to bottom everything out. Otherwise the recursion would be infinite, just like an infinite list.

I don't think that the test-by-class-consensus was very effective, even though some students seemed to take the reigns and tried to direct the class in the right direction. I think some people felt too alienated or peevish by their more brazen counterparts to participate or understant effectively, and I don't think that giving the class "hot or cold" directions really helped much either. I found that spending a lot of time using GHCI and playing around with actual code helped me learn the best. I encourage more tests that allow students to use the actual tools they're supposed to be using when learning something as complex as Haskell to their benefit. I understand that students are supposed to understand the foundation, much of which is hidden away by GHCI in many ways. It is invaluable, however, to allow students to solve problems using the problem solving tools (GHCI) they will be given in the "real world."

I realized my misunderstanding of the Stack was fundamentally to do with the base case, as well as how record syntax actually creates a data constructor. I did not understand the fact that the function names within the curly braces also stood as parameters for the data constructor. I didn't realize that the data constructor itself could not be constrained (that had to be done in the type constructor). Overall, I learned a lot about the actual way to use record syntax, which had not really been needed for Kattis before.

The other tricky question was the multiple implementations of `any` using the various folds. I know `fold` is an important set of functions within Haskell, and understanding its differences can help navigate implementation and performance issues alike, however it was really tricky and seemed a bit tedious to figure out. The `flip` for the `foldl` implementation was a bit frustrating, becuase I expected it to be more complicated than just literally flipping the arguments. The question mentioned that one might need to use `flip`, however based on the vague hints on other questions, surely a `flip` would not be all? Nay, in this instance, the problem hint was literally the answer, which was a bit infuriating, but alas, I eventually got it.

See my `test` folder for exam 2 explorations.