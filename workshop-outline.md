# Workshop outline

Here we sketch out the basic outline of the materials/handout for the workshop.

We indentify below a set of subject areas/areas of competence relevant to the workshop.

The goal here should be that a participant can start with a question "How do I...",
read a short section, and move on. 
Short and concise trumps wordy, theoretical and complete.
We want a quick, reasonable answer, not necessarily the full details in each case.

**Keep it simple!**

The below is notes to help us plan, not the final format of the materials.

For each subject area we need:

* a choice of library, where the functionality isn't covered in base.
  
  We'll have to make sure the total set of libraries chosen all work together, and ideally isn't too large.
  
  In some cases it might be okay to list two, with a brief discussion of pros/cons.
  Just don't bamboozle them with choices. We want to cut short the ever-branching search for possibilities.
* code samples to get people started. Cargo culting is good!

  Code samples should contain
    - packages required 
    - imports required
    - language extensions required
    - clear illustrative code 
    - where relevant, console input and output

  e.g. 
  
  requires: `containers`
  
  ```
  {-# LANGUAGE OverloadedLists #-}
  
  import Data.Map (Map, union)
  
  m1, m2 :: Map String Int
  m1 = [("quota", 200), ("priority", 3)]
  m2 = [("capacity", 5000), ("quota", 100)]
  ```
  ```
  λ> m1 `union` m2
fromList [("capacity",5000),("priority",3),("quota",200)]
  ```


## Subject areas to cover

### Installation

### Cabal, cabal files, stack

### Specific setup relevant to our organisation
Working under a corporate proxy etc


### Basic language and syntax
* Lack of parens
* .
* $
* modules
* imports (incl. import style)
* basic types: Int, Word
* type synonyms
* data and newtype definitions
* records
* basic type classes: Eq, Ord, Show, Read
* deriving clauses



### REPL
Working with the repl

Typed holes 

PartialTypeSignatures


### Editor suggestions
Perhaps provide more than one, as participants are highly likely to already have a favourite.

Links to articles for each editor with setup instructions, and how to get

  * type info
  * case split
  * jump to definition
  * insert type signature
  etc

Maybe choose a default with easy setup e.g. Atom.
We can use this for demos in the workshop.

### Scripting with haskell
runhaskell, stack interpreter

`#!/usr/bin/env stack`


### Hoogle and Hackage


### Language extensions

Quickly define what they are, show syntax.
Listing of ~5 most common extensions


### Basic list manipulation
map

foldl'

intersperse

intercalate

join

monadic manipulations


### Basic data structures
maps, sets

arrays, vector?

Seq

### Shelling out
Turtle

### Command line parsing

optparse-applicative

getopts

### Text manipulation

Text/String/ByteString Lazy/Strict

uses for each and conversions between

string formatting

printf

### Time
time, thyme?

### Regular expressions

### Directories and file I/O

### JSON and Serialization
Cereal, Binary

JSON - Aeson

### Envirionment variables 


### Basic networking (HTTP calls)

Network.HTTP.Simple? Maybe too complex
HTTP
http-streams

### Tests
tasty, hedgehog

golden testing


### Publishing, seting up CI

### Extensions/ more advanced materials
streaming

parser combinators

foldr/foldl/foldl' folds (and recursion combinators)

Standard type classes beyond the Eq, Ord, Read, Show

- Data.Monoid
- Control.Monad
- Control.Applicative
- Foldable
- Traversable

### Build tools
shake




```

# Specific exercises/examples


* Find oldest file called *.out


* Camel case conversion


Examples culled from (Stephan):

* SDN
* Vault management
* Make files















