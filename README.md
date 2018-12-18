# queue-framework
A re-useable open source version of an Queue Framework to be used as a code library referenced from other projects.
[![Build Status](https://dev.azure.com/pelleolsson/queue-framework/_apis/build/status/pelleo.queue-framework?branchName=master)](https://dev.azure.com/pelleolsson/queue-framework/_build/latest?definitionId=1?branchName=master)

## Requirements

    The requirements of the Queue Framework are organized into different versions, where each version 
    builds on the previous one
    
### Generic requirements

    Library should be easy to use, compile and contribute to
    Easy to reference and use from other projects
    Library should conform to Design Guidelines, Conventions, Idioms, and Patterns normally used in the eco system

## Version 1.0 - The Basics

Provide a basic re-usable "code library" that provides the following capabilities:

    A Priority Queue
        Where you can add objects of type T together with a priority
        An ability to pull from the queue where the most prioritized objects are taken first

### Version 1.1 - The Basics, Update 1

Introduce additional features:

    A Delayed Queue
        Works like a normal queue, but nothing pushed to the queue will be vissible until N seconds has passed
    A Faulty Queue
        Works like a normal queue, but sometimes (should be configurable how often) drops messages pushed to the queue

## Version 2.0 - Complexity

Introduce additional features:

    Persistant Queue
        Works like a normal queue, but will live through process restarts

### Version 2.1 - Complexity, Update 1

Introduce additional abilities to the Persistant Queue:

    Load Queue From File - Loads the content of the queue from a named file
    Reset Queue - Clears the queue

### Version 2.2 - Complexity, Update 2

Add ability to Load Queue From Stream if not already available

    For ideas and general discussions on queues vs. stream, please refer to 
    https://streaml.io/blog/unified-queuing-streaming

## Version 3.0 - Additional Features

Reliable Queue

    Implement a queue object that can span across several processes and servers
