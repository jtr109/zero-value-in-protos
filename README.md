## Example

```ipynb
In [1]: import helloworld_pb2

In [2]: from google.protobuf import json_format

In [3]: a = helloworld_pb2.HelloRequest(name='not empty')

In [4]: a
Out[4]: name: "not empty"

In [5]: a.name
Out[5]: 'not empty'

In [6]: json_format.MessageToJson(a)
Out[6]: '{\n  "name": "not empty"\n}'

In [7]: b = helloworld_pb2.HelloRequest(name='')

In [8]: a
Out[8]: name: "not empty"

In [9]: b
Out[9]:

In [10]: b.name
Out[10]: ''

In [11]: json_format.MessageToJson(b)
Out[11]: '{}'

In [12]: %notebook -e myhistory.ipynb

In [13]: exit
```
