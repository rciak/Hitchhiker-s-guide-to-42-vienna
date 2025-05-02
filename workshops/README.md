# Workshops

Here you can find Material related to peer workshops / demo sessions
that were already held. The following list is sorted by date (newest first)
and contains a link to a subsection.

* [25-04-29_makefiles][1]

## 25-04-29_makefiles

### Summary

*By:* René Ciak  
*For:* Beginners  
*Topics:* Basic notions, pattern rules, phony rules  
***Hint***: Consider the various hint.md files in every subfolder:
  They contain additional information about the Makefiles in that folder.

### Description

The workshops presents evolving `Makefile`s to introduce

* simple **rules**, **pattern rules** and **PHONY rules**,
* Meaning of `@` before a command,
* **Makefile variables** and their expansion via the `$( )` operator,
* **Autovariables** `^`, `<` and `@`,
* **Substitution** via `patsubst`

### Further reading

* [TUTO: Best practices and tricks for making a good makefile?](https://stackoverflowteams.com/c/42network/questions/1604)  
  This seems to be a good suplement to the `25-04-29_makefiles` workshop,
  touching additional interesting topics like dependencies.
  **As new 42 stundents you need to register to the 42 Network on 
  Stack Overflow for teams**: Click in the intra button on the speech bubbles...
* [Makefile tutorial](https://makefiletutorial.com)  
  I did not look closely at this one, seems to contain interesting topics,
  but maybe a bit too much for starting.
* [GNU make manual](https://www.gnu.org/software/make/manual/html_node/index.html)  
  This official documentation is very precise and seems good,
  but maybe not ideal for beginners.


* [Makefile cookbook](https://www.gnu.org/software/make/manual/html_node/Makefile-Cookbook.html)

### Ideas for further improvements of the workshop 25-04-29_makefiles:

When preparing to do the workshop another time here are some
(likely not yet fully thought thourgh) ideas that might be considered:

* Aks organizer if he can also look if there are questions (hands up) 
  in the audience that I did not note and decide if this is a question for 
  now or for the Q&A part. (Also for help to stay within 1h timeframe.)

* Give example in basic notions that illustrates the difference between `=` 
  and `:=` ?

* Introduce `$(@)` maybe earlier / along with `$(^)` and `$(<)` ?

* Items from or inspired by Thoughts and Feedback of Francesco:
  * Repeat the question
  * Start with introducing value of makefiles, related to questions like:
    * Makefiles can be annoying to write 
      "Why use them at all?"
        "What is is saving me from?"
        "What are the advantages?"

<--! Collection of links, suggestion: oldest first so that new entries are easy to add by just going to the bottom of this files.-->

[1]: https://github.com/rciak/Hitchhiker-s-guide-to-42-vienna/tree/main/workshops#25-04-29_makefiles
