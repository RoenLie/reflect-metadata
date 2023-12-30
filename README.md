# Reflect-Metadata

Partial implementation of TC39 reflect-metadata.
Primarily for use as a lightweight and function activated implementation shim to the proposal.

```typescript 
import { useReflectionShim } from '@roenlie/reflect-metadata';

useReflectionShim();
```


Repeated calls to `useReflectionShim` will have no effect.
If any of the methods being shimmed already exists from a different reflect-metadata shim.
This implementation will not have any effect.

Approximately 1.62kb compiled, 0.66kb gzipped.