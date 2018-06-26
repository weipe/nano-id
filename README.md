# nano-id
A unique string ID generator for Clojure and ClojureScript.

### Secure
nano-id uses [SecureRandom](https://docs.oracle.com/javase/7/docs/api/java/security/SecureRandom.html) and [crypto](https://developer.mozilla.org/en-US/docs/Web/API/Window/crypto) to generate cryptographically strong random IDs with a proper distribution of characters.

### Compact
nano-id generates compact IDs with just 21 characters. By using a larger alphabet than UUID, nano-id can generate a greater number of unique IDs, when compared to UUID, with fewer characters (21 versus 36).

### URL-Friendly
By default nano-id uses URL-friendly characters `[A-Za-z0-9_~]`. Perfect for unique identifiers in web applications.

### Customizable
TBD

### Tested
TBD

## Usage
Add to your project.clj: `[nano-id "0.9.0-SNAPSHOT"]`.

```clojure
(require [nano-id.core :refer [nano-id]])

(nano-id)    ; => YUpA5UAUMrDYHwh0bT~DB

(nano-id 10) ; => wcjXqT2Lhh
```

## Copyright and license
Code copyright 2018 [nano-id authors](https://github.com/zelark/nano-id/graphs/contributors) and [Andrey Sitnik](https://github.com/ai). Code released under the [MIT License](https://github.com/zelark/nano-id/blob/master/LICENSE).

Based on the original [NanoId](https://github.com/ai/nanoid) for JavaScript by [Andrey Sitnik](https://github.com/ai/).
