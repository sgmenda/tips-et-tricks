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

## latex

### Document IDs

Inspired by [D. J. Bernstein](https://cr.yp.to/bib/documentid.html), I have started adding document IDs to some of my documents. I generate it as follows.

```
head /dev/urandom | sha256sum.exe | head -c32
```
