```mermaid
flowchart TB
    User[User]
    Guest[Guest]
    Admin[Admin]

    subgraph SYSTEM
        Login[Logowanie]
        Browse[Przegladanie]
        Register[Rejestracja]
        ManageAccount[Zarzadzanie kontem]
        ExportReports[Eksport raportow]
    end

    User --> Login
    User --> Browse

    Guest --> Browse
    Guest --> Register

    Admin --> Login
    Admin --> ManageAccount

    ManageAccount --> ExportReports
```mermaid
