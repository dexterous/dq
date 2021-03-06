# dq

Check how developer friendly is your machine!

```
$ dq
✔ curl
✔ git
✔ java
✘ node
✔ perl
✔ python
✔ ruby
✔ vi

Your dq is 7 / 8
```

## Install

1. `wget -O ~/bin/dq https://raw.github.com/dexterous/dq/bash-only/dq`
1. `git clone git://github.com/dexterous/dq.git` and add `dq` to `PATH`

## Usage
 
There is more to it. Depending on what you develop, we have got some preselected profiles:

#### Minimal
To see if you have some common commands installed that a developer machine usually needs
`dq core`

#### ruby dev
`dq ruby_dev`

#### frontend dev
`dq frontend_dev`

#### java dev
`dq java_dev`

#### clojure dev
`dq clojure_dev`

#### groovy dev
`dq groovy_dev`

#### scala dev
`dq scala_dev`

#### db
`dq db`

#### all

**Feeling courageous**, see what all you have got :

`dq all`

This checks for about 40 commands on your box

#### Specific commands only

`dq --only lang`

This checks for all the commands in the `lang` group only.

`dq --only lang java`

This checks for all the `java` command in the `lang` group only.

The `--only` flag accepts glob params as well.

```
$ dq --only lang p*
✔ python
✔ perl

Your dq is 2 / 2
```

## Don't want to install

Run it straight off the interwebs!

`curl -sL https://raw.github.com/dexterous/dq/bash-only/dq | bash -s -- core`

## About

Ever got onto a new machine or a remote server? If you develop, you almost certainly need to check availability of your
tool-chain on command line. DQ is intended to relieve you from pain of checking each command individually.

It was named DQ as Developer Quotient (or Developer Friendliness Quotient of a machine), which may not be the most
apt name but that was the best name I could think of.

## Contributing

Please submit more command checks, it's very easy to do so. Fork the repo and send PR.
Issues and feedback welcomed.

## Paranoid?

Don't want to run `curl` piping to `sh`. Understandably, you might be concerned. Worry not.
- The source is hosted and is served directly from github, no app server in the middle.
- If you still want to check, do a  `curl -sL https://raw.github.com/kdabir/dq/master/bin/core/dq.sh | cat`  first.
    (basically, replacing `sh` with `cat`, to see the content of the file )
- Or, just `git clone` the repo and add the `dq` script to your `PATH`

### ♥
