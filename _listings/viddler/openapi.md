---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 1
info:
  title: Viddler  API
  description: the-viddler-api-exposes-viddleru2019s-key-features-to-those-that-would-like-to-build-custom-solutions-on-top-of-viddleru2019s-video-platform-
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.users.getPlayerBranding:
    get:
      summary: Users GetPlayerBranding
      description: Returns your player branding configuration.
      operationId: users-getplayerbranding
      x-api-path-slug: viddler-users-getplayerbranding-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetPlayerBranding
  viddler.users.getProfile:
    get:
      summary: Users GetProfile
      description: Get the public information for a profile. Can only get profile
        information for public profiles.
      operationId: users-getprofile
      x-api-path-slug: viddler-users-getprofile-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: user
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetProfile
  viddler.users.getSettings:
    get:
      summary: Users GetSettings
      description: Return account settings.
      operationId: users-getsettings
      x-api-path-slug: viddler-users-getsettings-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetSettings
  viddler.users.setPlayerBranding:
    post:
      summary: Users SetPlayerBranding
      description: 'Sets your player branding options. All options are optional other
        than your sessionid. Color formats are inu00a0hexadecimalu00a0format with
        preceding pound sign (IE: #rrggbb)'
      operationId: users-setplayerbranding
      x-api-path-slug: viddler-users-setplayerbranding-post
      parameters:
      - in: query
        name: bclicked
      - in: query
        name: bhover
      - in: query
        name: bidle
      - in: query
        name: control_bar
      - in: query
        name: enable_stripes
      - in: query
        name: logo_align
      - in: query
        name: logo_click_url
      - in: query
        name: logo_offset_x
      - in: query
        name: logo_offset_y
      - in: query
        name: logo_url
      - in: query
        name: logo_visible
      - in: query
        name: pclicked
      - in: query
        name: phover
      - in: query
        name: pidle
      - in: query
        name: sessionid
      - in: query
        name: shade_dark
      - in: query
        name: simple_color
      - in: query
        name: timebackground
      - in: query
        name: timeloaded
      - in: query
        name: timeplayed
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - SetPlayerBranding
  viddler.users.setProfile:
    get:
      summary: Users SetProfile
      description: Update your profile information.
      operationId: users-setprofile
      x-api-path-slug: viddler-users-setprofile-get
      parameters:
      - in: query
        name: avatar_url
      - in: query
        name: homepage
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - SetProfile
---