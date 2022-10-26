Browser -> Server: HTTP GET /exampleapp/spa
Server --> Browser: Returns markup for site

Note over Browser:
Browser requests additional files according to markup
end note

Browser -> Server:  HTTP GET /exampleapp/main.css 
Server --> Browser: Returns main.css
Browser -> Server: HTTP GET /exampleapp/spa.js 
Server --> Browser: Returns spa.js

Note over Browser:
Browser runs spa.js
JS requests JSON
end note

Browser -> Server: HTTP GET /exampleapp/data.json  
Server --> Browser: Returns data.json

note over Browser:
Browser reads and 
renders data to page
end note 
