# ShindigManager
Shindig Manager will be a suite of products for the management of events, emphasizing community technology events such as Code PaLOUsa.  There will also be provisions in the suite to allow speakers to manage their speaking portfolio and engagements.

While providing essential services for speakers and events, Chad Green uses Shindig Manager to demonstrate different technologies and practices.

### Shindig Manager Components
While subject to change, here are the products that are the goal of this project:
Shindig Site: The landing site for events using Shindig Manager.
Series Site: The landing page for a series of events to include annual editions.  This will help attendees, speakers, and sponsors to see content from past events.

* **Organizer Portal:** The administration portal for the event organizers to manage Shindig Manager and all of its components.
* **Speaker Portal:** The portal used for an event’s speakers to manage their content and participation.
* **Sponsor Portal:** The portal used for an event’s sponsors to manage their participation in the event.
* **Attendee Portal:** The portal used for an event’s attendees to manage their attendance.
* **Speaker Profile:** The place for speakers to manage their portfolio and speaking engagements.
* **External API:** API endpoints to allow access to the data of the products mentioned above.

### Shindig Architecture
Because Shindig Manager is used for demonstration purposes, it can store its data in either an Azure SQL database or a Cosmos DB Core database.  There might also be work done to keep data in a Cosmos DB Graph (Gremlin) database.  To accomplish this, Shindig Manager will use the Unit of Work and Repository patterns.

Also, a key to Shindig Manager is interacting with the products via an externally available REST API service.  This will allow users to use the backend services to run their sites.

Here is the target architecture:

![Conceptual Architecture](docs/Shindig%20Manager%20Conceptual%20Architecture.drawio.png)