# Child vs Node Selectors

**Activity:** To reveal how each selector works, remove the comments from each code block in `<style>...</style>` from the example file *childnodeselector.html*.

## 1. Child Selector

<u>Child selectors</u> use the `>` combinator to target elements that are direct children of a specified parent.

The following child selector targets `<h1>` elements that are direct children of a `<section>` element.

```
section > h1
```

> <small>**Note:** The example above only targets `<h1>` under `<section>`. Indirect descendants are not affected.</small>


## 2. Node Selectors

<u>Node selectors</u> target nodes (elements) based on relationships but are not limited to direct parent-child relationships.

### a. Descendant Selector

The <u>descendent selector</u> is a node selector because it targets all `<h1>` elements that are descendants of a `<section>` element, regardless of their nesting level.

```
section h1
```

> <small>**Note:** The example above targets `<h1>` elements in `<section>` even if they are nested.</small>


### b. Next Sibling Selector

The <u>next sibling selector</u> is a node selector because it targets `<h1>` elements immediately following an `<h2>` element.

```
h2 + h1
```

> <small>**Note:** The example above targets a `<h1>` element that directly follows a `<h2>` element under the same parent.</small>


### c. Subsequent Sibling Selector

The <u>subsequent sibling selector</u> is a node selector because targets all `<h1>` elements that follow an `<h2>` element, sharing the same parent, even if other elements exist in between.

```
h2 ~ h1
```

> <small>**Note:** The example above targets all `<h1>` siblings after an `<h2>` element.</small>
