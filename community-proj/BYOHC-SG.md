# Building Your Own Haskell Compiler (SHC: Singapore Haskell Compiler)

## Goal

* Learning by implementing it.
* You have your own compiler to hack on. 
* Don't overly focus on performance and optimization, as long as it is correct.
* Know Haskell compiler better.
* Having a Haskell compiler grows from local.


## Requirement

* Knowing Haskell is not a requirement, it's a community effort and we would help you pick up the language.
* Know how to program, passionate to hack.


## How does it work

* We would decide the expectation of the progress before next meetup. It could be paper reading or implementation.
* The speed could be coordinated, ideally it should be at the tempo where everybody doesn't feel stressful.
* The roadmap is not fixed, since it is a task that even organizers need to learn along the way.



## Roadmap

- Untyped Lambda Calculus Interpreter
  - Implement an untyped lamda calculus interpreter
    - Understand the glossary (what is untyped lambda calculus, normal form)
    - Implement a UCLi
    - Normal order evaluation strategy
    - The target could be decided later.

  - Adding build-in types and annotations to UCLi 
    - No typechecking, assuming the inputs are correct
    - Build-in type are not in the form of lambda calculus
    - Understand what is head normal form
  
  - Foreign Function Interface 
    - Bring in the side effect
    - It would become Turing Complete, you would be able to program anything you want

- Frontend of Haskell Compiler
  - Parsing Haskell (Using haskell-src-ext)
    - Making sure the following Hello World could be parsed

      ```
      main = putStrLn "Hello World"
      ```


  - Support Different Phases of Compilation (`desugar`, `type inference`)

    - We would start to collect sample programs as the test cases.
    - Annotate each `expr` and `binding` with type signature
    - Implement type inference, type check
    - Implement type class, type instance
    - Implement `import`, `export`

- Code Gen to ULC
  - With this step so that we have a full-functional compiler.

- Runtime System

  - STG (Spineless Tagless G-Machine)
  - Garbage Collection

- Standard Library


## Collaboration
* This community project is different from others, since this project is actually launched by CindyLinz in the Taiwan Haskell community. I thought it is a good chance to make two small communities to have contact with each other.
* For Taiwanese community, [gitter](https://gitter.im/CindyLinz/BuildYourOwnHaskellCompiler) has already been chosen.
* We would start by gitter collaboration for now, since the English speaking for Taiwanese community might be a concern, but chatting by text should be no problem. If it goes well, then we could consider video collaboration.
* The Singapore community's progress would be independent on Taiwan's community's progress.
* For offline meetup, we would stick to Singapore community alone at Hackerspace. 
