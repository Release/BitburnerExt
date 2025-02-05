<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [NS](./bitburner.ns.md) &gt; [printf](./bitburner.ns.printf.md)

## NS.printf() method

Prints a formatted string to the script’s logs.

**Signature:**

```typescript
printf(format: string, ...args: any[]): void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  format | string | Format of the message. |
|  args | any\[\] | Value(s) to be printed. |

**Returns:**

void

## Remarks

RAM cost: 0 GB

- See [print](./bitburner.ns.print.md) for how to add color to your printed strings.

- For more detail, see: https://github.com/alexei/sprintf.js

## Example


```js
const name = "Bit";
const age = 4;
ns.printf("My name is %s.", name);
ns.printf("I'm %d seconds old.", age);
ns.printf("My age in binary is %b.", age);
ns.printf("My age in scientific notation is %e.", age);
ns.printf("In %d seconds, I'll be %s.", 6, "Byte");
ns.printf("Am I a nibble? %t", (4 === age));
ns.tail();
```

