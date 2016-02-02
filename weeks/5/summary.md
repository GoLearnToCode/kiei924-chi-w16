
* Introduction to SQL
* What's Next


### Get a Cloud9 account

1. Go to http://c9.io
2. Create a free account by signing in with your GitHub credentials
3. You can ignore/dismiss the Welcome page
4. Find the big "Create Workspace" button and click it
5. Fill in two fields: the name should be "sql", and the "Clone from Git" field should be https://github.com/kiei924-chicago/learn-sql

### Using the Terminal

This is the window that has a prompt that says something like `(master) $` and is waiting for you to type a command.

Type this:

`sqlite3 hockey.sqlite3`

You are now in the Sqlite Shell.  To exit the shell at anytime and go back to the Terminal prompt:

`.exit`  or press `Ctrl-D`.

To see the list of tables and columns:

`.schema`

### SQL Commands

Here's a quick reference, but you should refer to the slides for complete examples.

* `SELECT`
* `FROM`
* `ORDER BY`
* `ORDER BY ... DESC`
* `LIMIT ...`
* `GROUP BY`
* `WHERE`
* `INNER JOIN ... ON ...`

REMEMBER: END ALL SQL COMMANDS WITH A COLON.  You can split your command over as many lines as you want - nothing will happen until you use a semicolon at the end.  If you seem to get "stuck", try just entering a colon.




