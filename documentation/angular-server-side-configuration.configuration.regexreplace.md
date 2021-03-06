[Home](./index) &gt; [angular-server-side-configuration](./angular-server-side-configuration.md) &gt; [Configuration](./angular-server-side-configuration.configuration.md) &gt; [regexReplace](./angular-server-side-configuration.configuration.regexreplace.md)

## Configuration.regexReplace() method

Add a replacement for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively.

<b>Signature:</b>

```typescript
regexReplace(regex: RegExp, replaceValue: string): this;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  regex | `RegExp` | A RegExp object or literal. The match or matches are replaced with replaceValue. |
|  replaceValue | `string` | The value that replaces the substring matched by the regex parameter. |

<b>Returns:</b>

`this`

This instance.

