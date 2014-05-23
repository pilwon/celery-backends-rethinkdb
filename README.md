# celery.backends.rethinkdb


[Celery](http://www.celeryproject.org/)'s custom result backend for [RethinkDB](http://rethinkdb.com/).

The task meta data can be kept in a RethinKDB table.

(Tested with Celery 3.1)


## Usage

1. Copy `rethinkdb.py` to your Celery project.

2. Add the following to `celeryconfig.py`.

```
CELERY_RESULT_BACKEND = '<__name__ of rethinkdb.py from #1>:RethinkBackend'

CELERY_RETHINKDB_BACKEND_SETTINGS = {
    # 'host': '127.0.0.1',
    # 'port': 28015,
    # 'db': 'test',
    # 'auth_key': '',
    # 'timeout': 20,
    # 'table': 'celery_taskmeta',
    # 'options': {}
}

CELERY_RESULT_SERIALIZER = 'json'  # NOTE: MUST BE SET TO JSON
```


## License

<pre>
The MIT License (MIT)

Copyright (c) 2014 Pilwon Huh

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
</pre>


[![Analytics](https://ga-beacon.appspot.com/UA-47034562-21/celery-backends-rethinkdb/readme?pixel)](https://github.com/pilwon/celery-backends-rethinkdb)
