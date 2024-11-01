---
layout: subpage-template
title: COMP367/MATH367: Programs and proofs with dependent types
hideheading: false
---
<style>
	i[class^="ri-"] { 
	color: #d9232d; 
	font-size: 24px; 
	vertical-align: sub; 
	/*padding-left: .2em; */
	padding-right: .2em 
}	
</style>

This page is a long-form course description, using a Q&A format.

**What will this course be like?**

We'll learn how to write programs in a language called [Agda](https://agda.readthedocs.io/en/latest/getting-started/what-is-agda.html), which is a "dependently typed" functional programming language. Agda is used for two main purposes: (1) writing verified computer programs, and (2) writing formal mathematical proofs.

A "verified" computer program is a program that carries with it a proof of correctness. You can think of this as an alternative to traditional unit testing--instead of testing that your program passes certain tests, in Agda you can prove that your program is correct. Your proof is not separate from your code; it is part of it, and the compiler checks your proof as part of the process of compiling your code.

A "formal" mathematical proof is a proof written in a formal language (in our case, as Agda code). You can express any mathematical definition or theorem statement as an Agda type, and you can write a proof of a theorem as Agda code. In contrast to informal (written) mathematical proofs which may contain errors, an Agda proof can be checked by running the Agda type-checker, so we can be confident of its correctness.

The main goals of the course are to learn how to write both verified computer programs and formal mathematical proofs in Agda, and to understand how this all works.

In terms of the structure of the class, the work will be centered around programming projects, along with some written homework assignments. Towards the end of the semester, we'll likely have a final programming project where you'll get to choose a topic. We'll likely have at least one midterm exam and possibly also a final exam.

**What are some major successes using Agda or similar languages?**

For a CS example, the [CompCert](https://compcert.org/) C compiler is a certified C compiler. It compiles C code to machine language, and comes along with a proof that the compiler preserves the behavior of your code, according to the C language specification and the processor specification.

For a math example, the [Kepler conjecture](https://en.wikipedia.org/wiki/Kepler_conjecture) was a 17th-century conjecture that the most space-efficient way to pack spheres is using a triangular pyramid pattern. This was proved in 1998 by Thomas Hales, but his proof was disputed by the mathematical community, as the details were hard to verify. In 2014, Hales and collaborators produced a computer-checked proof.

**What is the Agda language like?**

Agda is very different than most mainstream programming languages (e.g., Python, Java, C). Like these languages, Agda has expressions that are evaluated (e.g., 1 + 2 evaluates to 3). Unlike these languages, Agda has no statements that are executed; in particular, there are no if-statements or loops. Instead of if-statements, you use "pattern matching," and instead of loops, you use recursion. There are no objects or methods.

All of the above could be said not only about Agda but any functional programming language (e.g., ML or Haskell). Agda's unique feature is its type system, which allow "dependent types." This means that types can depend on values, for example, you can define a type "List Int n" which represents a list with n elements--this is not possible in most languages, which have a strict separation between types and terms. Agda's type system is really what allows Agda to be used for writing verified software or formal proofs.

From a math perspective, you might be wondering how writing a proof in Agda compares to writing a proof on paper. It's similar, in that the same proof ideas still apply--you can use cases, or induction, or use one theorem to prove another. It's different in that you can't skip details, since Agda must be able to check your proof. It's also different in that Agda uses what's called constructive logic by default, which means you can't use a proof by contradiction unless you enable it using an axiom.

**What's the practical benefit of taking this course?**

If you're a CS student, you'll learn how to write verified software. Proving correctness of code is not common in industry now, but there's a good chance it will become more common, and then you'll have an advantage. More immediately, learning to program in a language like Agda will make you a better programmer in more mainstream languages, which are increasingly adding features inspired by functional & dependently typed languages.

If you're a math student, you'll learn how to use a computer system to write proofs, which may be helpful, especially if you're doing math research. Also, likely, the proofs you've written up to this point have used "classical logic," and you might also be familiar with set theory as a foundation for math. In Agda you'll be working in a system based on type theory rather than set theory, and you'll be working with constructive rather than classical logic. This course will give you an opportunity to think about and understand the foundations of math, and also to recognize the tradeoffs between different logical systems.

In terms of academic requirements, the course counts as an upper-level "applications" elective in CS and an upper-level "proofs" elective in math.

**How do I know if I'm a good fit for this course?**

The prerequisites for the course are COMP142 & COMP172/MATH201, but essentially, you should have some experience with writing programs and some experience with writing proofs. If you do, and if you like thinking about how programming languages work or about why mathematical theorems are true, then you will enjoy this class.

Agda is very different from languages we teach in our introductory CS sequence, so we'll be starting from the very basics. In some ways, it will feel like learning programming for the first time again, and you'll be learning alongside other students who are in the same position. Please reach out to me (Dr. Superdock) if you have questions!

