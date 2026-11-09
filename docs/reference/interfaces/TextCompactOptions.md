---
id: TextCompactOptions
title: TextCompactOptions
---

Defined in: [packages/ai/src/types.ts:1584](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1584)

What `TextAdapter.compact` receives.

## Properties

### messages

```ts
messages: ModelMessage<
  | string
  | ContentPart<unknown, unknown, unknown, unknown, unknown>[]
  | null>[];
```

Defined in: [packages/ai/src/types.ts:1572](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1572)

The history to compact.

***

### model

```ts
model: string;
```

Defined in: [packages/ai/src/types.ts:1573](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1573)

***

### signal?

```ts
optional signal?: AbortSignal;
```

Defined in: [packages/ai/src/types.ts:1574](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1574)

***

### systemPrompts?

```ts
optional systemPrompts?: SystemPrompt[];
```

Defined in: [packages/ai/src/types.ts:1578](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1578)

The system prompts of the chat call.

***

### wrapFetch?

```ts
optional wrapFetch?: FetchWrapper;
```

Defined in: [packages/ai/src/types.ts:1591](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1591)

Wraps the fetch of the compaction request.

***

### tools?

```ts
optional tools?: AnyTool[];
```

Defined in: [packages/ai/src/types.ts:1598](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1598)

The tools of the chat call. The provider reads the definitions. The compaction call does not run a tool.

***

### modelOptions?

```ts
optional modelOptions?: Record<string, unknown>;
```

Defined in: [packages/ai/src/types.ts:1600](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1600)

Provider model options of the chat call, including `max_tokens`.

***

### reasoning?

```ts
optional reasoning?: ReasoningRequest;
```

Defined in: [packages/ai/src/types.ts:1602](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1602)

How hard the model thinks on the chat call.

***

### addUsage?

```ts
optional addUsage?: (usage: TokenUsage) => void;
```

Defined in: [packages/ai/src/types.ts:1604](https://github.com/TanStack/ai/blob/main/packages/ai/src/types.ts#L1604)

Report the token usage of the compaction call.
