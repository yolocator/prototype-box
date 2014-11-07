# YoLocator API
Documentation for consuming YoLocator API. Created by Ritchie Marihugh for the YoLocator service.

The YoLocator service will allow a user to use Yo to store a location (e.g. parking spots, meeting location) instantaneously and retrieve it at a later time. There is a limit of one stored location per username.

# Parking [/parking?username={username}&location={location}]
This resource represents parking location for a username.

## Retrieve/Store Parking Spot [GET]
When location is supplied the location will be stored for the username. When it location isn't supplied and an existing location exists for the username it will be sent back with the yo.

+ Parameters
    + username (required) ... Sender's username
    + location (optional) ... Parking location
    
+ Response 200 (text/plain)