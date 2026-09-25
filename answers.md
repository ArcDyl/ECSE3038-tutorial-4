POST /devices with the probe body           Status: 201     Deiices: 5
POST /devices with the probe body again     Status: 201     Devices: 6
PUT /devices/attic with the attic body      Status: 200     Devices: 6
PUT /devices/attic again                    Status: 200     Devices: 6
DELETE /devices/fridge                      Status: 200     Devices: 5
DELETE /devices/fridge again                Status: 404     Devices: 5
Two of the three methods left the system the same irregardless of whether the request was sent once or twice, these methods were 1. PUT & 2. DELETE. The property observed in these two methods is called idempotence.