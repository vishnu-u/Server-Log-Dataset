# Context
The dataset is a synthetically generated server log based on Apache Server Logging Format. Each line corresponds to each log entry. The log entry has the following parameters : 

# Components in Log Entry :
- <b>IP of client:</b> This refers to the IP address of the client that sent the request to the server.
- <b>Remote Log Name:</b> Remote name of the User performing the request. In the majority of the applications, this is confidential information and is hidden or not available.
- <b>User ID:</b> The ID of the user performing the request. In the majority of the applications, this is a piece of confidential information and is hidden or not available.
- <b>Date and Time in UTC format:</b> The date and time of the request are represented in UTC format as follows: - Day/Month/Year:Hour:Minutes: Seconds +Time-Zone-Correction.
- <b>Request Type:</b> The type of request (GET, POST, PUT, DELETE) that the server got. This depends on the operation that the request will do.
- <b>API:</b> The API of the website to which the request is related. Example: When a user accesses a carton shopping website, the API comes as /usr/cart.
- <b>Protocol and Version:</b> Protocol used for connecting with server and its version.
- <b>Status Code:</b> Status code that the server returned for the request. Eg: 404 is sent when a requested resource is not found. 200 is sent when the request was successfully served.
- <b>Byte:</b> The amount of data in bytes that was sent back to the client.
- <b>Referrer:</b> The websites/source from where the user was directed to the current website. If none it is represented by “-“.
- <b>UA String:</b> The user agent string contains details of the browser and the host device (like the name, version, device type etc.).
- <b>Response Time:</b> The response time the server took to serve the request. This is the difference between the timestamps when the request was received and when the request was served.

# Content
The dataset consists of two files - 
- <i>logfiles.log</i> is the actual log file in text format
- <i>TestFileGenerator.py</i> is the synthetic log file generator. The number of log entries required can be edited in the code.
