# Details #

The GetGamesList API search returns a listing of games matched up with loose search terms.

_Note: We have implemented special character stripping and loose word order searching in an attempt to provide better matching and a return a greater number of relevant hits._

**Changelog:**

7-17-11: Added Genre Filtering Support.


**Available Parameters:**

  * name (required)
  * platform (optional) - Filters results by platform (See this wiki article for a list of valid platforms [API\_ValidPlatformsList](API_ValidPlatformsList.md))
  * genre (optional) - Filters results by genre (See this wiki article for a list of valid genres [API\_ValidGenresList](API_ValidGenresList.md))

**Response Items:**

> >id

> >GameTitle

> >ReleaseDate

> >Platform


## Example: ##
A search for "x-men"  http://thegamesdb.net/api/GetGamesList.php?name=x-men  Returns the following:
```
<Data>
  <Game>
    <id>699</id>
    <GameTitle>Spider-Man/X-Men: Arcade's Revenge</GameTitle>
    <ReleaseDate>08/19/1993</ReleaseDate>
    <Platform>|Sega Genesis|</Platform>
  </Game>
  <Game>
    <id>1386</id>
    <GameTitle>The Uncanny X-Men</GameTitle>
    <Platform>|Nintendo Entertainment System (NES)|</Platform>
  </Game>
  <Game>
    <id>665</id>
    <GameTitle>X-Men</GameTitle>
    <ReleaseDate>1993</ReleaseDate>
    <Platform>|Sega Genesis|</Platform>
  </Game>
  <Game>
     <id>3123</id>
     <GameTitle>X-Men - Mojo World</GameTitle>
     <Platform>|Sega Master System|</Platform>
  </Game>
  <Game>
    <id>972</id>
    <GameTitle>X-Men 2: Clone Wars</GameTitle>
    <Platform>|Sega Genesis|</Platform>
  </Game>
  <Game>
    <id>628</id>
    <GameTitle>X-Men vs. Street Fighter</GameTitle>
    <ReleaseDate>09/09/1996</ReleaseDate>
    <Platform>|Sony Playstation|</Platform>
  </Game>
  <Game>
    <id>2468</id>
    <GameTitle>X-Men: Children Of The Atom</GameTitle>
    <ReleaseDate>1994</ReleaseDate>
    <Platform>|Arcade|</Platform>
  </Game>
</Data>
```