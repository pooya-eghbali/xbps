# xbps
A wrapper around void linux xbps tools.

# Installation

To install this, either do

```
xbps-install python3
git clone https://github.com/pooya-eghbali/xbps
cd xbps
chmod +x xbps
sudo ln -s $PWD/xbps /usr/local/bin/xbps
```

or any other way you prefer (idk, installing in sbin or /usr/bin, or downloading tarball instead of cloning, or renaming xbps to something else like void, pkg...)

# Features

1. Automatic sudo. 
2. Shortcuts
3. Python3 only.

# Usage

For `xbps-install` you have:

```
xbps install pkg  # same as xbps-install pkg
xbps in pkg       # same as above
xbps add pkg      # same as above
xbps + pkg        # same as above
xbps pkg          # same as above

xbps update       # same as xbps-install -Su
xbps up           # same as above
xbps ^            # same as above
```

for `xbps-remove` you have:

```
xbps remove pkg   # same as xbps-remove
xbps rm pkg       # same as above
xbps - pkg        # same as above

xbps remove+ pkg  # same as xbps-remove -R pkg
xbps rm+ pkg      # same as above
xbps -+ pkg       # same as above
```

for `xbps-query` you have:

```
xbps query pkg    # same as xbps query pkg
xbps info pkg     # same as above
xbps inf pkg      # same as above
xbps ! pkg        # same as above

xbps search pkg   # same as xbps-query -s pkg
xbps find pkg     # same as above
xbps ? pkg        # same as above

xbps list         # same as xbps-query -l
xbps ls           # same as xbps-query -l
xbps =            # same as xbps-query -l

xbps repositories # same as xbps-query -L
xbps reps         # same as above
```

for `xbps-reconfigure` you have:

```
xbps reconfigure pkg  # same as xbps-reconfigure pkg
xbps reconf pkg       # same as above
xbps ~ pkg            # same as above
```

for `xbps-alternatives` you have:

```
xbps alternatives pkg # same as xbps-alternatives pkg
xbps alt pkg          # same as above
xbps / pkg            # same as above
```

for `./xbps-src` you have:

```
xbps source pkg   # same as ./xbps-src pkg
xbps src pkg      # same as above
xbps * pkg        # same as above
```

for `xbps-pkgdb` you have:

```
xbps pkgdb pkg    # same as xbps-pkgdb pkg
xbps pkg pkg      # same as above
xbps db pkg       # same as above
xbps @ pkg        # same as above
```

for `xbps-rindex` you have:

```
xbps rindex       # same as xbps-rindex
xbps index        # same as above
xbps $            # same as above
```

if some of the one-char shortcuts don't make any sense, you can suggest replacement. for me some of them make sense, some of them don't, but i couldn't find any better ones.

# questions

1. why not bash? why python?

well, at first i wanted to do in bash, but thought maybe i'll add some features later that are impossible to do in bash

2. why python3?

Python 2 is dead.

3. why?

I don't like `xbps-command` method of doing things
