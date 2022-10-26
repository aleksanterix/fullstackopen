Browser -> Server: HTTP POST /exampleapp/new_note
Server --> Browser: Status 302
Browser -> Server: HTTP GET /exampleapp/notes 
Server --> Browser: Returns notes
Browser -> Server:  HTTP GET /exampleapp/main.css 
Server --> Browser: Returns main.css
Browser -> Server:  HTTP GET /exampleapp/main.js 
Server --> Browser: Returns main.js

Note over Browser:
Browser runs main.js
JS requests JSON
end note

Browser -> Server: HTTP GET /exampleapp/data.json  
Server --> Browser: Returns data.json

note over Browser:
Browser reads and 
renders data to page
end note 
