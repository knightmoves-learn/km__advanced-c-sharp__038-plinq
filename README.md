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
- Decompose problems into smaller components through systematic analysis, using constructs such as procedures, modules, and/or objects (3A-AP-17) https://www.csteachers.org/page/standards
- Create prototypes that use algorithms to solve computational problems by leveraging prior student knowledge and personal interests (3A-AP-13) https://www.csteachers.org/page/standards
- Create artifacts by using procedures within a program, combinations of data and procedures, or independent but interrelated programs (3A-AP-18) https://www.csteachers.org/page/standards
- Analyze a large-scale computational problem and identify generalizable patterns that can be applied to a solution (3B-AP-15) https://www.csteachers.org/page/standards
- Construct solutions to problems using student-created components, such as procedures, modules and/or objects (3B-AP-14) https://www.csteachers.org/page/standards


## Resources
- https://learn.microsoft.com/en-us/dotnet/standard/parallel-programming/introduction-to-plinq
- https://simple.wikipedia.org/wiki/Thread_(computer_science)
- https://simple.wikipedia.org/wiki/Parallel_computing

Copyright &copy; 2025 Knight Moves. All Rights Reserved.
