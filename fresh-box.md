What do they really mean?

---

Always assume you're on a fresh box

note:
can I
- clone your repo
- run
  - install
  - test
  - build
  - start

you wont have any databases, binaries, libraries


Bad
```sh
fresh-box@user ~ $ git clone git@github.com/user/not-working
cloning into not-working...

fresh-box@user ~ $ cd not-working

fresh-box@user ~/not-working $ npm install
installing all dependencies...

fresh-box@user ~/not-working $ npm test
08/29/2017 06:08:14 ERROR: Could not create connection over 3306
missing database
```


Good
```sh
fresh-box@user ~ $ git clone git@github.com/user/working
cloning into working...

fresh-box@user ~ $ cd working

fresh-box@user ~/working $ npm install
installing all dependencies...

fresh-box@user ~/working $ npm test
  PASS  src/reducers/api.spec.js
  PASS  src/App.test.js

  Test Suites: 5 passed, 5 total
  Tests:       14 passed, 14 total
  Time:        24.379s

```
