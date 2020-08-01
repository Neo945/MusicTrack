# MusicTrack
Application for keeping the track of all the songs present in the the XML file in SQLite.

### Use the following code in SQLite for testing checking all the data:

```
SELECT Track.title, Artist.name, Album.title, Genre.name 
    FROM Track JOIN Genre JOIN Album JOIN Artist 
    ON Track.genre_id = Genre.ID and Track.album_id = Album.id 
        AND Album.artist_id = Artist.id
    ORDER BY Artist.name LIMIT 3
```
