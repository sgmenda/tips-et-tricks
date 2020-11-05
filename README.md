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
