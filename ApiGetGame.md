# Details #

The GetGameApi title search returns game data in an XML document or if an id is given it just returns the data for that specific game. An id overrides a name search.

**Changelog:**

_7-19-11:_
Added Youtube TrailerSupport.
Removed CRC Support.

_7-17-11:_
Added CRC Support.

_6-13-11:_
Added Co-op tag.  Games that are checked with having Co-op capability can now be returned via the API.

Parameters:

**name** (string): Alpha characters only, case insensitive, partial phrases accepted, no partial words.

**id** (int): ID representing a specific game.

**platform** (string) _(optional)_: Platform to filter results by, Alpha-Numeric characters only, See this wiki article for a list of valid platforms [API\_ValidPlatformsList](API_ValidPlatformsList.md)

_example request_:
`http://thegamesdb.net/api/GetGame.php?id=170`

_example result_:

```
<?xml version="1.0" encoding="UTF-8" ?>

<Data>
  <baseImgUrl>http://thegamesdb.net/banners/</baseImgUrl>
  <Game>
    <id>170</id>
    <GameTitle>New Super Mario Bros. Wii</GameTitle>
    <Platform>Nintendo Wii</Platform>
    <Overview>The game follows the traditional storyline of Princess Peach getting kidnapped by Bowser and his children, the Koopalings and Bowser Jr. When Mario, Luigi, Blue Toad, and Yellow Toad are celebrating Princess Peach's birthday in her castle, a large cake rolls in. Immediately, Bowser Jr. and the Koopalings pop out and throw the cake on top of Peach, trapping her. The cake is loaded onto Bowser's airship and it takes off, with Mario, Luigi, and the Toads giving chase. The Toads in the castle then grant them access to the Propeller and Penguin Suits via a cannon.</Overview>
    <ESRB>E - Everyone</ESRB>
    <Genres>
      <genre>Adventure</genre>
      <genre>Sandbox</genre>
    </Genres>
    <Players>4+</Players>
    <Co-op>No</Co-op>
    <Youtube>http://www.youtube.com/watch?v=BrtpflukHSg&amp;hd=1</Youtube>
    <Publisher>Nintendo</Publisher>
    <Developer>Nintendo</Developer>
    <Rating>10</Rating>
    <Images>
      <fanart>
        <original width="1920" height="1080">fanart/original/170-1.jpg</original>
        <thumb>fanart/thumb/170-1.jpg</thumb>
      </fanart>
      <fanart>
        <original width="1920" height="1080">fanart/original/170-2.jpg</original>
        <thumb>fanart/thumb/170-2.jpg</thumb>
      </fanart>
      <fanart>
        <original width="1920" height="1080">fanart/original/170-3.jpg</original>
        <thumb>fanart/thumb/170-3.jpg</thumb>
      </fanart>
      <fanart>
        <original width="1920" height="1080">fanart/original/170-4.jpg</original>
        <thumb>fanart/thumb/170-4.jpg</thumb>
      </fanart>
      <boxart side="back" width="1531" height="2126">boxart/original/back/170-2.jpg</boxart>
      <boxart side="front" width="1530" height="2126">boxart/original/front/170-1.jpg</boxart>
      <banner width="760" height="140">graphical/170-g.jpg</banner>
      <screenshot>
        <original width="832" height="456">screenshots/170-1.jpg</original>
        <thumb>screenshots/thumb/170-1.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-2.jpg</original>
        <thumb>screenshots/thumb/170-2.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-3.jpg</original>
        <thumb>screenshots/thumb/170-3.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-5.jpg</original>
        <thumb>screenshots/thumb/170-5.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-6.jpg</original>
        <thumb>screenshots/thumb/170-6.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-7.jpg</original>
        <thumb>screenshots/thumb/170-7.jpg</thumb>
      </screenshot>
      <screenshot>
        <original width="832" height="456">screenshots/170-8.jpg</original>
        <thumb>screenshots/thumb/170-8.jpg</thumb>
      </screenshot>
    </Images>
  </Game>
</Data>

```