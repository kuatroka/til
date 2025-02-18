# til
Today I learned

## markdown
- Convert epub to markdown with pandoc in terminal

`pandoc -i /path/to/file.epub -o /path/to/output.md`

## Github / Git
- when failing to upload the initial git repo to github with error below, in terminal use `git config http.postBuffer 524288000`

```
error: RPC failed; HTTP 400 curl 22 The requested URL returned error: 400
 ..............
fatal: the remote end hung up unexpectedly
```
## Frontend / UI
- Sometimes when DOM thrashing happens, check if there are multiple tailwind libraries imported and used. I had both `preline` and `flowbite` imported and they created DOM thrashing when clicking on some buttons in the global menu


## Backend DB
- When using SQLite and `sqlite3-rsync` replication, the app would crash when visiting only certain routes. The most possible reason was the NULL values in the fields that were used in the table or search functionalities. When filling NULLs with blank strings, the crashing stopped. (further tests are needed) 
