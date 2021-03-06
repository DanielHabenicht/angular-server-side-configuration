[Home](./index) &gt; [angular-server-side-configuration](./angular-server-side-configuration.md) &gt; [Configuration](./angular-server-side-configuration.configuration.md) &gt; [applyAndSaveRecursively](./angular-server-side-configuration.configuration.applyandsaverecursively.md)

## Configuration.applyAndSaveRecursively() method

Apply the replacements to the content of the matched files and save them asynchronously.

<b>Signature:</b>

```typescript
applyAndSaveRecursively(options?: ApplyAndSaveRecursivelyOptions): Promise<string[]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  options | `ApplyAndSaveRecursivelyOptions` | Options for applying replacements. |

<b>Returns:</b>

`Promise<string[]>`

A promise, which resolves to the matched files, after all matched files have had the replacements applied.

