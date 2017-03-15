# Code Standards

## Spaces, Hyphens, or Underscores
Use underscores for contiguous sets of non-compound words (e.g. `long_component_name`) and hyphens for conveying heirarchy (e.g. `long_component_name-child_component`). Spaces should not be used in any file, folder, function name, or URI if at all possible to avoid.

My reasoning for this is basically that "underscore" is considered a "word character" at a very low level, such as in Regular Expressions in which `\w` matches `[a-zA-Z0-9_]` whereas hyphens are a _non-word-character_ and as such are viable to separate sets of words from each other.

For another take on it: https://blog.codinghorror.com/of-spaces-underscores-and-dashes/
