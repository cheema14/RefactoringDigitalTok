# RefactoringDigitalTok


# Thoughts
1. Inside BookingController - Instead of having an if/else check in the index method, it can be handled via a middleware. Purpose is to have less if/else statements.
2. No null checking/Validations - BookingController - id parameter in update method, no validation of request params in store and update method. 

BookingController - getHistory method - if statement can be handled via middleware. 
Overall validation is required for request parameters fetching being done in the controller.
I am not aware of the exact structure of the code, but instead of passing ids, the model which is needed to be updated can be passed so that we don't have to run a search query before updating/saving.


# Refactoring Points

distanceFeed method - I replaced longer if statements with shorthand if operators.