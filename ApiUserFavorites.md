# Details #

The ApiUserFavorites allows you get, set and remove a user game favorite. Always returns a list of the current favorite game id's.

Parameters:

**accountid** (int): users unique account api id. HowToGetMyApiId

**type** (string add|remove): Optional. sets the action (add or remove) for the request.

**gameid** (int): Optional, required if type is set. The game id to preform the type on.

_example request_:
`http://thegamesdb.net/api/User_Favorites.php?accountid=58536D31278176DA&type=add&gameid=2`

_example result_:

```
<?xml version="1.0" encoding="UTF-8" ?>
<Favorites>
    <Game>1</Game>
    <Game>2</Game>
</Favorites>
```