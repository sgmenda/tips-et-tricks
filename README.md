# tips-et-tricks

## git

### Locally Ignoring Files

To ignore locally
```
git update-index --assume-unchanged [filename]
```

To un-ignore locally
```
git update-index --no-assume-unchanged [filename]
```

### Sending Patches via Email

[email + git = <3](https://git-send-email.io)

## latex

### Document IDs

Inspired by [D. J. Bernstein](https://cr.yp.to/bib/documentid.html), I have started adding document IDs to some of my documents. I generate it as follows.

```
head /dev/urandom | sha256sum.exe | head -c32
```

### Latex to Markdown (and vice versa)

```
pandoc -f latex -t markdown xyz.tex > xyz.md
pandoc -f markdown -t latex xyz.md > xyz.tex
```

## Code Indexing

[SourceTrail](https://github.com/CoatiSoftware/Sourcetrail)

## Tor Browser

### Where to find nightly builds

```
http://f4amtbsowhix7rrf.onion/tor-browser-builds/
```

(`tor-guest` is the username and password.)

## Zips

### Adding/Updating a Zip

```
jar -uf A.zip B
```

## Firefox

### Bugzilla query for sec-high and sec-critical bugs

I got this handy query link from page 11 of [this report](https://github.com/iSECPartners/publications/tree/master/reports/Tor%20Browser%20Bundle).

https://bugzilla.mozilla.org/buglist.cgi?j_top=OR&f1=keywords&o1=anywordssubstr&resolution=---&resolution=FIXED&classification=Client%20Software&classification=Components&o2=anywordssubstr&query_format=advanced&f2=status_whiteboard&v1=sec-high%20sec-critical&v2=sg%3Ahigh%20sg%3Acritical&list_id=10101000

