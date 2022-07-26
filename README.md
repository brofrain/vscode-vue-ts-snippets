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

`.if`

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

`.ife`

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

`.ok`

</td>
<td>

```
Object.keys(${1:object})
```

</td>
<td>

Object-Keys

</td>
</tr>

<tr>
<td>

`.ov`

</td>
<td>

```
Object.values(${1:object})
```

</td>
<td>

Object-Values

</td>
</tr>

<tr>
<td>

`.oe`

</td>
<td>

```
Object.entries(${1:object})
```

</td>
<td>

Object-Entries

</td>
</tr>

<tr>
<td>

`.ofe`

</td>
<td>

```
Object.fromEntries(${1:entries})
```

</td>
<td>

Object-From-Entries

</td>
</tr>

<tr>
<td>

`.oa`

</td>
<td>

```
Object.assign(${1:target}, ${2:source})
```

</td>
<td>

Object-Assign

</td>
</tr>

<tr>
<td>

`.fin`

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

`.fof`

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

`.fofv`

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

`.fofe`

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

`.f`

</td>
<td>

```
($1) => $0
```

</td>
<td>

Function

</td>
</tr>

<tr>
<td>

`.fb`

</td>
<td>

```
($1) => {
	$0
}
```

</td>
<td>

Function-with-Body

</td>
</tr>

<tr>
<td>

`.nf`

</td>
<td>

```
const ${1:name} = ($2) => $0
```

</td>
<td>

Named-Function

</td>
</tr>

<tr>
<td>

`.nfb`

</td>
<td>

```
const ${1:name} = ($2) => {
	$0
}
```

</td>
<td>

Named-Function-with-Body

</td>
</tr>

<tr>
<td>

`.af`

</td>
<td>

```
async ($1) => $0
```

</td>
<td>

Async-Function

</td>
</tr>

<tr>
<td>

`.afp`

</td>
<td>

```
async ($1) => new Promise((resolve) => {
	$0
})
```

</td>
<td>

Async-Function-with-Promise

</td>
</tr>

<tr>
<td>

`.afb`

</td>
<td>

```
async ($1) => {
	$0
}
```

</td>
<td>

Async-Function-with-Body

</td>
</tr>

<tr>
<td>

`.naf`

</td>
<td>

```
const ${1:name} = async ($2) => $0
```

</td>
<td>

Named-Async-Function

</td>
</tr>

<tr>
<td>

`.nafp`

</td>
<td>

```
const ${1:name} = async ($2) => new Promise((resolve) => {
	$0
})
```

</td>
<td>

Named-Async-Function-with-Promise

</td>
</tr>

<tr>
<td>

`.nafb`

</td>
<td>

```
const ${1:name} = async ($2) => {
	$0
}
```

</td>
<td>

Named-Async-Function-with-Body

</td>
</tr>

<tr>
<td>

`.re`

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

`.reb`

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

`.im`

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

`.imd`

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

`.ex`

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

`.exd`

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

`.exn`

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

`.cl`

</td>
<td>

```
console.log(${1:message})
```

</td>
<td>

Console-LoG

</td>
</tr>

</table>

### TS only

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`.afpt`

</td>
<td>

```
async ($1) => new Promise<${2:void}>((resolve) => {
	$0
})
```

</td>
<td>

Async-Function-with-Promise-and-Type

</td>
</tr>

<tr>
<td>

`.nafpt`

</td>
<td>

```
const ${1:name} = async ($2) => new Promise<${3:void}>((resolve) => {
	$0
})
```

</td>
<td>

Named-Async-Function-with-Promise-and-Type

</td>
</tr>

<tr>
<td>

`.rec`

</td>
<td>

```
Record<${1:string}, ${2:string}>
```

</td>
<td>

RECord

</td>
</tr>

</table>

### Vue API (JS & TS)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`.r`

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

`.nr`

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

`.c`

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

`.cb`

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

`.nc`

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

`.ncb`

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

`.pstore`

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

Pinia-STORE

</td>
</tr>

<tr>
<td>

`.pstoress`

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

Pinia-STORE-SSr

</td>
</tr>

<tr>
<td>

`$pstore`

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

$macro-Pinia-STORE

</td>
</tr>

<tr>
<td>

`$pstoress`

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

$macro-Pinia-STORE-SSr

</td>
</tr>

</table>

### Vue API (JS only)

<table>
<tr> <th>Trigger</th> <th>Body</th> <th>Naming explanation</th> </tr>
<tr>
<td>

`.dp`

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

`.de`

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

`.rt`

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

`.nrt`

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

`.ct`

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

`.cbt`

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

`.nct`

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

`.ncbt`

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

`.dp`

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

`.dpb`

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

`.dpi`

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

`.de`

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

`.deb`

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

`.dei`

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

`.vjs`

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

`.vts`

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

`.vtp`

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

`.vcss`

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

`.vscss`

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

`.vroute`

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

`.vtp`

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

`.vfor`

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

`.vfor`

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

`.vif`

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

`.vshow`

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

`.vmod`

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

`.vmodn`

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
