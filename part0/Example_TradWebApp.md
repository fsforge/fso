sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/
    activate server
    server-->>browser: HTML document
    deactivate server
	
	Note right of server: The number of notes is calculated on the server backend!

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/kuva.png
    activate server
    server-->>browser: the png file
    deactivate server