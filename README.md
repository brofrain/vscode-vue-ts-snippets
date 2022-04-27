# Vue/TS Snippets

> The extension is currently in development and will evolve in the future.\
> Some of the existing triggers may also change.

Simplistic snippets for modern Vue+TypeScript development ([Reactivity Transform](https://vuejs.org/guide/extras/reactivity-transform.html) included).

## Snippets

### Vue SFC

| Trigger | Preview                      |
| ------- | ---------------------------- |
| vjs     | `<script setup>`             |
| vts     | `<script setup lang="ts">`   |
| vtp     | `<template>`                 |
| vcss    | `<style lang="css" scoped>`  |
| vscss   | `<style lang="scss" scoped>` |
| vroute  | `<route lang="yaml">`        |

### Vue Template

| Trigger | Preview                                  | Naming explanation |
| ------- | ---------------------------------------- | ------------------ |
| vtp     | `<template>`                             | TemPlate           |
| vfor    | `v-for="item in array" :key="item"`      | -                  |
| vfori   | `v-for="(item, i) in array" :key="item"` | -                  |
| vif     | `v-if=""`                                | -                  |
| vshow   | `v-show=""`                              | -                  |
| vmod    | `v-model=""`                             | V-MODel            |
| vmodn   | `v-model:property=""`                    | V-MODel-Named      |

### Vue API (JS)

| Trigger | Preview                             | Naming explanation              |
| ------- | ----------------------------------- | ------------------------------- |
| vr      | `ref()`                             | Ref                             |
| vnr     | `const name = ref()`                | Named-Ref                       |
| $r      | `$ref()`                            | $macro-Ref                      |
| $nr     | `const name = $ref()`               | $macro-Named-Ref                |
| $lnr    | `let name = $ref()`                 | $macro-Let-Named-Ref            |
| vc      | `computed(() => )`                  | Computed                        |
| vcb     | `computed(() => { })`               | Computed-with-Body              |
| vnc     | `const name = computed(() => )`     | Named-Computed                  |
| vncb    | `const name = computed(() => { })`  | Named-Computed-with-Body        |
| $c      | `$computed(() => )`                 | $macro-Computed                 |
| $cb     | `$computed(() => { })`              | $macro-Computed-with-Body       |
| $nc     | `const name = $computed(() => )`    | $macro-Named-Computed           |
| $ncb    | `const name = $computed(() => { })` | $macro-Named-Computed-with-Body |
| dp      | `const props = defineProps({ })`    | Define-Props                    |
| $dp     | `const { } = defineProps({ })`      | $macro-Define-Props             |
| de      | `const emit = defineEmits([])`      | Define-Emits                    |

### Vue API (TS)

| Trigger | Preview                               | Naming explanation                       |
| ------- | ------------------------------------- | ---------------------------------------- |
| vrt     | `ref<>()`                             | Ref-with-Type                            |
| vnrt    | `const name = ref<>()`                | Named-Ref-with-Type                      |
| $rt     | `$ref<>()`                            | $macro-Ref-with-Type                     |
| $nrt    | `const name = $ref<>()`               | $macro-Named-Ref-with-Type               |
| $lnrt   | `let name = $ref<>()`                 | $macro-Let-Named-Ref-with-Type           |
| vct     | `computed<>(() => )`                  | Computed-with-Type                       |
| vcbt    | `computed<>(() => { })`               | Computed-with-Body-and-Type              |
| vnct    | `const name = computed<>(() => )`     | Named-Computed-with-Type                 |
| vncbt   | `const name = computed<>(() => { })`  | Named-Computed-with-Body-and-Type        |
| $ct     | `$computed<>(() => )`                 | $macro-Computed-with-Type                |
| $cbt    | `$computed<>(() => { })`              | $macro-Computed-with-Body-and-Type       |
| $nct    | `const name = $computed<>(() => )`    | $macro-Named-Computed-with-Type          |
| $ncbt   | `const name = $computed<>(() => { })` | $macro-Named-Computed-with-Body-and-Type |
| dp      | `const props = defineProps<>()`       | Define-Props                             |
| dpb     | `const props = defineProps<{ }>()`    | Define-Props-with-Body                   |
| dpi     | `const props = defineProps<Props>()`  | Define-Props-with-Interface              |
| $dp     | `const { } = defineProps<>()`         | $macro-Define-Props                      |
| $dpb    | `const { } = defineProps<{ }>()`      | $macro-Define-Props-with-Body            |
| $dpi    | `const { } = defineProps<Props>()`    | $macro-Define-Props-with-Interface       |
| de      | `const emit = defineEmits<>()`        | Define-Emits                             |
| deb     | `const emit = defineEmits<{ }>()`     | Define-Emits-with-Body                   |
| dei     | `const emit = defineEmits<Emits>()`   | Define-Emits-with-Interface              |

### Utility (JS)

| Trigger | Preview                                            | Naming explanation       |
| ------- | -------------------------------------------------- | ------------------------ |
| obk     | `Object.keys()`                                    | OBject-Keys              |
| obv     | `Object.values()`                                  | OBject-Values            |
| obe     | `Object.entries()`                                 | OBject-Entries           |
| obfe    | `Object.fromEntries()`                             | OBject-From-Entries      |
| oba     | `Object.assign()`                                  | OBject-Assign            |
| fin     | `for (const key in object) { }`                    | For-IN                   |
| fof     | `for (const item of array) { }`                    | For-OF                   |
| fofv    | `for (const item of Object.values(object)) { }`    | For-OF-object-Values     |
| fofe    | `for (const [k, v] of Object.entries(object)) { }` | For-OF-object-Entries    |
| fn      | `() => `                                           | FuNction                 |
| fnb     | `() => { }`                                        | FuNction-with-Body       |
| nfn     | `const name = () => `                              | Named-FuNction           |
| nfnb    | `const name = () => { }`                           | Named-FuNction-with-Body |
| im      | `import { } from "module"`                         | IMport                   |
| imd     | `import module from "module"`                      | IMport-Default           |
| ex      | `export `                                          | EXport                   |
| exd     | `export default `                                  | EXport-DEfault           |
| exn     | `export const name = `                             | EXport-Named             |
| clg     | `console.log()`                                    | Console-LoG              |
| cwa     | `console.warn()`                                   | Console-WArn             |
| cer     | `console.error()`                                  | Console-ERror            |

### Utility (TS)

| Trigger | Preview     | Naming explanation |
| ------- | ----------- | ------------------ |
| re      | `Record<> ` | REcord             |

## License

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2022-PRESENT Kajetan Welc

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
