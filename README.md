# Expo Camera and useEffect Race Condition

This repository demonstrates a bug encountered while using Expo's Camera component in conjunction with the useEffect hook. The bug manifests as an app freeze or crash during image processing, without providing clear error messages.

## Bug Description

The problem arises from a race condition between asynchronous operations within useEffect and the availability of image data from the Camera component. Attempts to access or modify the image data before it's fully loaded can lead to unexpected behavior or app crashes.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `expo start`.
4. Try taking a picture and observe the application behavior. Note that the app freeze happens only when a specific image processing steps are used.