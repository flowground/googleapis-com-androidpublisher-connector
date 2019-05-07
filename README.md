# ![LOGO](logo.png) Google Play Developer **flow**ground Connector

## Description

A generated **flow**ground connector for the Google Play Developer API (version v3).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/androidpublisher/v3/swagger.json<br/>
Generated at: 2019-05-07T17:41:11+03:00

## API Description

Accesses Android application developers' Google Play accounts.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Creates a new edit for an app, populated with the app's current state.

*Tags:* `edits`

#### Input Parameters
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes an edit for an app. Creating a new edit will automatically delete any of your previous edits so this method need only be called if you want to preemptively abandon an edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns information about the edit specified. Calls will fail if the edit is no long active (e.g. has been deleted, superseded or expired).

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_apks_list

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_apks_upload

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new APK without uploading the APK itself to Google Play, instead hosting the APK at a specified URL. This function is only available to enterprises using Google Play for Work whose application is configured to restrict distribution to the enterprise domain.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Uploads the deobfuscation file of the specified APK. If a deobfuscation file already exists, it will be replaced.

*Tags:* `edits`

#### Input Parameters
* `apkVersionCode` - _required_ - The version code of the APK whose deobfuscation file is being uploaded.
* `deobfuscationFileType` - _required_
    Possible values: proguard.
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier of the Android app for which the deobfuscatiuon files are being uploaded; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Fetches the Expansion File configuration for the APK specified.

*Tags:* `edits`

#### Input Parameters
* `apkVersionCode` - _required_ - The version code of the APK whose Expansion File configuration is being read or modified.
* `editId` - _required_ - Unique identifier for this edit.
* `expansionFileType` - _required_
    Possible values: main, patch.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the APK's Expansion File configuration to reference another APK's Expansion Files. To add a new Expansion File use the Upload method. This method supports patch semantics.

*Tags:* `edits`

#### Input Parameters
* `apkVersionCode` - _required_ - The version code of the APK whose Expansion File configuration is being read or modified.
* `editId` - _required_ - Unique identifier for this edit.
* `expansionFileType` - _required_
    Possible values: main, patch.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Uploads and attaches a new Expansion File to the APK specified.

*Tags:* `edits`

#### Input Parameters
* `apkVersionCode` - _required_ - The version code of the APK whose Expansion File configuration is being read or modified.
* `editId` - _required_ - Unique identifier for this edit.
* `expansionFileType` - _required_
    Possible values: main, patch.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the APK's Expansion File configuration to reference another APK's Expansion Files. To add a new Expansion File use the Upload method.

*Tags:* `edits`

#### Input Parameters
* `apkVersionCode` - _required_ - The version code of the APK whose Expansion File configuration is being read or modified.
* `editId` - _required_ - Unique identifier for this edit.
* `expansionFileType` - _required_
    Possible values: main, patch.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_bundles_list

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Uploads a new Android App Bundle to this edit. If you are using the Google API client libraries, please increase the timeout of the http request before calling this endpoint (a timeout of 2 minutes is recommended). See: https://developers.google.com/api-client-library/java/google-api-java-client/errors for an example in java.

*Tags:* `edits`

#### Input Parameters
* `ackBundleInstallationWarning` - _optional_ - Must be set to true if the bundle installation may trigger a warning on user devices (for example, if installation size may be over a threshold, typically 100 MB).
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Fetches app details for this edit. This includes the default language and developer support contact information.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates app details for this edit. This method supports patch semantics.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates app details for this edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes all localized listings from an edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns all of the localized store listings attached to this edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified localized store listing from an edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing to read or modify. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Fetches information about a localized store listing.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing to read or modify. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates or updates a localized store listing. This method supports patch semantics.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing to read or modify. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates or updates a localized store listing.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing to read or modify. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes all images for the specified language and image type.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `imageType` - _required_
    Possible values: featureGraphic, icon, phoneScreenshots, promoGraphic, sevenInchScreenshots, tenInchScreenshots, tvBanner, tvScreenshots, wearScreenshots.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing whose images are to read or modified. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all images for the specified language and image type.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `imageType` - _required_
    Possible values: featureGraphic, icon, phoneScreenshots, promoGraphic, sevenInchScreenshots, tenInchScreenshots, tvBanner, tvScreenshots, wearScreenshots.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing whose images are to read or modified. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Uploads a new image and adds it to the list of images for the specified language and image type.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `imageType` - _required_
    Possible values: featureGraphic, icon, phoneScreenshots, promoGraphic, sevenInchScreenshots, tenInchScreenshots, tvBanner, tvScreenshots, wearScreenshots.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing whose images are to read or modified. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the image (specified by id) from the edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `imageId` - _required_ - Unique identifier an image within the set of images attached to this edit.
* `imageType` - _required_
    Possible values: featureGraphic, icon, phoneScreenshots, promoGraphic, sevenInchScreenshots, tenInchScreenshots, tvBanner, tvScreenshots, wearScreenshots.
* `language` - _required_ - The language code (a BCP-47 language tag) of the localized listing whose images are to read or modified. For example, to select Austrian German, pass "de-AT".
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_testers_get

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify. Acceptable values are: "alpha", "beta", "production", "rollout" or "internal".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_testers_patch

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify. Acceptable values are: "alpha", "beta", "production", "rollout" or "internal".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### androidpublisher_edits_testers_update

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify. Acceptable values are: "alpha", "beta", "production", "rollout" or "internal".
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all the track configurations for this edit.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Fetches the track configuration for the specified track type. Includes the APK version codes that are in this track.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the track configuration for the specified track type. When halted, the rollout track cannot be updated without adding new APKs, and adding new APKs will cause it to resume. This method supports patch semantics.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the track configuration for the specified track type. When halted, the rollout track cannot be updated without adding new APKs, and adding new APKs will cause it to resume.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `track` - _required_ - The track to read or modify.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Commits/applies the changes made in this edit back to the app.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Checks that the edit can be successfully committed. The edit's changes are not applied to the live app.

*Tags:* `edits`

#### Input Parameters
* `editId` - _required_ - Unique identifier for this edit.
* `packageName` - _required_ - Unique identifier for the Android app that is being updated; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### List all the in-app products for an Android app, both subscriptions and managed in-app products..

*Tags:* `inappproducts`

#### Input Parameters
* `maxResults` - _optional_
* `packageName` - _required_ - Unique identifier for the Android app with in-app products; for example, "com.spiffygame".
* `startIndex` - _optional_
* `token` - _optional_
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new in-app product for an app.

*Tags:* `inappproducts`

#### Input Parameters
* `autoConvertMissingPrices` - _optional_ - If true the prices for all regions targeted by the parent app that don't have a price specified for this in-app product will be auto converted to the target currency based on the default price. Defaults to false.
* `packageName` - _required_ - Unique identifier for the Android app; for example, "com.spiffygame".
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Delete an in-app product for an app.

*Tags:* `inappproducts`

#### Input Parameters
* `packageName` - _required_ - Unique identifier for the Android app with the in-app product; for example, "com.spiffygame".
* `sku` - _required_ - Unique identifier for the in-app product.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns information about the in-app product specified.

*Tags:* `inappproducts`

#### Input Parameters
* `packageName` - _required_
* `sku` - _required_ - Unique identifier for the in-app product.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the details of an in-app product. This method supports patch semantics.

*Tags:* `inappproducts`

#### Input Parameters
* `autoConvertMissingPrices` - _optional_ - If true the prices for all regions targeted by the parent app that don't have a price specified for this in-app product will be auto converted to the target currency based on the default price. Defaults to false.
* `packageName` - _required_ - Unique identifier for the Android app with the in-app product; for example, "com.spiffygame".
* `sku` - _required_ - Unique identifier for the in-app product.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the details of an in-app product.

*Tags:* `inappproducts`

#### Input Parameters
* `autoConvertMissingPrices` - _optional_ - If true the prices for all regions targeted by the parent app that don't have a price specified for this in-app product will be auto converted to the target currency based on the default price. Defaults to false.
* `packageName` - _required_ - Unique identifier for the Android app with the in-app product; for example, "com.spiffygame".
* `sku` - _required_ - Unique identifier for the in-app product.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Refund a user's subscription or in-app purchase order.

*Tags:* `orders`

#### Input Parameters
* `orderId` - _required_ - The order ID provided to the user when the subscription or in-app order was purchased.
* `packageName` - _required_ - The package name of the application for which this subscription or in-app item was purchased (for example, 'com.some.thing').
* `revoke` - _optional_ - Whether to revoke the purchased item. If set to true, access to the subscription or in-app item will be terminated immediately. If the item is a recurring subscription, all future payments will also be terminated. Consumed in-app items need to be handled by developer's app. (optional)
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Checks the purchase and consumption status of an inapp item.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application the inapp product was sold in (for example, 'com.some.thing').
* `productId` - _required_ - The inapp product SKU (for example, 'com.some.thing.inapp1').
* `token` - _required_ - The token provided to the user's device when the inapp product was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Checks whether a user's subscription purchase is valid and returns its expiry time.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application for which this subscription was purchased (for example, 'com.some.thing').
* `subscriptionId` - _required_ - The purchased subscription ID (for example, 'monthly001').
* `token` - _required_ - The token provided to the user's device when the subscription was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Cancels a user's subscription purchase. The subscription remains valid until its expiration time.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application for which this subscription was purchased (for example, 'com.some.thing').
* `subscriptionId` - _required_ - The purchased subscription ID (for example, 'monthly001').
* `token` - _required_ - The token provided to the user's device when the subscription was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Defers a user's subscription purchase until a specified future expiration time.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application for which this subscription was purchased (for example, 'com.some.thing').
* `subscriptionId` - _required_ - The purchased subscription ID (for example, 'monthly001').
* `token` - _required_ - The token provided to the user's device when the subscription was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Refunds a user's subscription purchase, but the subscription remains valid until its expiration time and it will continue to recur.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application for which this subscription was purchased (for example, 'com.some.thing').
* `subscriptionId` - _required_ - The purchased subscription ID (for example, 'monthly001').
* `token` - _required_ - The token provided to the user's device when the subscription was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Refunds and immediately revokes a user's subscription purchase. Access to the subscription will be terminated immediately and it will stop recurring.

*Tags:* `purchases`

#### Input Parameters
* `packageName` - _required_ - The package name of the application for which this subscription was purchased (for example, 'com.some.thing').
* `subscriptionId` - _required_ - The purchased subscription ID (for example, 'monthly001').
* `token` - _required_ - The token provided to the user's device when the subscription was purchased.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the purchases that were canceled, refunded or charged-back.

*Tags:* `purchases`

#### Input Parameters
* `endTime` - _optional_ - The time, in milliseconds since the Epoch, of the newest voided in-app product purchase that you want to see in the response. The value of this parameter cannot be greater than the current time and is ignored if a pagination token is set. Default value is current time. Note: This filter is applied on the time at which the record is seen as voided by our systems and not the actual voided time returned in the response.
* `maxResults` - _optional_
* `packageName` - _required_ - The package name of the application for which voided purchases need to be returned (for example, 'com.some.thing').
* `startIndex` - _optional_
* `startTime` - _optional_ - The time, in milliseconds since the Epoch, of the oldest voided in-app product purchase that you want to see in the response. The value of this parameter cannot be older than 30 days and is ignored if a pagination token is set. Default value is current time minus 30 days. Note: This filter is applied on the time at which the record is seen as voided by our systems and not the actual voided time returned in the response.
* `token` - _optional_
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns a list of reviews. Only reviews from last week will be returned.

*Tags:* `reviews`

#### Input Parameters
* `maxResults` - _optional_
* `packageName` - _required_ - Unique identifier for the Android app for which we want reviews; for example, "com.spiffygame".
* `startIndex` - _optional_
* `token` - _optional_
* `translationLanguage` - _optional_
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Returns a single review.

*Tags:* `reviews`

#### Input Parameters
* `packageName` - _required_ - Unique identifier for the Android app for which we want reviews; for example, "com.spiffygame".
* `reviewId` - _required_
* `translationLanguage` - _optional_
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Reply to a single review, or update an existing reply.

*Tags:* `reviews`

#### Input Parameters
* `packageName` - _required_ - Unique identifier for the Android app for which we want reviews; for example, "com.spiffygame".
* `reviewId` - _required_
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-androidpublisher-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
