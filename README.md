# TruffleTracker

An opinionated project management system.

# Stack

* node
* mongoDB
* SASS
* React

# Features

* products
* versions
* backlog
* sprints
* time
* developers
* goals
* user stories
* tasks
* dependencies
* issues
* time management
* cost management

# Why TruffleTracker?

TruffleTracker is being built as a side-project to improve my skills in a number of disciplines, but also to resolve many headaches that I have experienced when developing software using other project management tools. 

The ethos of TruffleTracker is that it will tie heavily into a semantically versioned, agile project development cycle. 

# What is a product?

A product is the core entity within TruffleTracker. Issues, stories, time and cost are all elements that exist within a product. When you first create an account within TruffleTracker you will be asked to create your first product. As an account holder you may have many products. 

A product has a given end date (but this is not a requirement, some products don't have an end date) and a cost. Projection and reporting of cost and time can be executed at the product level against these two values.

# What is a version?

A version can be a major, minor or patch of a given product. Issues and stories are assigned to a version, and a version has a goal for completion date and cost. Tracking of cost and time can be done against a version, independantly of a product as a whole.

# What is a backlog?

Each product has a backlog of issues and stories. They exist in the backlog as they are work items that currently have no delivery expectation. An issue or story is moved from the backlog to a version to indicate that it will be included in the release of that version. 

# What is a sprint?

A sprint is a period of time that is customised on a per product basis. A sprint defaults to 5 working days. It is the period of time that a portion of a version of a product is completed in. A version must have at least 1 sprint, and may have an infinite amount of them (though this would indicate a creeping scope to the version). 

Issues or stories are assigned to a sprint, and tracking can then be performed on the progress of the sprint, if it is likely to be completed and how much a sprint cost compared to time assigned.

# What is a time?

A time has three types, actioned, estimated, size. 

## What is size time?

Size time is a rough guide to the size of an issue or story. It indicates in very fluid terms what level of work is expected for any given item. Size is measured in a configurable way, the default is tall, grande and venti (this is because I like Starbucks coffee). 

Size is applied to an item by a senior developer or project lead who has a core understanding of existing code and what would be involved to complete the item. This lack of mental involvement in the precise nature of what has to happen allows quick estimates to be applied, and complete or large areas of work identified and broken down. This can be achieved efficently and provide quick cost and time projections to a sprint.

## What is estimated time?

Estimated time is a hour based estimate that a develop working on a issue or story gives to it when they have a fully developed notion of precisely what is involved in the completion of the item. It is more accurate than a size as it indicates a review of code/systems and defines the developers understanding of the work involved at the beginning of execution.

## What is actioned time?

Actioned time is the number of minutes/hours/days that a developer has spent on an issue or story. It is the real time that it has taken to complete or execute a portion of a issue or story.

# What is a developer?

A developer is quite obviously a person that executes issues or stories within a sprint. They can be a back end engineer, system arcitect, deisnger, frond end developer, or even a linguist. They assign themselves to issues or stories and complete them.

# What is a goal?

A goal is some ability that is achieved by the product. This can vary from the very simple - I can see a title of my news article - to the very complete - I can see aggregated reporting data for the past decade, with splitting for financial quarters cross referenced by department.

Goals are attached to stories and represent a value of completion. A view should be available for a product to see the goals and what user stories and issues are involved in completing them.

Goals will likely start as very broad ideas, and be broken down time and again until they have more narrow focus. This allows a non-technical user to understand what is possible within product, and what aspects of the product are being worked on and how far away they are from completion.

# What is a user story?

A user story is an item of new functionality that is going to be implemented. It has a size (see time) and it may then have tasks. 

A user story should have a description of Why? and What? before reaching the developer(s) responsible for executing the story. Why and What are created with the story by a product owner who understands the needs of the client and product direction. They describe in brief terms the rationale for the goals of the user story.

When a developer(s) decides to execute a story it should be assigned to a sprint. When the sprint begins the details of How? that story should be developed are applied to the story. Discussion should happen between the developer(s) and product owner to assign or adjust the goals the story belongs to so that they are manageable within the sprint and split off any unachievable parts into separate stories.

A user story should achieve at least one goal.

# What is a task?

A task is some small aspect of a user story. It represents a more simple unit of work, perhaps it represents some small change to an API to support further client side development. 

Tasks should be used when more than one developer is executing a user story so that dependencies can be created and followed. By using tasks to distribute development accross more than one developer stories should be more easily managed.

# What is an dependency?

Large products are complicated, even small versions of a product may require a lot of work to be completed. A dependency identifies links between user stories, tasks or issues. It indicates that something can't be started until something else has finished.

Dependencies will show on items when they have been established and time / cost estimation for items will be displayed with dependency values included as a separate figure. This will allow management of projets to see the real involvement required to complete some particular thing.

# What is an issue?

When user stories and tasks are completed and deployed to staging or UAT environments, issues may arise from testing. An issue represents some behaviour that is not intended. This is different from non-acceptence by a client of how something works (this is addressed by re-assessing the goals and the user stories to complete them), instead it is something that is not right according to the user stories intended outcomes.

An issue has a severity, the severity indicates how far away from the intended functionality the issue is. An issue has a priority, this indicates how important it is to fix. Severity and priority represent two distinct areas of assessment. Severity is effect, where as priority is for value. For example, a low severity bug might be very important to fix as it impacts a client workflow. However, a high severity issue may wait for 1/2 sprints because it doesn't effect anything a client will see for a while.

By correctly applying severity and priority it is possible to identify and schedule for completion issues with a product.

# What is time management?

Time management is an area of reporting within TruffleTracker. It indicates how close a product. version, goal, user story, task or issue is to completion and when it is estimated to be completed based on assignment to sprint, version and actioned time applied compared to estimated.

# What is cost management?

Cost management is an area of reporting within TruffleTracker. It indicates how expensive a product, version, goal, user story, task or issue is going to be, or has been. It uses time multiple by cost of development and maps that against budgets. 

## What is a budget?

A budget is a monetary figure that can be applied to a product, version, goal, user story or issue to indicate how much a business may wish to spend developing that aspect. 

This can be used to flag when budgets dont match predicted work loads. 
