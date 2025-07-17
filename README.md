<table><tr><td>
<p>Sunday 13th of July 2025 Robbert Müller has passed away, surrounded by his loved ones.

<p>After battling cancer for several years, Robert left this plane of existence for a hopefully better one.

<p>Our hearts and thoughts go out to his bereaved.

<p>We will miss him dearly, but we will always remember his contributions to the community and the joy he brought to our lives.

_“A man is not dead while his name is still spoken.”_

![ GNU Robbert Müller.gif][2]

</td><td align="center">

![robbert.jpg][3]
Robbert Müller<br>1979 † 2025
  
</td></tr></table>

To keep his name alive, we promote adding `Clacks-Overhead` header for [GNU][1] Robbert Müller to any site that wants to commemorate his name.

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

For instructions on how to add the `X-Clacks-Overhead` header to web servers, see the ["Add headers" page](add-headers/)

After setting up the header, [verify it works](verify-headers/).

[1]: https://wiki.lspace.org/GNU_Terry_Pratchett
[2]: img/GNU-Robbert-Muller.gif
[3]: img/robbert.jpg
[4]: https://www.rfc-editor.org/rfc/rfc7230#section-3.2
