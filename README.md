#SED

##01
>Simple change and create new file
```
$ sed 's/nonconformism/<b>nonconformism<\/b>/' <01_old.html > 01_new.html
```

---

##02
>The slash as a delimiter(The character after the s is the delimiter) // -g
```
$ sed 's:nonconformism:<i>nonconformism<\/i>:g' <01_old.html > 02_new.html
```

---

##03
>Using & as the matched string. greedy
```
$ sed 's/[a-z]*/(&)/' <01_old.html > 03_new.html
$ sed 's/[a-z][a-z]*/(&)/' <01_old.html > 03_new.html
```

---

##04
>Extended Regular Expressions. Using Apple Mac OS X -E
```
$ sed -r 's/[a-z]+/(&)/' <01_old.html > 04_new.html
```

---

##05
>Using \1 to keep part of the pattern
```
$ echo abcd123 | sed -r 's@([a-z]*).*@\1@'
```

---

##06
>Using \1 to keep part of the pattern
```
$ echo abcd123 | sed -r 's@([a-z]*).*@\1@'
```

---

##07
>/1, /2, etc. Specifying which occurrence // 2 || after 2 >> -g2
```
$ sed 's:nonconformism:<i>nonconformism<\/i>:2' <01_old.html > 07_new.html
```
