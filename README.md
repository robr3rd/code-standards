# Code Standards
> Note: If anything goes EXPLICITLY against any "contextual standards" (language/framework/project/company), those standards--not these--win.


## Table of Contents
- Naming Conventions
	- Spaces, Hyphens, and Underscores
	- Code
		- Markup
		- Programming


## Naming Conventions
### Spaces, Hyphens, and Underscores
Use underscores for contiguous sets of non-compound words (e.g. `long_component_name`) and hyphens for conveying heirarchy (e.g. `long_component_name-child_component`).

My reasoning for this is basically that "underscore" is considered a "word character" at a very low level, such as in Regular Expressions in which `\w` matches `[a-zA-Z0-9_]` whereas hyphens are a _non-word-character_ and as such are viable to separate sets of words from each other.  ([another take on it](https://blog.codinghorror.com/of-spaces-underscores-and-dashes/))

Spaces should not be used in any file, folder, function name, or URI if at all possible.


### Code
#### Markup/CSS
- XML/HTML: Follow strict XML or X/HTML standards, respectively, e.g. `disabled="disabled"` and `<input />.
	- Attributes: `kebab-case` only
- CSS classes: Follow BEM, but allow the use of underscores in accordance with the aforementioned space/hyphen/underscore standards.

#### Programming
- **Variables**: `snake_case`
- **Functions/Methods**: `camelCase`
- **Classes/Namespaces**: `StudlyCase`

The reasons for this are simple and basically come down to a desire for easy and instant identification of a symbol's purpose, while maximizing readability on the most-used symbol:

- **Variables**: `snake_case` due to being objectively* faster/easier to read with higher accuracy and there will almost always be more of these than other types of symbols.
- **Methods**: `camelCase` _looks_ "bigger" than `snake_case` but isn't quite as "big"-looking as `StudlyCase`.
- **Classes**: `StudlyCase` is "biggest".

> *[Research Paper](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.158.9499) ([Direct Link](http://www.cs.loyola.edu/~binkley/papers/icpc09-clouds.pdf))
