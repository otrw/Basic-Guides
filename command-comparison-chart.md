# Command Comparison: info, Vim, and less

| Action                    | info              | Vim (Command Mode) | less              |
|---------------------------|-------------------|---------------------|-------------------|
| Move down one line        | ], Enter          | j                   | j, Enter, Down    |
| Move up one line          | [                 | k                   | k, y, Up          |
| Next page                 | Space, Page Down  | Ctrl+f              | Space, Page Down  |
| Previous page             | Backspace, Del    | Ctrl+b              | b, Page Up        |
| Go to top                 | t                 | gg                  | g, <               |
| Go to bottom              | e                 | G                   | G, >               |
| Search forward            | s, /              | /                   | /                 |
| Search backward           | ?                 | ?                   | ?                 |
| Next search result        | }                 | n                   | n                 |
| Previous search result    | {                 | N                   | N                 |
| Quit                      | q                 | :q                  | q                 |
| Help                      | h                 | :help               | h                 |
| Go to specific line       | g                 | :[number]           | :[number]         |
| Follow link/tag           | Enter             | Ctrl+]              | N/A               |
| Return from link          | l                 | Ctrl+t              | N/A               |
| Next node/file            | n                 | :next               | :n                |
| Previous node/file        | p                 | :prev               | :p                |
| Open menu                 | m                 | N/A                 | N/A               |
| Up in hierarchy           | u                 | N/A                 | N/A               |
|                           |                   |                     |                   |

Note: Chart covers common default behaviors, some commands will vary depending on configuration settings and version.