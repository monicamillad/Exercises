
# Troubleshooting exercise - V1 - 13/06/2021

This is a specification for a programming exercise to develop a Troubleshooting web app for technicians. The final result should be a web application that provide some features to help technicians in troubleshooting and fixing problems.

The exercise is divided into N phases to ease the implementation by allowing for incremental development. However, it is <b>imperative</b> that the design and the implementation of each is done with the next phases taken into consideration.

> Please note that the usage of any library (third-party or built-in) requires an explicit permission from your supervisor, i.e. the supervisor has the right to prevent the usage of some library/class even if it is a built-in library in Java.

## Phase 01: Initial user interface - 3 days

In this phase, it is required to create the very first pages in the app; which are:
- Register and login pages
- Home page that contains a nav bar at the top that contains one tab `Reboot Requests` and an icon that show dropdown list when on clicking, the dropdown list has account settings and logout button.
- account settings page that contains a form to edit user (technician) data.

> In this phase there will be no integration with backend so you can use dummy data or dummy APIs' calls

> <b>Preparation for next phase:</b>
> - [Functional Interfaces in Java 8](https://www.baeldung.com/java-8-functional-interfaces)
> - [Parallel and Asynchronous Programming with Streams and CompletableFuture](https://www.youtube.com/watch?v=0hQvWIdwnw4&t=10140s)

## Phase 02: Queueing System implementation (1) - 10 days

In this phase it is required to develop the Reboot devices queue system.
### Implementation requirements
- Create function that takes a Consumer as input [let's call it here `applyTask`].
- These functions should be applied on multiple threads with queue management System.

## Phase 03: Queueing System implementation (2) - 10 days


In this phase, the client can get notification on finished tasks if subscribed, and there will be another version from applyTask function.

### Implementation requirements

-   Notification on finished tasks should be done in two ways:
    -   Using Observables.
    -   Using Streams.
-   Create another version of applyTask that returns CompletableFuture.
-   Ability to change the number of threads.

## Phase 04: Use our Queueing System in managing reboot devices - 5 days

## Phase 04: Enhance login and Register functionalities - 10 days



### Notes
- -   It is prefered to apply the concept of the  **Fluent interface**  in the Queueing System part.
