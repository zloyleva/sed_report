#SED

##01
>Simple change and create new file
```
$ sed 's/nonconformism/<b>nonconformism<\/b>/' <01_old.html > 01_new.html
```

---

##02
>The slash as a delimiter(The character after the s is the delimiter)
```
$ sed 's:nonconformism:<i>nonconformism<\/i>:' <01_old.html > 02_new.html
```

---

##03
>Using & as the matched string. greedy
```
$ sed 's/[a-z]*/(&)/' <01_old.html > 03_new.html
$ sed 's/[a-z][a-z]*/(&)/' <01_old.html > 03_new.html
```

---
