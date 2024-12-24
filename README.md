# @byldd/expo

The `@byldd/expo` package is a versatile wrapper for commonly used packages created by BYLDD developers. It simplifies integrating features like authentication, reusable components, and more into your React Native apps built with Expo.

## Features

- Simplified integration of common functionalities like authentication and reusable components.
- Built-in support for Expo.
- Leverages the latest Firebase and other dependencies.
- Modular design to extend functionalities easily.

## Installation

To install the package, run the following command:

```bash
npm install @byldd/expo
```

### Peer Dependencies

Ensure the following dependencies are installed in your project:

```bash
npm install @react-native-firebase/app @react-native-firebase/auth @react-native-google-signin/google-signin expo-build-properties
```

## Configuration

Follow these steps to configure the packages in your project:

### 1. Firebase Setup and Google Sign In
 For Firebase Setup and Google Sign In, please visit the [Google Sign-In Guide](https://github.com/byldd/expo-google-signin#readme).

### Additional Functionalities

The `@byldd/expo` package includes various modules to streamline development:

1. **Authentication**: Simplifies Firebase and other authentication methods.
2. **Components**: Provides reusable UI components to speed up development.
3. **Utilities**: Includes helper functions to handle common tasks.


## Dependencies

- `@react-native-firebase/app` `^21.6.1`
- `@react-native-firebase/auth` `^21.6.1`
- `@react-native-google-signin/google-signin` `^13.1.0`
- `expo-build-properties` `~0.13.1`
## Usage

Here’s an example of how to use `@byldd/expo` for authentication services:

### Google Sign-In

```javascript
import { GoogleSigninService } from '@byldd/expo';

const handleGoogleSignIn = async (webClientID:string) => {
  try {
    const data = await GoogleSigninService.googleSignIn(webClientID);
    console.log('Google Sign-In Success:', data);
  } catch (error) {
    console.error('Google Sign-In Error:', error);
  }
};
```

### Facebook Sign-In

```javascript
import { FacebookSigninService } from '@byldd/expo';

const handleFacebookSignIn = async () => {
  try {
    const data = await FacebookSigninService.facebookSignIn();
    console.log('Facebook Sign-In Success:', data);
  } catch (error) {
    console.error('Facebook Sign-In Error:', error);
  }
};
```
## Contributing

Contributions are welcome! If you have suggestions or encounter issues, please open a pull request or issue in the GitHub repository.

## License

This package is licensed under the MIT License.

# expo
