#### Symbolic Links

---

symbolic links (also called soft links) is a file that points to another file for execution/refernce; think shortcuts in Windows or an alias on a Mac.

---
#### Creating symlinks
Creating symbolic links can be done in the command line (terminal). Use the `ln` command to create links.

* symbolic links (also called soft links) is a file that points to another file for execution/refernce; think shortcuts in Windows or an alias on a Mac.

To create a symbolic link in Unix, enter:
```
ln -s source_file myfile
```

* `source_file` : name of the existing file for which you want to create the symbolic link.

* `myfile` : name of the symbolic link.

* After creating the symbolic link, you can perform an operation on or execute `myfile`.


Example:
```
ln -sfn /new/target /path/to/symlink
```


[Source](https://kb.iu.edu/d/abbe)

---
