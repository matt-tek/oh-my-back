### How to run the code
```
uvicorn app.main:app --reload
```

### Project structure
```
.
├── app                  # "app" is a Python package
│   ├── __init__.py      # this file makes "app" a "Python package"
│   ├── main.py          # "main" module, e.g. import app.main
│   ├── dependencies.py  # "dependencies" module, e.g. import app.dependencies
│   └── routers          # "routers" is a "Python subpackage"
│   │   ├── __init__.py  # makes "routers" a "Python subpackage"
│   │   ├── items.py     # "items" submodule, e.g. import app.routers.items
│   │   └── users.py     # "users" submodule, e.g. import app.routers.users
│   └── schemas          # "schemas" is a "Python subpackage"
│       ├── __init__.py  # makes "internal" a "Python subpackage"
│       └── todo.py      # "admin" submodule, e.g. import app.internal.admin
```