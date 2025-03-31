
flowchart TD
    %% Global Entities
    User["User"]:::user

    %% Docker & Compose Orchestration
    Docker["Docker & Compose Orchestration"]:::docker

    %% Main Services
    Rails["Rails Meme Search Application"]:::rails
    Python["Image-to-Text Generator (Python)"]:::python
    DB["PostgreSQL Database (with pgvector)"]:::database

    %% Shared File Volumes Subgraph
    subgraph "Shared Meme Files"
        PublicMemes["Public Memes"]:::volume
        MemeDir["Meme Directory"]:::volume
    end

    %% Interactions
    User -->|"interaction"| Rails
    Rails -->|"DBQueryUpdate"| DB
    Rails -->|"APIRequest"| Python
    Python -->|"APIResponse"| Rails

    %% Volume Access
    Rails ---|"VolumeMountAccess"| PublicMemes
    Python ---|"VolumeMountAccess"| MemeDir

    %% Docker Orchestration Links
    Docker ---|"orchestrates"| Rails
    Docker ---|"orchestrates"| Python
    Docker ---|"orchestrates"| DB

    %% Click Events
    click Rails "https://github.com/neonwatty/meme-search/tree/main/meme_search_pro/meme_search_app"
    click Python "https://github.com/neonwatty/meme-search/tree/main/meme_search_pro/image_to_text_generator"
    click DB "https://github.com/neonwatty/meme-search/blob/main/meme_search_pro/meme_search_app/config/database.yml"
    click Docker "https://github.com/neonwatty/meme-search/blob/main/docker-compose.yml"
    click PublicMemes "https://github.com/neonwatty/meme-search/tree/main/meme_search_pro/meme_search_app/public/memes"
    click MemeDir "https://github.com/neonwatty/meme-search/tree/main/meme_search_pro/memes"

    %% Styles
    classDef user fill:#fceabb,stroke:#d79b00,stroke-width:2px;
    classDef rails fill:#c8e6c9,stroke:#388e3c,stroke-width:2px;
    classDef python fill:#bbdefb,stroke:#1976d2,stroke-width:2px;
    classDef database fill:#ffe082,stroke:#f9a825,stroke-width:2px,stroke-dasharray: 5 5;
    classDef docker fill:#d1c4e9,stroke:#673ab7,stroke-width:2px,stroke-dasharray: 3 3;
    classDef volume fill:#ffcdd2,stroke:#e53935,stroke-width:2px,stroke-dasharray: 2 2;
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTU1NjMzNDI1LDgzNTM4MDk2OSwxNTgwMz
A5Njk3LDIxMjE2NzcxMjFdfQ==
-->