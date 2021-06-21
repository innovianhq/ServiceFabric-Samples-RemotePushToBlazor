# Service Fabric Sample - Pushing data into Blazor via Service Remoting
This is a sample implementation that demonstrates a server-side Blazor website running in a Stateless Reliable Service Fabric service receiving data via [Service Remoting](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-reliable-services-communication-remoting) and pushing it out to a page.

## Why?
Typically, websites will utilize a timer to regularly poll the server for content updates. This puts a consistent (albeit potentially staggered) load on the server to identify changes since the last check. This example demonstrates how the server can instead push changes out to the relevant circuits only when it is notified by other services that something has changed eliminating the need for state change polling.

### Contributing
Pull requests are welcome!

### License
This sample is [MIT licensed](./LICENSE).
