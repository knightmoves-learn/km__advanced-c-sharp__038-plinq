# 038 Plinq

## Lecture

[![# Plinq (Part 1)](https://img.youtube.com/vi/IYME73S-Zmo/0.jpg)](https://www.youtube.com/watch?v=IYME73S-Zmo)
[![# Plinq (Part 2)](https://img.youtube.com/vi/GzCzegdIxnQ/0.jpg)](https://www.youtube.com/watch?v=GzCzegdIxnQ)

## Instructions

- In `HomeEnergyApi/Services/ZipCodeLocationService.cs`
    - Modify the `Report()` method
      - Create a new variable named `stateFromFluentLinqParallel` to hold the state from the `response`, set the value of this variable by calling executing the following fluent LINQ methods on `response.Places`
        - WHERE the state is not null
        - Execute in Parallel
        - SELECT the `State` property
        - Return as a list
      - Immediately after, call `logger.LogInformation()` with the following argument `$"State from API: {stateFromFluentLinqParallel[0]}"`

## Additional Information

- Do not remove or modify anything in `HomeEnergyApi.Tests`
- Some Models may have changed for this lesson from the last, as always all code in the lesson repository is available to view
- Along with `using` statements being added, any packages needed for the assignment have been pre-installed for you, however in the future you may need to add these yourself

## Building toward CSTA Standards:

- Document design decisions using text, graphics, presentations, and/or demonstrations in the development of complex programs (3A-AP-23) https://www.csteachers.org/page/standards
- Systematically design and develop programs for broad audiences by incorporating feedback from users (3A-AP-19) https://www.csteachers.org/page/standards

## Resources

- https://swagger.io/
- https://github.com/dotnet/aspnet-api-versioning/wiki/API-Documentation

Copyright &copy; 2025 Knight Moves. All Rights Reserved.
