# Details #

The ApiUserRating allows you get and set a user rating on a game.

Parameters:

**accountid** (int): users unique account api id. HowToGetMyApiId

**itemid** (int): game id

**rating** (int 0-10): Optional, user rating. If user rating is 0 then the user rating will be deleted. If no rating is supplied at all the users current rating for the item will be returned.

_example request_:
`http://thegamesdb.net/api/User_Rating.php?accountid=58536D31278176DA&itemid=2`

_example result_:

```
<?xml version="1.0" encoding="UTF-8" ?>
<Data>
    <game>
    <Rating>4.0</Rating>
    </game>
</Data>
```