This is Spring architecture. The client calls the REST APIs, which interact with the controller. The controller interacts with the service, the service calls the repository, and the repository interacts with the database.

why is a dto object important ?

1. not to expose the internal representation of object,
2. if directly using the model to pass request, response, it is very difficult to change the model. 
    -backward compatibility issues.
