# Demo for MapBox

## How to build

In order build the project succesfully we need 2 tokens from mapbox.com

### Secret token
- Secret token will be used for downloading the library at compile time.
- Get a private token from [mapbox.com/access-tokens](https://account.mapbox.com/access-tokens). Secret tokens start with `sk`.
- Create a file in `$HOME/.gradle/gradle.properties`, if it exists then just open it. The add your token as below.
  
  ```properties
  MAPBOX_DOWNLOADS_TOKEN=YOUR_SECRET_TOKEN_HERE
  ```

### Public token
- Public token will be used everytime a request is sent to mapbox servers.
- Get your public default token from [mapbox.com/access-tokens](https://account.mapbox.com/access-tokens). Public tokens start with `pk`.
- Create a file in `app/src/main/res/values/developer_config.xml` and paste the token there. In this project, below file is ignored by git.
  
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
  <resources>
    <string name="mapbox_access_token">YOUR_PUBLIC_TOKEN_HERE</string>
  </resources>
  ```
