```mermaid
sequenceDiagram
    participant browser
    participant server


    note left of browser: User types a note
    note left of browser: User saves the note
    browser-->>server: note
    activate server
    note right of server: Server adds note <br> to notes.json
    deactivate server
    note left of browser: browser adds note <br> to notes.json
    note left of browser: browser renders <br> notes element

```