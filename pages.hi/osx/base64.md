# base64

> बेस 64 प्रस्तुतीकरण का उपयोग करके कोड और डिकोड करें।
> अधिक जानकारी: <https://keith.github.io/xcode-man-pages/bintrans.1>।

- फ़ाइल को कोड करें:

`base64 {{[-i|--input]}} {{सादा_फ़ाइल}}`

- फ़ाइल को डिकोड करें:

`base64 {{[-d|--decode]}} {{[-i|--input]}} {{base64_फ़ाइल}}`

- `stdin` से कोड करें:

`echo -n "{{सादा_फ़ाइल}}" | base64`

- `stdin` से डिकोड करें:

`echo -n {{base64_फ़ाइल}} | base64 {{[-d|--decode]}}`
