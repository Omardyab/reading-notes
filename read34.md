# Reading 13
Status Codes based on REST Methodes
100’s = These error code are typically to notify the client that requests are OK and that it should continue if it has not finished
200’s = These code are seen when requests meet validation at the time of sending, doesn't necessarily mean the request was successful
300’s = 300 codes usually mean that a request for resource is no longer available, or that the request needs to be redirect to the correct resource
400’s = This is the most common client side error code. It can range form things like wrong URL, to an invalid request, timeouts, or missing authentication.
500’s = When these codes are present, it's a signafier that the server encountered a problem, like over trafficed or unreachable servers. It could be related to the client request, which caused an error exception. It's typically useful for the client to try the same request again.
What is a status code 202? = An HTTP status code indicating that the request has been accpted or processing. At this point processing may not be complete, or have even started
What is a status code 308? - The 308 status code is present when the requested resource has been permenantly changed toa nother URL.
What code would you use if an update didn’t return data to a client? - status code 204
What code would you use if a resource used to exist but no longer does? - status code 410 Gone
What is the ‘Forbidden’ status code? - The client has authorized or does not need to authrize itself, but does not have permission to access the resources