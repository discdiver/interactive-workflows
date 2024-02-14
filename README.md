# Active workflows

The goal is to get more comfortable creating active workflows.

## Instructions

Fork and make PRs to this repo.

Use the folder for your group/room number.

Use whatever Prefect Cloud workspace your group wants.


### Challenge 1

Finance wants to approve any manually approve any ml model training runs that will cost over $1k.

Make a flow that gets an estimated cost from one of the tasks it calls and pauses for approval. 
If the request is approved, a task to train the model is called model training  (dummy stub for this exercise). 
You can make the code look however you like. 
For the first challenge, just take a string input and see if it matches "Approve".

This can be a "dumb" example that doesn't cover any edge cases.


### Challenge 2

Extend/modify your code from Challenge 1. 
Make a new code file. 
Make the default string value "Approve".

### Challenge 3

Extend/modify your code from Challenge 2. 
Make a new code file. 
Make the approver's options either "Approve" or "Disapprove".

### Challenge 4

Extend/modify your code from previous challenges. 
Make a new code file. 
Make the approver's options either "Approve" or "Disapprove".
If the request is approved 
