<h1 align="center"> Remark SnackPlayer </h1>

Remark plugin to embed [Expo Snack's](https://snack.expo.io/) using Code Blocks

<hr>

<p align="center">

  <a href="https://dev-to-uploads.s3.amazonaws.com/i/2xg59r17v72yvqfb3wu5.jpg">
    <img src="https://forthebadge.com/images/badges/built-with-love.svg"
         alt="Javascript">
  </a>

  <a href="https://dev-to-uploads.s3.amazonaws.com/i/2xg59r17v72yvqfb3wu5.jpg">
    <img src="https://forthebadge.com/images/badges/made-with-javascript.svg"
         alt="Javascript">
  </a>
  
</p>

## Installing

`npm install remark-snackplayer`

or

`yarn add remark-snackplayer`

## Usage

This plugin parses codeblocks with language set as `SnackPlayer` and replaces them with embedded Expo's SnackPlayers, you can also provide parameters along with the codeblock to set some basic details.

Example Code Block:

````

```SnackPlayer name=Hello%20World description=This%20is%20a%20description
import React from 'react';
import { Text, View } from 'react-native';

const YourApp = () => {
    return (
    <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
        <Text>
        Try editing me! 🎉
        </Text>
    </View>
    );
}

export default YourApp;```


````

The above code snippet would look like this on your page

<img width="783" alt="Screenshot 2020-10-03 at 1 11 19 AM" src="https://user-images.githubusercontent.com/11258286/94963203-67de3500-0515-11eb-974a-a2289c0bfdc8.png">


Parameters:

| Name               | Description                | Default           |
| ------------------ | -------------------------- | ----------------- |
| name               | SnackPlayer Name           | "Example"         |
| description        | Description of the example | "Example usage"   |
| platform           | Example Platform           | "ios"             |
| supportedPlatforms | Supported Platforms        | "ios,android,web" |

## To Do

* Support Passing Configuration Parameters
* Fix and Document Mobile Fallback
* Write Comprehensive tests

## License

[MIT](./LICENSE) © Darsh Patel