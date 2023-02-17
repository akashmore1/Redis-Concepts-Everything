### Always refer to redis documentation for commands

```
https://redis.io/commands/
```

# Commands used for setting and retrieving _String Data_

![String commands](./GetterSetterString.png)

# Variations of SET:

1. **_EX_** is used for setting when our data will expire.
2. **_XX_** is used for setting value to key only if key is present in cache already.

```
SET colour 'red' XX
```

👆This will first check if key is present in cache or redis.
if(present) then colour will be set to red and returned null.
else colour will not be set and null will be returned.
