## Python client library for Domino API

This library permits interaction with a Domino deployment from Python using the [Domino API](https://dominodatalab.github.io/api-docs/)

Domino API belongs to [Domino Data Lab](https://www.dominodatalab.com/)

Install
```bash
pip install git+https://github.com/reclada/domino_api.git
```

Use:
```python
from reclada.domino import Domino

client = Domino(token="your api token", trial=True)
client.start_run("username", "project", ["main.py"])
print(client.runs("username", "project"))
```