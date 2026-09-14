# Convert Anything

JSON, CSV, YAML and Markdown tables, converted between each other offline - with a real CSV parser that handles quoted commas and honest limits on the YAML it supports.

A feature for [Mavis AI](https://www.mavis-ai.com) — a desktop voice assistant.

```
You: "open convert anything"
```

Mavis opens it and stands its own panels down so they are not in your way. Say *"show the interface"* to bring them back.

## Install

From the Mavis Appstore — find **Convert Anything** and click Install.

Or install it directly:

```python
from utils.feature_install import install_from_github
install_from_github("https://github.com/keefng8/convert-anything")
```

## What you can say

- *"open convert anything"*
- *"convert json to csv"*
- *"turn this into a markdown table"*
- *"csv to json"*

These are not matched word for word. Mavis gives them to its language model as examples of intent, so close variations work too.

## How it works

The YAML support is deliberately a subset and says so when it meets anchors, block scalars or multiple documents. Silently mis-parsing those is worse than refusing them.

## Requirements

None. A single HTML file — it runs in your browser, offline, and nothing leaves your machine.

## Building your own

See [Building features for Mavis](https://github.com/keefng8/mavis-feature-docs) — a feature is just a GitHub repository with a `mavis.json`.

## License

MIT — see [LICENSE](LICENSE).
