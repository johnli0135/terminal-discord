### Commands that always work

`servers`: List servers

`server s c`: View a channel in a server where channel name contains `c` and server name contains `s`. If not specified, `c` is the empty string

`tab-server s c`: Like `server`, but open the channel in a new tab

`direct-message s`: Open DMs between you and a user whose name contains `s`

`tab-message s`: Like `direct-message`, but open the channel in a new tab

`save`: Save the current open tabs to `saved_tabs.json`, overwriting any previous save

`pwd`: Print your current location (usually `/<server>/<channel>`)

`quit`: Quit

`help`: Display this text

### Commands that only work while already in at least one channel

`channels`: List all other channels in the current server

`channel c`: View a channel in the current server where channel name contains `c`

`tab-channel c`: Like `channel`, but open the channel in a new tab

`image path`: Attach an image

`refresh`: Refetch latest messages

`delete k n`: Delete your `k`th most recent message. Search through `n` messages to find the one to delete (if not specified, `n` = 10)

`edit`: Enter "edit mode." In this mode, the message being edited is highlighted and its contents are copied into the input buffer for editing. Hotkeys are rebound to move between past messages and finalize edits

`at s ...`: Send a message mentioning a user whose name contains `s` with content `...`. For example, `/at user hello` might send `@user, hello`

`close n`: Close the `n`th tab

`n`: View the `n`th tab

### Command aliases

Every command has a 1-2 letter alias:

`ss` → `servers`

`s` → `server`

`t` → `tab-server`

`dm` → `direct-message`

`tm` → `tab-message`

`sv` → `save`

`p` → `pwd`

`q` → `quit`

`h` → `help`

`cs` → `channels`

`c` → `channel`

`tc` → `tab-channel`

`i` → `image`

`r` → `refresh`

`d` → `delete`

`e` → `edit`

`a` → `at`

`x` → `close`

### Hotkeys

| Key(s)                         | Description                                     |
| ------------------------------ | ----------------------------------------------- |
| Control+c or Control+d         | Quit                                            |
| Up/Down                        | View next/previous in input history             |
| Home/End                       | Jump to beginning/end of current line of buffer |
| Left/Right                     | Move left/right in input buffer                 |
| Alt+h/j/k/l                    | Move left/down/up/right in input buffer         |
| Control+e/y                    | Scroll down/up                                  |
| Control+f/b or PageDown/PageUp | Scroll down/up by pageful                       |
| Control+g                      | Scroll to latest messages                       |
| Escape                         | Clear input buffer                              |
| Enter                          | Send message or command                         |
| Alt+semicolon                  | Send newline (for multiline messages)           |
| Alt+`([0-9])`                  | View tab `\1`                                   |

### Hotkeys that are different in edit mode

| Key(s)      | Description                             |
| ----------- | --------------------------------------- |
| Control+f/b | Switch to editing next/previous message |
| Escape      | Cancel edit                             |
| Enter       | Finalize edit                           |
