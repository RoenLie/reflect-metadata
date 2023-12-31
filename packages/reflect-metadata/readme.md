# Reflect-Metadata

Partial implementation of TC39 reflect-metadata.
Primarily for use as a lightweight and function activated implementation shim to the proposal.

### Manual activation
```typescript 
import { useReflectMetadata } from '@roenlie/reflect-metadata';

useReflectMetadata();
```

### Automatic activation
```typescript
import '@roenlie/reflect-metadata/use';
```
```html
<script type="module" src="@roenlie/reflect-metadata/use"></script>
```


Repeated calls to `useReflectMetadata` will have no effect.
If any of the methods being shimmed already exists from a different reflect-metadata shim, this implementation will not have any effect.

Approximately 1.70kb compiled, 0.70kb gzipped.