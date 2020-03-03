## Replacing Git Remote URL

There was a problem of not being able to push to orgin master,
because repo address was wrong.

It's probably due to copying a wrong repo address.

Here is how to update the remote address for future reference.


Check current status of git remote & get the url of the remote.  
```
git remote
git remote get-url origin
```

Remove the remote origin and check if it is successfully removed.
```
git remote remove origin
git remote 
```


add origin with the right git address to the remote and check.
```
git remote add origin git@gist123456789.git
git remote
git remote get-url origin
 
```

See if git can be successfully be pushed.

```
git push origin master
```
