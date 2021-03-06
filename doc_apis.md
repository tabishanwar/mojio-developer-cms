# APIs Overview #

Mojio provides two types of APIs for your application. A REST API and a PUSH API.

The REST API is good for request-response type problems. For example, you would use this if you are interested in the current status of a Vehicle. If, however, you are looking for an event on the Vehicle, constantly polling for changes on the Vehicle record is inefficient. The PUSH API is better suited for this.

The PUSH API follows the Observer model where you register the event or condition you are interested in (e.g. excessive speed or change in vehicle ignition status) and the Mojio Platform will notify your application with a push notification when this condition is met.

The PUSH API supports the following transports for receiving push notifications

- Apple Push Notification (APN for iOS)
- Google Cloud Messaging (GCM for Andorid)
- WebSockets
- HTTP POST 