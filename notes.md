[client] -send a request -> [server] - send a response -> [client]

[client] -send a request -> [DNS server] -> [CDN] -> [server] - send a response -> [client]

| Not RESTful             | RESTful                                                     |
| ----------------------- | ----------------------------------------------------------- |
| `/createHubs`           | POST `/hubs`                                                |
| `/listHubMessages/:id`  | GET `/hubs/:id/messages`                                    |
| `/countHubMessages/:id` | GET `/hubs/:id/messages` add a `count` prop to the response |

Separation of Concerns
