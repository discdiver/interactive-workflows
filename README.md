# Interactive workflows

## Background

You are software developers at We Train Models.
Finance wants more control of model training expenses in this cash-constrained time. 

You are users of the most popular orchestration product company in the world, naturally.
You've heard about active workflows, can you use them to help make the finance team happy?

## Instructions

- Fork and make PRs to this repo.
- Use a folder for your group/room number.
- Use whichever Prefect Cloud workspace your group wants.

## Part 1: HITL

### Challenge 1

Finance wants to manually approve any ml model training runs that will cost over $1k.

Make a flow that gets an estimated cost from one of the tasks (can be a hard coded value for this project) it calls and pauses for approval. 
If the request is approved, a task to train the model is called model training  (dummy stub for this exercise).  
For the first challenge, just take a string input and see if it matches "Approve".

This should be a "dumb" example that doesn't cover any edge cases.

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
If the request is approved the approver needs to then enter a 7 digit authorization code with no zeroes. 
Why? Don't ask. Zeroes look too much like the letter O for these folks, one was burned in a password incident years ago, idk. 

Validate that the authorization code meets the criteria in the UI - not in later Python code.


## Part 2: Send and receive input

Let's get more familiar with Prefect flows that can work together to send and receive input.

This [repo](https://github.com/PrefectHQ/interactive_workflow_examples) contains two interactive workflows that rely on `send` and `receive` input:
`llm_chatbot.py` and `sending_receiving.py`. 

Note, these features are a little rougher around the edges than the features you used above.

### Challenge 1
Try out `sending_receiving.py`.

### Challenge 2
Try out `llm_chatbot.py`.

### Challenge 3
Implement a proof of concept email drip campaign with an interactive workflow.

Here's the business process:

Send an email to a user.

If the user responds within two minutes (we'll pretend that's simulating two days), then they don't get the second email.

If the user doesn't respond within two minutes, then they will be sent the secon email.

Use two flows that interact. 

You don't need to create the actual emails, you can just mock them with basic functions for now.

### Challenge 4: Bonus

Take your work from challenge 3 and actually implement the sending and receiving of emails.

### Challenge 5: Super bonus

Scale your work from challenge 5 to work with multiple email recipients. 






