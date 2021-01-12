## Dominino data labs API client

Example:

```python
from reclada.domino import Domino

client = Domino(token="your api token", trial=True)
client.start_run("username", "project", ["main.py"])
print(client.runs("username", "project"))
```