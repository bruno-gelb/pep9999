# Contributing

When contributing to this repository, please follow this guide.

## General rules

1. Use [issues](https://github.com/nazarov-tech/pep9999/issues)
to describe the work that needs to be done
1. While editing PEP, follow the style guide required by [PEP 12](https://www.python.org/dev/peps/pep-0012)
1. You should lint your changes. Install the Python requirements from `requirements.txt`, then `rst-lint README.rst`
1. Do not use any language other than English

## Commit messages

1. Separate subject from body with a blank line
1. Limit the subject line to 50 characters
1. Capitalize the subject line
1. Do not end the subject line with a period
1. Use the imperative mood in the subject line
1. Wrap the body at 72 characters
1. Use the body to explain what and why vs. how

For example:

```
Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```

[source](https://chris.beams.io/posts/git-commit/)