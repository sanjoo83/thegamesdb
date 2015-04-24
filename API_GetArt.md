# Overview #

This API feature returns a list of available artwork types and locations specific to the requested game id in the database.  It also lists the resolution of any images available.  Scrapers can be set to use a minimum or maximum resolution for specific images.

Accepted arguments for the GetArt.php GET request:
  * id
    1. **_Integer_**
    1. The numeric ID of the game in our database that you like to fetch artwork details for
    1. _example:_ id=910


---


# Usage Example #

An API call with the numeric id of the game desired:

e.g. _http://thegamesdb.net/api/GetArt.php?id=170_

Returns the Following

# Response: #
```
<?xml version="1.0" encoding="UTF-8" ?>

<Data>
  <baseImgUrl>http://thegamesdb.net/banners/</baseImgUrl>
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
</Data>
```