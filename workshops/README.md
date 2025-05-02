# Workshops

Here you can find Material related to peer workshops / demo sessions
that were already held. The following list is sorted by date (newest first).

* ***25-04-29_makefiles*** - Beginner's level  
  *Subtopics:* Basic notions, pattern rules, phony rules  
  *Description:* The workshops presents evolving `Makefile`s to introduce
  * simple **rules**, **pattern rules** and **PHONY rules**,
  * Meaning of `@` before a command,
  * **Makefile variables** and their expansion via the `$( )` operator,
  * **Autovariables** `^`, `<` and `@`,
  * **Substitution** via `patsubst`

# Ideas for further improvements of this workshops:

When preparing to do the workshop another time here are some
(likely not yet fully thought thourgh) ideas that might be considered:

* Aks organizer if he can also look if there are questions (hands up) 
  in the audience that I did not note and decide if this is a question for 
  now or for the Q&A part. (Also for help to stay within 1h timeframe.)

* Give example in basic notions that illustrates the difference between `=` 
  and `:=` ?

* Introduce `$(@)` maybe earlier / along with `$(^)` and `$(<)` ?

* Items from or inspired by Feedback of Francesco:
  * Start with introducing value of makefiles, related to questions like:
    * Makefiles can be annoying to write 
      "Why use them at all?"
        "What is is saving me from?"
        "What are the advantages?"