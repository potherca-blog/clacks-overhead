# Adding Clacks Overhead

To keep his name alive, we promote adding `Clacks-Overhead` header for [GNU][1] Robbert to any site that wants to commemorate his name.

For servers this can be done by adding a `Clacks-Overhead` header to HTTP responses.

Sadly, non-ASCII characters cannot be used in HTTP headers (see [RFC-7230][4]). So instead of using a `ü`, we'll have to settle for a `u`.

```http
X-Clacks-Overhead: GNU Terry Pratchett, Robbert Muller
```

If you're not a Terry Pratchett fan, you can remove the `Terry Pratchett` part and just use `GNU Robbert Muller`.

If you must have a `ü`, or if you cannot modify the HTTP headers, the following meta-tag can be added to HTML pages:

```html
<meta http-equiv="X-Clacks-Overhead" content="GNU Robbert Müller" />
```

How the Clacks Overhead header should be added depends on the server software that is used. 

Instructions for common server software are provided here:

- [Apache](apache.md)
- [Cloudflare](cloudflare.md)
- [Nginx](nginx.md)

Instructions for more servers, frameworks, and programming languages can be found at http://www.gnuterrypratchett.com/.
