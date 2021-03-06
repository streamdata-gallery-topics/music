---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Delete Following
  description: '[Unfollow Artists or Users](https://developer.spotify.com/web-api/unfollow-artists-users/)'
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /albums:
    get:
      summary: Get Albums
      description: '[Get Several Albums](https://developer.spotify.com/web-api/get-several-albums/)'
      operationId: get-several-albumshttpsdeveloperspotifycomwebapigetseveralalbums
      x-api-path-slug: albums-get
      parameters:
      - in: query
        name: ids
        description: A comma-separated list of IDs
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      responses:
        200:
          description: OK
      tags:
      - Music
      - Albums
  /albums/{id}:
    get:
      summary: Get Album
      description: '[Get an Album](https://developer.spotify.com/web-api/get-album/)'
      operationId: get-an-albumhttpsdeveloperspotifycomwebapigetalbum
      x-api-path-slug: albumsid-get
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the album
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      responses:
        200:
          description: OK
      tags:
      - Music
      - Albums
  /albums/{id}/tracks:
    get:
      summary: Get Album Tracks
      description: '[Get an Album''s Tracks](https://developer.spotify.com/web-api/get-albums-tracks/)'
      operationId: get-an-albums-trackshttpsdeveloperspotifycomwebapigetalbumstracks
      x-api-path-slug: albumsidtracks-get
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the album
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - Album
      - Tracks
  /artists:
    get:
      summary: Get Artists
      description: '[Get Several Artists](https://developer.spotify.com/web-api/get-several-artists/)'
      operationId: get-several-artistshttpsdeveloperspotifycomwebapigetseveralartists
      x-api-path-slug: artists-get
      parameters:
      - in: query
        name: ids
        description: A comma-separated list of IDs
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
  /artists/{id}:
    get:
      summary: Get Artist
      description: '[Get an Artist](https://developer.spotify.com/web-api/get-artist/)'
      operationId: get-an-artisthttpsdeveloperspotifycomwebapigetartist
      x-api-path-slug: artistsid-get
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the artist
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
  /artists/{id}/albums:
    get:
      summary: Get Artist Albums
      description: '[Get an Artist''s Albums](https://developer.spotify.com/web-api/get-artists-albums/)'
      operationId: get-an-artists-albumshttpsdeveloperspotifycomwebapigetartistsalbums
      x-api-path-slug: artistsidalbums-get
      parameters:
      - in: query
        name: album_type
        description: Filter by album types
      - in: path
        name: id
        description: The Spotify ID for the artist
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
      - Albums
  /artists/{id}/related-artists:
    get:
      summary: Get Artist Related ARtists
      description: '[Get an Artist''s Related Artists](https://developer.spotify.com/web-api/get-related-artists/)'
      operationId: get-an-artists-related-artistshttpsdeveloperspotifycomwebapigetrelatedartists
      x-api-path-slug: artistsidrelatedartists-get
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the artist
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
  /artists/{id}/top-tracks:
    get:
      summary: Get Artist Top Tracks
      description: '[Get an Artist''s Top Tracks](https://developer.spotify.com/web-api/get-artists-top-tracks/)'
      operationId: get-an-artists-top-trackshttpsdeveloperspotifycomwebapigetartiststoptracks
      x-api-path-slug: artistsidtoptracks-get
      parameters:
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: path
        name: id
        description: The Spotify ID for the artist
      responses:
        200:
          description: OK
      tags:
      - Music
      - Artists
      - Tracks
  /browse/categories:
    get:
      summary: Browse Categories
      description: '[Get a List of Browse Categories](https://developer.spotify.com/web-api/get-list-categories/)'
      operationId: get-a-list-of-browse-categorieshttpsdeveloperspotifycomwebapigetlistcategories
      x-api-path-slug: browsecategories-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: locale
        description: The desired language, consisting of an ISO 639 language code
          and an ISO 3166-1 alpha-2 country code, joined by an underscore
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - Categories
  /browse/categories/{category_id}:
    get:
      summary: Browse Category
      description: '[Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)'
      operationId: get-a-single-browse-categoryhttpsdeveloperspotifycomwebapigetcategory
      x-api-path-slug: browsecategoriescategory-id-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: path
        name: category_id
        description: The Spotify ID of the category you wish to fetch
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: locale
        description: The desired language, consisting of an ISO 639 language code
          and an ISO 3166-1 alpha-2 country code, joined by an underscore
      responses:
        200:
          description: OK
      tags:
      - Music
      - Categories
      - Playlists
  /browse/categories/{category_id}/playlists:
    get:
      summary: Browse Category Playlists
      description: '[Get a Category''s playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)'
      operationId: get-a-categorys-playlistshttpsdeveloperspotifycomwebapigetcategorysplaylists
      x-api-path-slug: browsecategoriescategory-idplaylists-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: path
        name: category_id
        description: The Spotify ID of the category you wish to fetch
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - Playlists
  /browse/featured-playlists:
    get:
      summary: Browse Featured Playlists
      description: '[Get a List of Featured Playlists](https://developer.spotify.com/web-api/get-list-featured-playlists/)'
      operationId: get-a-list-of-featured-playlistshttpsdeveloperspotifycomwebapigetlistfeaturedplaylists
      x-api-path-slug: browsefeaturedplaylists-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: locale
        description: The desired language, consisting of an ISO 639 language code
          and an ISO 3166-1 alpha-2 country code, joined by an underscore
      - in: query
        name: offset
        description: The index of the first item to return
      - in: query
        name: timestamp
        description: A timestamp in ISO 8601 format (yyyy-MM-ddTHH:mm:ss) with the
          users local time to get results tailored to a specific date and time in
          the day
      responses:
        200:
          description: OK
      tags:
      - Music
      - Playlists
  /browse/new-releases:
    get:
      summary: Browse New Releases
      description: '[Get a List of New Releases](https://developer.spotify.com/web-api/get-list-new-releases/)'
      operationId: get-a-list-of-new-releaseshttpsdeveloperspotifycomwebapigetlistnewreleases
      x-api-path-slug: browsenewreleases-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - New Releases
  /me:
    get:
      summary: Get Me
      description: '[Get Current User''s Profile](https://developer.spotify.com/web-api/get-current-users-profile/)'
      operationId: get-current-users-profilehttpsdeveloperspotifycomwebapigetcurrentusersprofile
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Music
      - Me
  /me/following:
    delete:
      summary: Delete Following
      description: '[Unfollow Artists or Users](https://developer.spotify.com/web-api/unfollow-artists-users/)'
      operationId: unfollow-artists-or-usershttpsdeveloperspotifycomwebapiunfollowartistsusers
      x-api-path-slug: mefollowing-delete
      parameters:
      - in: query
        name: ids
        description: A comma-separated list of the artists or users ids
      - in: query
        name: type
        description: The type to unfollow
      responses:
        200:
          description: OK
      tags:
      - Music
      - Me
      - Following
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---