---
swagger: "2.0"
info:
  title: Spotify Get Artist
  description: '[Get an Artist](https://developer.spotify.com/web-api/get-artist/)'
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
  /artists/{id}:
    get:
      summary: Get Artist
      description: '[Get an Artist](https://developer'
      operationId: get-an-artisthttpsdeveloperspotifycomwebapigetartist
      parameters:
      - in: path
        name: id
        description: The Spotify ID for the artist
      responses:
        200:
          description: OK
      tags:
      - music
      - artists
definitions:
  album:
    properties:
      album_type:
        description: This is a default description.
        type: put
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      copyrights:
        description: This is a default description.
        type: put
      external_ids:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      genres:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
  album-simple:
    properties:
      album_type:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  album-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  album-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  artist:
    properties:
      external_urls:
        description: This is a default description.
        type: put
      genres:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      popularity:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  artist-simple:
    properties:
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  category:
    properties:
      href:
        description: This is a default description.
        type: put
      icons:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  category-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  current-user-profile:
    properties:
      birthdate:
        description: This is a default description.
        type: put
      country:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      email:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      product:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
  featured-playlists:
    properties:
      message:
        description: This is a default description.
        type: put
  followers:
    properties:
      href:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  image:
    properties:
      height:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
      width:
        description: This is a default description.
        type: put
  playlist:
    properties:
      collaborative:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      followers:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      public:
        description: This is a default description.
        type: put
      snapshot_id:
        description: This is a default description.
        type: put
  playlist-simple:
    properties:
      collaborative:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      images:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      public:
        description: This is a default description.
        type: put
      snapshot_id:
        description: This is a default description.
        type: put
      tracks:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  playlist-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  playlist-snapshot:
    properties:
      snapshot_id:
        description: This is a default description.
        type: put
  playlist-track:
    properties:
      added_at:
        description: This is a default description.
        type: put
      is_local:
        description: This is a default description.
        type: put
  playlist-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  saved-track:
    properties:
      added_at:
        description: This is a default description.
        type: put
  saved-track-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  search:
    properties:
      albums:
        description: This is a default description.
        type: put
      artists:
        description: This is a default description.
        type: put
      tracks:
        description: This is a default description.
        type: put
  track:
    properties:
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      disc_number:
        description: This is a default description.
        type: put
      duration_ms:
        description: This is a default description.
        type: put
      explicit:
        description: This is a default description.
        type: put
      external_ids:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      is_playable:
        description: This is a default description.
        type: put
  track-simple:
    properties:
      artists:
        description: This is a default description.
        type: put
      available_markets:
        description: This is a default description.
        type: put
      disc_number:
        description: This is a default description.
        type: put
      duration_ms:
        description: This is a default description.
        type: put
      explicit:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      is_playable:
        description: This is a default description.
        type: put
      linked_from:
        description: This is a default description.
        type: put
  track-simple-page:
    properties:
      href:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      limit:
        description: This is a default description.
        type: put
      next:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      previous:
        description: This is a default description.
        type: put
      total:
        description: This is a default description.
        type: put
  user-followed:
    properties:
      artists:
        description: This is a default description.
        type: put
  user-profile:
    properties:
      displayName:
        description: This is a default description.
        type: put
      external_urls:
        description: This is a default description.
        type: put
      href:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      uri:
        description: This is a default description.
        type: put
x-collection-name: Spotify
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