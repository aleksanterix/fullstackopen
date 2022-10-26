Browser -> Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes     Retrieves markup for site
Server --> Browser: sends HTML-code    Sends markup for site
Browser -> Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes/main.css Retrieves styling info for site
Server --> Browser: Sends styling info / .css file
Browser -> Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes/main.js    Retrieves JS for site

Note over Browser:
Browser runs javascript
which requests JSON file
which has the notes
end note

Browser -> Server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes/data.json Retrieves notes / data.json
Server --> Browser: {"content": "What's going on here then?", "date": "2022-10-26T08:12:17.517Z"}

note over Browser:
Browser reads and renders the data to page
end note 