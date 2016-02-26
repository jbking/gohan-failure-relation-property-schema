# Configuration and Assets of Issue Gohan Relation Property Bug

with pre-release gohan 7aeaa1f

## Operation log

```
% ./gohan client service create --name serv1
+----------+--------------------------------------+
| PROPERTY |                VALUE                 |
+----------+--------------------------------------+
| id       | a840de34-fed4-4201-b324-61b4f50d5b59 |
| name     | serv1                                |
+----------+--------------------------------------+

% ./gohan client instance create --name ins1 --service a840de34-fed4-4201-b324-61b4f50d5b59
+----------+--------------------------------------+
| PROPERTY |                VALUE                 |
+----------+--------------------------------------+
| id       | e2c73093-c3ba-4539-a698-2fd8b4c1760c |
| name     | ins1                                 |
| service  | a840de34-fed4-4201-b324-61b4f50d5b59 |
+----------+--------------------------------------+

% ./gohan client instance set --name ins1_alt e2c73093-c3ba-4539-a698-2fd8b4c1760c
Unexpected response: 409 Conflict
```
