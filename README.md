# Note: This has been moved to [facebook/react-native-website](https://github.com/facebook/react-native-website/tree/master/plugins/remark-snackplayer)
## This plugin was a part of efforts for migrating the React Native's website to Docusaurus v2

<h1 align="center"> Remark SnackPlayer </h1>

<p align="center"> 
Remark plugin to embed <a href="https://snack.expo.io/">Expo Snack's</a> using Code Blocks 
</p>

<p align="center">

  <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/darshkpatel/remark-snackplayer/Test,%20Publish,%20&%20Release?style=for-the-badge">
  
<img alt="npm bundle size" src="https://img.shields.io/bundlephobia/min/remark-snackplayer?style=for-the-badge">

<img alt="Libraries.io dependency status for latest release" src="https://img.shields.io/librariesio/release/npm/remark-snackplayer?style=for-the-badge">

<img alt="npm" src="https://img.shields.io/npm/v/remark-snackplayer?style=for-the-badge">

</p>

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

- Support Passing Configuration Parameters
- Write Comprehensive tests

## License

[MIT](./LICENSE) © Darsh Patel
