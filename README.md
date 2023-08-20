# API

db.json contains an object for serving data via My JSON Server. Properties in this object become endpoints that can be used to mimic 3rd party APIs. These properties can be arrays of objects, whose id fields can then be used in detail endpoints.

## Movies
This endpoint contains an array of supplemental data for the Movies API, used in the React tutorial series. The data is served through My JSON Server at the following endpoints:

**GET**: `my-json-server.typicode.com/dCC-Online/api/movies`
```
[
  {
      "id": "The Dark Knight",
      "poster_url": "https://image.tmdb.org/t/p/w500/1hRoyzDtpgMU7Dz4JF22RANzQO7.jpg",
      "release_date": "2008-07-18"
  },
  {
      "id": "Inception",
      "poster_url": "https://image.tmdb.org/t/p/w500/9gk7adHYeDvHkCSEqAvQNLV5Uge.jpg",
      "release_date": "2010-07-16"
  }
  ...
]
```

**GET**: `my-json-server.typicode.com/dCC-Online/api/movies/The Dark Knight`
```
{
  "id": "The Dark Knight",
  "poster_url": "https://image.tmdb.org/t/p/w500/1hRoyzDtpgMU7Dz4JF22RANzQO7.jpg",
  "release_date": "2008-07-18"
}
```
