[Home](./index) &gt; [angular-server-side-configuration](./angular-server-side-configuration.md) &gt; [Configuration](./angular-server-side-configuration.configuration.md)

## Configuration class

Discover and apply configuration.

<b>Signature:</b>

```typescript
export declare abstract class Configuration 
```

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [defaultInsertionFilePattern](./angular-server-side-configuration.configuration.defaultinsertionfilepattern.md) |  | `RegExp` | The default pattern for files to have the environment variables inserted into. |
|  [directory](./angular-server-side-configuration.configuration.directory.md) |  | `string` | The directory. Defaults to current working directory. |
|  [replacements](./angular-server-side-configuration.configuration.replacements.md) |  | `Array<(fileContent: string, fileName: string) => string>` | An array of replacement functions. |
|  [variables](./angular-server-side-configuration.configuration.variables.md) |  | `string[]` |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [applyAndSaveRecursively(options)](./angular-server-side-configuration.configuration.applyandsaverecursively.md) |  | Apply the replacements to the content of the matched files and save them asynchronously. |
|  [applyAndSaveTo(file)](./angular-server-side-configuration.configuration.applyandsaveto.md) |  | Apply the replacements to the content of the given file and save it asynchronously. |
|  [applyTo(file)](./angular-server-side-configuration.configuration.applyto.md) |  | Apply the replacements to the content of the given file and return the resulting content as a promise. |
|  [discoverVariables(fileContent)](./angular-server-side-configuration.configuration.discovervariables.md) |  | Search for variables in the received file content. Should return an array of found variable names. |
|  [generateIIFE()](./angular-server-side-configuration.configuration.generateiife.md) |  | Generates the IIFE which the renders the populated environment variables. |
|  [insertVariables(placeholder)](./angular-server-side-configuration.configuration.insertvariables.md) |  | Replace the placeholder with the populated variables wrapped in an IIFE inside a script tag. |
|  [insertVariablesIntoHead()](./angular-server-side-configuration.configuration.insertvariablesintohead.md) |  | Insert the populated variables (wrapped in an IIFE inside a script tag) into the head tag. Appends variables to title tag, or if not found, at the end of the head tag. |
|  [populateVariables()](./angular-server-side-configuration.configuration.populatevariables.md) |  | Generates an object, with the environment variable names being the key and the actual values being the values. |
|  [regexReplace(regex, replaceValue)](./angular-server-side-configuration.configuration.regexreplace.md) |  | Add a replacement for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively. |
|  [renderIIFE(environmentVariables)](./angular-server-side-configuration.configuration.renderiife.md) |  | Render the IIFE |
|  [replace(replacement)](./angular-server-side-configuration.configuration.replace.md) |  | Add a replacement function for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively. The function receives the file content and the file name as parameters and returns the file content with the replacement applied. |
|  [replaceBaseHref(newBaseHref)](./angular-server-side-configuration.configuration.replacebasehref.md) |  | Replace the base href attribute for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively. |
|  [replaceHtmlLang(newHtmlLang)](./angular-server-side-configuration.configuration.replacehtmllang.md) |  | Replace the html lang attribute for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively. |
|  [replaceTagAttribute(tag, attribute, newValue)](./angular-server-side-configuration.configuration.replacetagattribute.md) |  | Replace the attribute value of a tag for the file received through applyTo, applyAndSaveTo or applyAndSaveRecursively. |
|  [searchEnvironmentVariables(options)](./angular-server-side-configuration.configuration.searchenvironmentvariables.md) |  | Searches for environment variable declarations in files matched by file pattern, starting from given directory. |
|  [setDirectory(directory)](./angular-server-side-configuration.configuration.setdirectory.md) |  | Set the directory, where the files to be configured reside in. Default is current working directory. |

