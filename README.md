# Build v2rayNG Android App

This repository provides GitHub Actions workflows to automate the build process of the v2rayNG Android app. You can use this setup to build the app with your own signing keys and credentials.

## Prerequisites

Before you can build the v2rayNG Android app, You need to add the following **GitHub Secrets** to your repository:
 - `SIGNING_KEY`: Your signing key (Keystore) in base64-encoded format.
 - `SIGNING_KEY_ALIAS`: The alias for your signing key.
 - `SIGNING_KEY_PASSWORD`: The password for your signing key.
 - `SIGNING_STORE_PASSWORD`: The store password for your signing key.

## Building the App

To build the v2rayNG Android app, follow these steps:

1. Fork this repository to your own GitHub account.

2. Go to the "Settings" tab of your repository, and then click on "Secrets."

3. Add the required secrets mentioned above with your signing key information.

4. To trigger the GitHub Actions workflow manually, navigate to the "Actions" tab, select the workflow you want to run, and click the "Run workflow" button. This will initiate the build process.
Additionally, please make sure to provide the input data for XRAY_CORE_VERSION and V2RAYNG_VERSION when running the workflow.
   - `XRAY_CORE_VERSION`: The version of XRay Core to use for the build e.g `v1.8.4`.
   - `V2RAYNG_VERSION`: The version of v2rayNG (you can pass anything you want , it's not important).
5. Once the workflow completes, the built app will be uploaded to the GitHub Releases section of your repository. You can find it there and download the APK for installation on your Android device.

## Contributing

If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request. Your contributions are welcome!

For more information about the v2rayNG Android app, visit the [original repository](https://github.com/2dust/v2rayNG).

Happy building!

<a href="https://nowpayments.io/donation?api_key=MG750CX-D7AMMH9-QWARQ7V-9ZKH9XQ&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>