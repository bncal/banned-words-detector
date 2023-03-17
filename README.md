# 🧰 Simple banned-words-detector

### Features

- Easy
- Typescript 4.9.5

### Functions

## `hasBannedWords(text: string): boolean`
checks if a word or a long text contains banned words. 
```ts
hasBannedWords("Badword");
// Output: true

hasBannedWords("This is a badword!");
// Output: true

hasBannedWords("Hello world!");
// Output: false

```
## `redactBannedWords(text: string, censor: string = "******"): string`
```ts
console.log(redactBannedWords("Leave this badword outta my badwording face!"));
// Output: Leave this ***** outta my ***** face!

console.log(redactBannedWords("Leave this badword outta my badwording face!", "[REDACTED]"));
// Output: Leave this [REDACTED] outta my [REDACTED] face!

```
