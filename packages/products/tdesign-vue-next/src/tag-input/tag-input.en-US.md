:: BASE_DOC ::

## API
### TagInput Props

name | type | default | description | required
-- | -- | -- | -- | --
autoWidth | Boolean | false | \- | N
clearable | Boolean | false | \- | N
collapsedItems | Slot / Function | - | Typescript：`TNode<{ value: TagInputValue; collapsedTags: TagInputValue; count: number }>`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
disabled | Boolean | - | \- | N
dragSort | Boolean | false | \- | N
excessTagsDisplayType | String | break-line | options：scroll/break-line | N
inputProps | Object | - | Typescript：`InputProps`，[Input API Documents](./input?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
inputValue | String / Number | '' | input value。`v-model:inputValue` is supported。Typescript：`InputValue`，[Input API Documents](./input?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
defaultInputValue | String / Number | '' | input value。uncontrolled property。Typescript：`InputValue`，[Input API Documents](./input?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
label | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
max | Number | - | max tag number | N
minCollapsedNum | Number | 0 | \- | N
placeholder | String | undefined | placeholder description | N
readonly | Boolean | false | \- | N
size | String | medium | options：small/medium/large | N
status | String | - | options：default/success/warning/error | N
suffix | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
suffixIcon | Slot / Function | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
tag | String / Slot / Function | - | Typescript：`string \| TNode<{ value: string \| number }>`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
tagProps | Object | - | Typescript：`TagProps`，[Tag API Documents](./tag?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
tips | String / Slot / Function | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
value | Array | [] | value。`v-model` and `v-model:value` is supported。Typescript：`TagInputValue` `type TagInputValue = Array<string \| number>`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
defaultValue | Array | [] | value。uncontrolled property。Typescript：`TagInputValue` `type TagInputValue = Array<string \| number>`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts) | N
valueDisplay | String / Slot / Function | - | Typescript：`string \| TNode<{ value: TagInputValue; onClose: (index: number, item?: any) => void }>`。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/blob/develop/src/common.ts) | N
onBlur | Function |  | Typescript：`(value: TagInputValue, context: { inputValue: InputValue; e: FocusEvent }) => void`<br/>trigger on blur | N
onChange | Function |  | Typescript：`(value: TagInputValue, context: TagInputChangeContext) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputChangeContext { trigger: TagInputTriggerSource; index?: number; item?: string \| number; e?: MouseEvent \| KeyboardEvent }`<br/><br/>`type TagInputTriggerSource = 'enter' \| 'tag-remove' \| 'backspace' \| 'clear'`<br/> | N
onClear | Function |  | Typescript：`(context: { e: MouseEvent }) => void`<br/> | N
onDragSort | Function |  | Typescript：`(context: TagInputDragSortContext) => void`<br/>trigger on drag sort。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputDragSortContext { newTags: TagInputValue; currentIndex: number; current: string \| number; targetIndex: number; target: string \| number }`<br/> | N
onEnter | Function |  | Typescript：`(value: TagInputValue, context: { e: KeyboardEvent; inputValue: InputValue }) => void`<br/> | N
onFocus | Function |  | Typescript：`(value: TagInputValue, context: { inputValue: InputValue; e: FocusEvent }) => void`<br/>trigger on focus | N
onInputChange | Function |  | Typescript：`(value: InputValue, context?: InputValueChangeContext) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface InputValueChangeContext { e?: InputEvent \| MouseEvent \| CompositionEvent \| KeyboardEvent; trigger: 'input' \| 'clear' \| 'enter'  }`<br/> | N
onMouseenter | Function |  | Typescript：`(context: { e: MouseEvent }) => void`<br/>trigger on mouseenter | N
onMouseleave | Function |  | Typescript：`(context: { e: MouseEvent }) => void`<br/>trigger on mouseleave | N
onPaste | Function |  | Typescript：`(context: { e: ClipboardEvent; pasteValue: string }) => void`<br/> | N
onRemove | Function |  | Typescript：`(context: TagInputRemoveContext) => void`<br/>[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputRemoveContext { value: TagInputValue; index: number; item: string \| number; e?: MouseEvent \| KeyboardEvent; trigger: TagInputRemoveTrigger }`<br/><br/>`type TagInputRemoveTrigger = 'tag-remove' \| 'backspace'`<br/> | N

### TagInput Events

name | params | description
-- | -- | --
blur | `(value: TagInputValue, context: { inputValue: InputValue; e: FocusEvent })` | trigger on blur
change | `(value: TagInputValue, context: TagInputChangeContext)` | [see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputChangeContext { trigger: TagInputTriggerSource; index?: number; item?: string \| number; e?: MouseEvent \| KeyboardEvent }`<br/><br/>`type TagInputTriggerSource = 'enter' \| 'tag-remove' \| 'backspace' \| 'clear'`<br/>
clear | `(context: { e: MouseEvent })` | \-
drag-sort | `(context: TagInputDragSortContext)` | trigger on drag sort。[see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputDragSortContext { newTags: TagInputValue; currentIndex: number; current: string \| number; targetIndex: number; target: string \| number }`<br/>
enter | `(value: TagInputValue, context: { e: KeyboardEvent; inputValue: InputValue })` | \-
focus | `(value: TagInputValue, context: { inputValue: InputValue; e: FocusEvent })` | trigger on focus
input-change | `(value: InputValue, context?: InputValueChangeContext)` | [see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface InputValueChangeContext { e?: InputEvent \| MouseEvent \| CompositionEvent \| KeyboardEvent; trigger: 'input' \| 'clear' \| 'enter'  }`<br/>
mouseenter | `(context: { e: MouseEvent })` | trigger on mouseenter
mouseleave | `(context: { e: MouseEvent })` | trigger on mouseleave
paste | `(context: { e: ClipboardEvent; pasteValue: string })` | \-
remove | `(context: TagInputRemoveContext)` | [see more ts definition](https://github.com/Tencent/tdesign-vue-next/tree/develop/src/tag-input/type.ts)。<br/>`interface TagInputRemoveContext { value: TagInputValue; index: number; item: string \| number; e?: MouseEvent \| KeyboardEvent; trigger: TagInputRemoveTrigger }`<br/><br/>`type TagInputRemoveTrigger = 'tag-remove' \| 'backspace'`<br/>