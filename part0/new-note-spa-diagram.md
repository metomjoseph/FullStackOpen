```mermaid
sequenceDiagram
    participant browser
    participant server

    browser ->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server -->> browser: JSON Data
    deactivate server

    Note right of browser: Callback function is executed by browser to render notes
```