---
layout: tour
title: "If"
description: "Scala language tour"
pageNumber: 20
isLast: false
group: tour
nextPage: interactive_tour_of_scala_match_as_a_switch.html
prevPage: interactive_tour_of_scala_loops_without_loops.html
links:

code:
  |
  if (true)   
    println("no braces on a single expression")  
  
  if (1 + 1 == 2) {  
    println("multiple")  
    println("statements")  
    println("require")  
    println("braces")  
  } else {  
    println("new math is found!")  
    println("or your CPU went crazy")  
  }  
  
  val likeEggs = false  
  val breakfast =  
    if (likeEggs) "scrambled eggs"  
    else "Apple"  
  
  println(breakfast)  
---

Conditions are almost the same as in imperative languages such as Java or C. However one important thing to remember in Scala, is that everything is an expression, even an `if` block. 

The ternary operator (`condition ? truePart : falsePart`) in Scala is simply `if (condition) truePart else falsePart`