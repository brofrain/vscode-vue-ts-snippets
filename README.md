# Vue/TS Snippets

> The extension is currently in development and will evolve in the future.\
> Some of the existing triggers may also change.

Simplistic snippets for modern Vue+TypeScript development ([Reactivity Transform](https://vuejs.org/guide/extras/reactivity-transform.html) included).

## Snippets

### Common (JS & TS)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`if`

</td>
<td>

```
if (${1:condition}) {
	$0
}
```

</td>
<td>

IF

</td>
</tr>

<tr>
<td>

`ife`

</td>
<td>

```
if (${1:condition}) {
	$2
} else {
	$3
}
```

</td>
<td>

IF-Else

</td>
</tr>

<tr>
<td>

`ok`

</td>
<td>

```
Object.keys(${1:object})
```

</td>
<td>

OBject-Keys

</td>
</tr>

<tr>
<td>

`ov`

</td>
<td>

```
Object.values(${1:object})
```

</td>
<td>

OBject-Values

</td>
</tr>

<tr>
<td>

`oe`

</td>
<td>

```
Object.entries(${1:object})
```

</td>
<td>

OBject-Entries

</td>
</tr>

<tr>
<td>

`ofe`

</td>
<td>

```
Object.fromEntries(${1:entries})
```

</td>
<td>

OBject-From-Entries

</td>
</tr>

<tr>
<td>

`oa`

</td>
<td>

```
Object.assign(${1:target}, ${2:source})
```

</td>
<td>

OBject-Assign

</td>
</tr>

<tr>
<td>

`fin`

</td>
<td>

```
for (const ${2:key} in ${1:object}) {
	$0
}
```

</td>
<td>

For-IN

</td>
</tr>

<tr>
<td>

`fof`

</td>
<td>

```
for (const ${2:item} of ${1:array}) {
	$0
}
```

</td>
<td>

For-OF

</td>
</tr>

<tr>
<td>

`fofv`

</td>
<td>

```
for (const ${2:item} of Object.values(${1:object})) {
	$0
}
```

</td>
<td>

For-OF-object-Values

</td>
</tr>

<tr>
<td>

`fofe`

</td>
<td>

```
for (const [${2:k}, ${3:v}] of Object.entries(${1:object})) {
	$0
}
```

</td>
<td>

For-OF-object-Entries

</td>
</tr>

<tr>
<td>

`fn`

</td>
<td>

```
($1) => $0
```

</td>
<td>

FuNction

</td>
</tr>

<tr>
<td>

`fnb`

</td>
<td>

```
($1) => {
	$0
}
```

</td>
<td>

FuNction-with-Body

</td>
</tr>

<tr>
<td>

`nfn`

</td>
<td>

```
const ${1:name} = ($2) => $0
```

</td>
<td>

Named-FuNction

</td>
</tr>

<tr>
<td>

`nfnb`

</td>
<td>

```
const ${1:name} = ($2) => {
	$0
}
```

</td>
<td>

Named-FuNction-with-Body

</td>
</tr>

<tr>
<td>

`afn`

</td>
<td>

```
async ($1) => $0
```

</td>
<td>

Async-FuNction

</td>
</tr>

<tr>
<td>

`afnp`

</td>
<td>

```
async ($1) => new Promise((resolve) => {
	$0
})
```

</td>
<td>

Async-FuNction-with-Promise

</td>
</tr>

<tr>
<td>

`afnb`

</td>
<td>

```
async ($1) => {
	$0
}
```

</td>
<td>

Async-FuNction-with-Body

</td>
</tr>

<tr>
<td>

`nafn`

</td>
<td>

```
const ${1:name} = async ($2) => $0
```

</td>
<td>

Named-Async-FuNction

</td>
</tr>

<tr>
<td>

`nafnp`

</td>
<td>

```
const ${1:name} = async ($2) => new Promise((resolve) => {
	$0
})
```

</td>
<td>

Named-Async-FuNction-with-Promise

</td>
</tr>

<tr>
<td>

`nafnb`

</td>
<td>

```
const ${1:name} = async ($2) => {
	$0
}
```

</td>
<td>

Named-Async-FuNction-with-Body

</td>
</tr>

<tr>
<td>

`re`

</td>
<td>

```
return $0
```

</td>
<td>

REturn

</td>
</tr>

<tr>
<td>

`reb`

</td>
<td>

```
return { $0 }
```

</td>
<td>

REturn-with-Body

</td>
</tr>

<tr>
<td>

`im`

</td>
<td>

```
import { $2 } from "${1:module}"
```

</td>
<td>

IMport

</td>
</tr>

<tr>
<td>

`imd`

</td>
<td>

```
import ${2:module} from "${1:module}"
```

</td>
<td>

IMport-Default

</td>
</tr>

<tr>
<td>

`ex`

</td>
<td>

```
export $0
```

</td>
<td>

EXport

</td>
</tr>

<tr>
<td>

`exd`

</td>
<td>

```
export default $0
```

</td>
<td>

EXport-DEfault

</td>
</tr>

<tr>
<td>

`exn`

</td>
<td>

```
export const ${1:name} = $0
```

</td>
<td>

EXport-Named

</td>
</tr>

<tr>
<td>

`cl`

</td>
<td>

```
console.log(${1:message})
```

</td>
<td>

Console-Log

</td>
</tr>

<tr>
<td>

`cw`

</td>
<td>

```
console.warn(${1:message})
```

</td>
<td>

Console-Warn

</td>
</tr>

<tr>
<td>

`ce`

</td>
<td>

```
console.error(${1:message})
```

</td>
<td>

Console-Error

</td>
</tr>

</table>

### TS only

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`afnpt`

</td>
<td>

```
async ($1) => new Promise<${2:void}>((resolve) => {
	$0
})
```

</td>
<td>

Async-FuNction-with-Promise-and-Type

</td>
</tr>

<tr>
<td>

`nafnpt`

</td>
<td>

```
const ${1:name} = async ($2) => new Promise<${3:void}>((resolve) => {
	$0
})
```

</td>
<td>

Named-Async-FuNction-with-Promise-and-Type

</td>
</tr>

<tr>
<td>

`re`

</td>
<td>

```
Record<${1:string}, ${2:string}>
```

</td>
<td>

REcord

</td>
</tr>

</table>

### Vue API (JS & TS)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`vr`

</td>
<td>

```
ref($1)
```

</td>
<td>

Ref

</td>
</tr>

<tr>
<td>

`vnr`

</td>
<td>

```
const ${1:name} = ref($2)
```

</td>
<td>

Named-Ref

</td>
</tr>

<tr>
<td>

`$r`

</td>
<td>

```
$ref($1)
```

</td>
<td>

$macro-Ref

</td>
</tr>

<tr>
<td>

`$nr`

</td>
<td>

```
const ${1:name} = $ref($2)
```

</td>
<td>

$macro-Named-Ref

</td>
</tr>

<tr>
<td>

`$lnr`

</td>
<td>

```
let ${1:name} = $ref($2)
```

</td>
<td>

$macro-Let-Named-Ref

</td>
</tr>

<tr>
<td>

`vc`

</td>
<td>

```
computed(() => $1)
```

</td>
<td>

Computed

</td>
</tr>

<tr>
<td>

`vcb`

</td>
<td>

```
computed(() => {
	$0
})
```

</td>
<td>

Computed-with-Body

</td>
</tr>

<tr>
<td>

`vnc`

</td>
<td>

```
const ${1:name} = computed(() => $2)
```

</td>
<td>

Named-Computed

</td>
</tr>

<tr>
<td>

`vncb`

</td>
<td>

```
const ${1:name} = computed(() => {
	$0
})
```

</td>
<td>

Named-Computed-with-Body

</td>
</tr>

<tr>
<td>

`$c`

</td>
<td>

```
$computed(() => $1)
```

</td>
<td>

$macro-Computed

</td>
</tr>

<tr>
<td>

`$cb`

</td>
<td>

```
$computed(() => {
	$0
})
```

</td>
<td>

$macro-Computed-with-Body

</td>
</tr>

<tr>
<td>

`$nc`

</td>
<td>

```
const ${1:name} = $computed(() => $2)
```

</td>
<td>

$macro-Named-Computed

</td>
</tr>

<tr>
<td>

`$ncb`

</td>
<td>

```
const ${1:name} = $computed(() => {
	$0
})
```

</td>
<td>

$macro-Named-Computed-with-Body

</td>
</tr>

<tr>
<td>

`$re`

</td>
<td>

```
return $$($0)
```

</td>
<td>

$macro-REturn

</td>
</tr>

<tr>
<td>

`$reb`

</td>
<td>

```
return $$({ $0 })
```

</td>
<td>

$macro-REturn-with-Body

</td>
</tr>

<tr>
<td>

`vstore`

</td>
<td>

```
import { defineStore } from "pinia"

export const use${1:Store} = defineStore("${2:store}", () => {
	$0

	return { }
})
```

</td>
<td>

pinia-STORE

</td>
</tr>

<tr>
<td>

`vstoress`

</td>
<td>

```
import { acceptHMRUpdate, defineStore } from "pinia"

export const use${1:Store} = defineStore("${2:store}", () => {
	$0

	return { }
})

if (import.meta.hot) {
	import.meta.hot.accept(acceptHMRUpdate(use${1:Store}, import.meta.hot));
}
```

</td>
<td>

pinia-STORE-SSr

</td>
</tr>

<tr>
<td>

`$store`

</td>
<td>

```
import { defineStore } from "pinia"

export const use${1:Store} = defineStore("${2:store}", () => {
	$0

	return $$({ })
})
```

</td>
<td>

$macro-pinia-STORE

</td>
</tr>

<tr>
<td>

`$storess`

</td>
<td>

```
import { acceptHMRUpdate, defineStore } from "pinia"

export const use${1:Store} = defineStore("${2:store}", () => {
	$0

	return $$({ })
})

if (import.meta.hot) {
	import.meta.hot.accept(acceptHMRUpdate(use${1:Store}, import.meta.hot));
}
```

</td>
<td>

$macro-pinia-STORE-SSr

</td>
</tr>

</table>

### Vue API (JS only)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`vdp`

</td>
<td>

```
const props = defineProps({ $1 })
```

</td>
<td>

Define-Props

</td>
</tr>

<tr>
<td>

`$dp`

</td>
<td>

```
const { $2 } = defineProps({ $1 })
```

</td>
<td>

$macro-Define-Props

</td>
</tr>

<tr>
<td>

`vde`

</td>
<td>

```
const emit = defineEmits(["${1:event}"])
```

</td>
<td>

Define-Emits

</td>
</tr>

</table>

### Vue API (TS only)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`vrt`

</td>
<td>

```
ref<$2>($1)
```

</td>
<td>

Ref-with-Type

</td>
</tr>

<tr>
<td>

`vnrt`

</td>
<td>

```
const ${1:name} = ref<$3>($2)
```

</td>
<td>

Named-Ref-with-Type

</td>
</tr>

<tr>
<td>

`$rt`

</td>
<td>

```
$ref<$2>($1)
```

</td>
<td>

$macro-Ref-with-Type

</td>
</tr>

<tr>
<td>

`$nrt`

</td>
<td>

```
const ${1:name} = $ref<$3>($2)
```

</td>
<td>

$macro-Named-Ref-with-Type

</td>
</tr>

<tr>
<td>

`$lnrt`

</td>
<td>

```
let ${1:name} = $ref<$3>($2)
```

</td>
<td>

$macro-Let-Named-Ref-with-Type

</td>
</tr>

<tr>
<td>

`vct`

</td>
<td>

```
computed<$2>(() => $1)
```

</td>
<td>

Computed-with-Type

</td>
</tr>

<tr>
<td>

`vcbt`

</td>
<td>

```
computed<$1>(() => {
	$0
})
```

</td>
<td>

Computed-with-Body-and-Type

</td>
</tr>

<tr>
<td>

`vnct`

</td>
<td>

```
const ${1:name} = computed<$3>(() => $2)
```

</td>
<td>

Named-Computed-with-Type

</td>
</tr>

<tr>
<td>

`vncbt`

</td>
<td>

```
const ${1:name} = computed<$2>(() => {
	$0
})
```

</td>
<td>

Named-Computed-with-Body-and-Type

</td>
</tr>

<tr>
<td>

`$ct`

</td>
<td>

```
$computed<$2>(() => $1)
```

</td>
<td>

$macro-Computed-with-Type

</td>
</tr>

<tr>
<td>

`$cbt`

</td>
<td>

```
$computed<$1>(() => {
	$0
})
```

</td>
<td>

$macro-Computed-with-Body-and-Type

</td>
</tr>

<tr>
<td>

`$nct`

</td>
<td>

```
const ${1:name} = $computed<$3>(() => $2)
```

</td>
<td>

$macro-Named-Computed-with-Type

</td>
</tr>

<tr>
<td>

`$ncbt`

</td>
<td>

```
const ${1:name} = $computed<$2>(() => {
	$0
})
```

</td>
<td>

$macro-Named-Computed-with-Body-and-Type

</td>
</tr>

<tr>
<td>

`vdp`

</td>
<td>

```
const props = defineProps<${1:Props}>()
```

</td>
<td>

Define-Props

</td>
</tr>

<tr>
<td>

`vdpb`

</td>
<td>

```
const props = defineProps<{ $1 }>()
```

</td>
<td>

Define-Props-with-Body

</td>
</tr>

<tr>
<td>

`dpi`

</td>
<td>

```
interface Props {
	$0
}

const props = defineProps<Props>()
```

</td>
<td>

Define-Props-with-Interface

</td>
</tr>

<tr>
<td>

`$dp`

</td>
<td>

```
const { $2 } = defineProps<${1:Props}>()
```

</td>
<td>

$macro-Define-Props

</td>
</tr>

<tr>
<td>

`$dpb`

</td>
<td>

```
const { $2 } = defineProps<{ $1 }>()
```

</td>
<td>

$macro-Define-Props-with-Body

</td>
</tr>

<tr>
<td>

`$dpi`

</td>
<td>

```
interface Props {
	$1
}

const { $2 } = defineProps<Props>()
```

</td>
<td>

$macro-Define-Props-with-Interface

</td>
</tr>

<tr>
<td>

`vde`

</td>
<td>

```
const emit = defineEmits<${1:Emits}>()
```

</td>
<td>

Define-Emits

</td>
</tr>

<tr>
<td>

`vdeb`

</td>
<td>

```
const emit = defineEmits<{
	(e: "${1:event}", value: ${2:number}): void$3
}>()
```

</td>
<td>

Define-Emits-with-Body

</td>
</tr>

<tr>
<td>

`vdei`

</td>
<td>

```
interface Emits {
	(e: "${1:event}", value: ${2:number}): void$0
}

const emit = defineEmits<Emits>()
```

</td>
<td>

Define-Emits-with-Interface

</td>
</tr>

</table>

### Vue SFC

<table>
<tr> <th>Trigger</th> <th>Body</th> </tr>
<tr>
<td>

`vjs`

</td>
<td>

```
<script setup>
$0
</script>
```

</td>
</tr>

<tr>
<td>

`vts`

</td>
<td>

```
<script setup lang="ts">
$0
</script>
```

</td>
</tr>

<tr>
<td>

`vtp`

</td>
<td>

```
<template>
	$0
</template>
```

</td>
</tr>

<tr>
<td>

`vcss`

</td>
<td>

```
<style lang="css" scoped>
$0
</style>
```

</td>
</tr>

<tr>
<td>

`vscss`

</td>
<td>

```
<style lang="scss" scoped>
$0
</style>
```

</td>
</tr>

<tr>
<td>

`vroute`

</td>
<td>

```
<route lang="yaml">
$0
</route>
```

</td>
</tr>

</table>

### Vue Template

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`vtp`

</td>
<td>

```
<template>
	$0
</template>
```

</td>
<td>

TemPlate

</td>
</tr>

<tr>
<td>

`vfor`

</td>
<td>

```
v-for="${2:item} in ${1:array}" :key="${3:item}"
```

</td>
<td>

\-

</td>
</tr>

<tr>
<td>

`vfori`

</td>
<td>

```
v-for="(${2:item}, ${3:i}) in ${1:array}" :key="${4:i}"
```

</td>
<td>

\-

</td>
</tr>

<tr>
<td>

`vif`

</td>
<td>

```
v-if="${1:condition}"
```

</td>
<td>

\-

</td>
</tr>

<tr>
<td>

`vshow`

</td>
<td>

```
v-show="${1:condition}"
```

</td>
<td>

\-

</td>
</tr>

<tr>
<td>

`vmod`

</td>
<td>

```
v-model="${1:variable}"
```

</td>
<td>

V-MODel

</td>
</tr>

<tr>
<td>

`vmodn`

</td>
<td>

```
v-model:${1:property}="${2:variable}"
```

</td>
<td>

V-MODel-Named

</td>
</tr>

</table>

## License

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2022-PRESENT Kajetan Welc

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
