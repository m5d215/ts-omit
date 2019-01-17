# ts-omit

![version](https://badgen.net/npm/v/@m5d215/ts-omit?icon=npm)
![license](https://badgen.net/npm/license/@m5d215/ts-omit)
![dependents](https://badgen.net/npm/dependents/@m5d215/ts-omit)

[![CircleCI](https://circleci.com/gh/m5d215/ts-omit.svg?style=svg)](https://circleci.com/gh/m5d215/ts-omit)

Delete properties from type at compilation time.

```sh
yarn add --dev @m5d215/ts-omit
```

```ts
import Omit from '@m5d215/ts-omit'

interface Person {
  name: string
  age: number
}

// Anonymous is { age: number }
type Anonymous = Omit<Person, 'name'>
```
