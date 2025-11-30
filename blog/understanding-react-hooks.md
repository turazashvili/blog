---
title: Understanding React Hooks
date: 2025-12-01
description: A deep dive into useState and useEffect.
---

# Understanding React Hooks

Hooks let you use state and other React features without writing a class.

## Common Hooks

### useState

```javascript
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

### useEffect

`useEffect` lets you perform side effects in function components.

```javascript
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `You clicked ${count} times`;
  });
}
```
