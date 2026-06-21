# TikTok App Review Resubmission Text

Use this text when resubmitting the TikTok developer app.

## App Description

Speaki Cuayo Publisher is a web-based publishing assistant for creators who prepare, review, and publish original short-form videos to connected social channels. Approved creators can connect their TikTok account through TikTok Login Kit, select a video they own or have permission to publish, review captions and posting settings, and upload or publish that content through the TikTok Content Posting API.

## Website URL

https://yangs777.github.io/speaki-cuayo-publisher/

The website includes visible links to:

- Terms of Service: https://yangs777.github.io/speaki-cuayo-publisher/terms.html
- Privacy Policy: https://yangs777.github.io/speaki-cuayo-publisher/privacy.html
- Data Deletion Instructions: https://yangs777.github.io/speaki-cuayo-publisher/data-deletion.html

## Product and Scope Explanation

### Login Kit

Login Kit is used so a creator can securely connect a TikTok account through TikTok's official authorization flow. The app uses the returned authorization code to obtain tokens and identify the connected account. The app does not ask for TikTok passwords and does not bypass TikTok's login or security systems.

### user.info.basic

This scope is used only to confirm which TikTok account was connected and to display basic account identity in the publishing workflow, such as account identifier, display name, and profile image when available.

### Content Posting API

The Content Posting API is used to upload or publish creator-selected short-form videos. The creator chooses the video file, caption, hashtags, and posting settings before the upload or publishing request is sent. The app supports creator-controlled publishing and can use draft/manual review behavior when direct publishing is not appropriate.

### video.upload

This scope is used to upload creator-selected video files to the connected TikTok account as part of the publishing workflow.

### video.publish

This scope is used when the creator requests direct publishing from the app. The app sends only content selected and reviewed by the creator, with the creator's chosen caption and posting settings.

## Reviewer Note

This revision updates the public website, Terms of Service, Privacy Policy, and Data Deletion Instructions to accurately describe the app as a creator publishing assistant rather than a private or personal-use tool. The Terms and Privacy Policy are linked directly from the public website without requiring login or opening a menu.

The app is not a scraping tool, analytics harvester, engagement bot, spam tool, or private credential storage utility. It is a creator-controlled publishing workflow for original short-form video content, using only the TikTok permissions needed for account identification and content posting.
