# MyNotes

Very simple notes manager from bash terminal.

## First step:
Add this lines to your .basrc directory
```
# For MyNotes
export PATH=<path_to_mynotes>/mynotes/bin:$PATH
```

## Usage
MyNotes contains 4 scripts:
- mynotes-create: Will create a new note. Use:

  * -t to specify the task
  * -d to specify a limit day
  * -p for priority
  * -g to specify the group of task it belongs
  
  Example: 
  ```
  mynotes-create -t "Do this super importat thing" -d "Now" -p "Super high" -g "Work"
  ```
- mynotes-list: Will list all your current notes.
- mynotes-edit: Edit a note. It will be opened with vim editor. If you would like another one you can edit this script 
to use your preferred editor.
- mynotes-delete: Delete a note(s). To use it:
```
mynotes-delete 1234089 3049813 130498
```
will delete notes with those IDs. The ID of each note can be found by mynotes-list.
