# REDLINE iOS build

This repository is configured to compile the **REDLINE iOS game** with GitHub Actions.

## Upload the project archive

Upload the file named **`REDLINE-GitHub-Upload.zip`** to the root of the repository using **Add file → Upload files**. Do not rename the archive or unzip it.

The upload automatically starts the **Build REDLINE IPA** workflow, which will unzip the complete project, run JavaScript tests, build the iOS app on a GitHub-hosted macOS runner, and upload the unsigned iPhone IPA and Simulator app as workflow artifacts.

Go to **Actions → Build REDLINE IPA** to see progress. Open a successful run and download **Redline-unsigned-IPA** under Artifacts.

The IPA is **unsigned**. A suitable Apple certificate/provisioning profile is required to install it on a real iPhone. Game Center multiplayer requires proper app registration and entitlements.

**Note:** the repository is currently public, so uploading the project archive makes its code publicly accessible.