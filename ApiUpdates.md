# Details #

The ApiUpdates returns all the games updated since the time in seconds.

Parameters:

**time** (int): time in seconds.

_example request_:
`http://thegamesdb.net/api/Updates.php?time=2000`

_example result_:

```
<?xml version="1.0" encoding="UTF-8" ?>
<Items>
    <Time>1274641478</Time>
    <Game>1</Game>
</Items>
```