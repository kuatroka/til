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

