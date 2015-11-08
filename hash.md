# Hash
### Base64
Base64 is a group of similar binary-to-text encoding schemes that represent binary data in an ASCII string format by translating it into a radix-64 (6 bits) representation (1 char representation 1 byte). 

Example, how many chars of base64 to represent 6 Billion urls?
$$
\lceil\log_{64}{6e9}\rceil = \lceil5.4\rceil = 6
$$

```python
import base64
encoded = base64.b64encode('data to be encoded')
print encoded  # >>> ZGF0YSB0byBiZSBlbmNvZGVk
data = base64.b64decode(encoded)
print data  # >>> data to be encoded
```

### Hashing
Shortening an url:
```
hashed_url = base64(md5(url+salf))[:6]
```

Constructors for hash algorithms that are always present in this module are md5(), sha1(), sha224(), sha256(), sha384(), and sha512().

```python
import hashlib
m = hashlib.md5()
m.update("Nobody inspects")
m.update(" the spammish repetition")  # m.update(a); m.update(b) is equivalent to m.update(a+b)
print m.hexdigest()

print hashlib.md5("whatever your string is").hexdigest()
```

#### Bytes and scale
* 1M (million): 1MB
* 1B (million): 1GB
* 1T (trillion): 1TB



