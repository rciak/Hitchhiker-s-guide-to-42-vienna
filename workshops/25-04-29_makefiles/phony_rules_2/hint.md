# Phony rules 2

* Continue story:  
  * Now Dog Mulder had enough and implements the (PHONY) rules
    `clear_priated_copies` and
    `clear_pirated_copies_and_collection`.

* **tecnical Remark:** 
  *Mention at the end of the workshop:* That for simplicity and not to distract the audience from the main topic the likely familiar command `cp` was used. For interactive use on the terminal this is ok, but in scripts or makefiles one should rely not on it for copying tasks but rather, on `rsync`; if for instance the common `alias cp='cp -i'` is set in the shell from where you start make, unintended behavious is to occur ...