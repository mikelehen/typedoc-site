---
layout: "guide"
tags: tag
title: "@template"
---

# @template

{% include 'tag-info', kind: 'Block' %}

The `@template` tag is used to document a type parameter of a function, method, class, interface or type alias.

TypeDoc recognizes the `@template` tag as an alias of `@typeParam` for compatibility with JavaScript
projects using TypeScript via doc comments. For TypeScript projects, the TSDoc standard
[`@typeParam`](/tags/typeParam/) tag should be preferred.

## Example

```js
/**
 * @template {string} T - the identity type
 */
export function identity(x) {
    return x;
}
```

## See Also

-   The [`@typeParam`](/tags/typeParam/) tag
