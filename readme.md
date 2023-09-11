# Example Remark Plugin (`mdast`/`unist`)

```ts
import type { Plugin } from "unified";
import type { Root } from "mdast";

interface PluginConfig {}

/**
 * Unified/Remark `mdast` plugin.
 * <Options Type, InputAST, OutputAST>
 */
const remarkPlugin: Plugin<[PluginConfig], Root> = (config) => {
  return async (tree) => {
    // ...do stuff
    return tree;
  };
};

export default remarkPlugin;
```

# Example Rehype Plugin (`hast`/`unist`)

```ts
import type { Plugin } from "unified";
import type { Root } from "hast";

interface PluginConfig {}

/**
 * Unified/Rehype `hast` plugin.
 */
const rehypePlugin: Plugin<[PluginConfig], Root> = (config) => {
  return async (tree) => {
    // ...do stuff
    return tree;
  };
};

export default rehypePlugin;
```
