# 🕉 @sensethenlove/get-form-entries


### 🙏 Description
* Recieves Form Data & responds with an Object
* Converts `<input name="foo" value="bar" />` into `{ foo: 'bar' }`
* Converts `<input name="image" />` into `{ image: File }`
* Converts `<input name="images" multiple />` into `{ images: File[] }`


### ☯️ Install
```bash
pnpm add @sensethenlove/get-form-entries
```

### 💛 Example
```ts
import { getFormEntries } from '@sensethenlove/get-form-entries'

const fields = getFormEntries(formData)
```


### 🧡 Example: FormData (request)
```json
  FormData <entries>
    0: message → "Hello World!"
​​    1: images → File
​​​     <key>: "images"
​​​     <value>: File
​​    2: images → File
​​​     <key>: "images"
​​​     <value>: File
​​    3: images → File
​​​     <key>: "images"
​​     <value>: File
```

### 💚 Example: Fields (response)
```ts
{
  message: 'Hello World!',
  images: [
    File {
      size: 93146,
      type: 'image/jpeg',
      name: 'glew-fl.jpg',
      lastModified: 1683003052322
    },
    File {
      size: 64056,
      type: 'image/jpeg',
      name: 'violet flame.jpg',
      lastModified: 1683003052322
    },
    File {
      size: 46030,
      type: 'image/jpeg',
      name: 'violet-flame.jpg',
      lastModified: 1683003052323
    }
  ]
}
```

### 💖 Our helpful packages!
* [@sensethenlove/jwt](https://www.npmjs.com/package/@sensethenlove/jwt)
* [@sensethenlove/slug](https://www.npmjs.com/package/@sensethenlove/slug)
* [@sensethenlove/toast](https://www.npmjs.com/package/@sensethenlove/toast)
* [@sensethenlove/env-write](https://www.npmjs.com/package/@sensethenlove/env-write)
* [@sensethenlove/svelte-modal](https://www.npmjs.com/package/@sensethenlove/svelte-modal)
* [@sensethenlove/global-style](https://www.npmjs.com/package/@sensethenlove/global-style)
* [@sensethenlove/svelte-turnstile](https://www.npmjs.com/package/@sensethenlove/svelte-turnstile)
* [@sensethenlove/svelte-loading-anchor](https://www.npmjs.com/package/@sensethenlove/svelte-loading-anchor)
