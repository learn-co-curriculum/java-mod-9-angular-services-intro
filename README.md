# Services Introduction

## Learning Goals

- Explain Angular services purpose.

## Introduction

Our current application has the basic layout, component structure and models we
want. We also started reacting to user input with the "message preview"
functionality we added earlier. Next, we should add the ability to react to a
user sending a new message and updating our application data accordingly.

To do this, we need our components to talk to each other. Going back to our
application hierarchy, you can see that the component that holds the user's
message is the "Send Message" component, which in our case is a  
"Level 3" component, while the component that currently holds the list of
messages for a given conversation is the "Conversation Thread" component, which
in our case is also a "Level 3" component, i.e. a peer to the send message
component in the hierarchy.

Here is our component hierarchy to refresh your memory:

![Messaging Application Component Hierarchy](https://curriculum-content.s3.amazonaws.com/java-mod-8/ng-messaging-component-hierarchy.png)

In order to have various components across an application talk to each other, we
will use a new type of class, which is a service. Services can be accessible
from different components, and therefore can be used to a) share functionality
and b) share data.

We will be looking at different services in the following lessons.
