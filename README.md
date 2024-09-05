# ts_mutex

Simple TypeScript Mutex Implementation

## Example Usage

```typescript
const shoppingCartMutex = new Mutex();

shoppingCartMutex.runExclusive(async () => {
  cart.add(items);
  total = await cart.calculateTotal();
});

shoppingCartMutex.runExclusive(async () => {
  await cart.applyCoupons();
  total = await cart.calculateTotal();
});
```

## All imports

```typescript
import { Mutex, ReleaseFunction } from "https://deno.land/x/ts_mutex/mod.ts";
```

## About

Based on (https://dev.to/0916dhkim/simple-typescript-mutex-implementation-5544)

Author: Henrique Emanoel Viana, a Brazilian computer scientist, enthusiast of
web technologies, cel: +55 (41) 99999-4664. URL:
https://sites.google.com/view/henriqueviana

Improvements and suggestions are welcome!
