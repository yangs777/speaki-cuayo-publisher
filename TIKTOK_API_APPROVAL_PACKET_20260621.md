# TikTok Content Posting API Approval Packet

Date: 2026-06-21

## Official Route

Use TikTok for Developers, not the public problem-report form.

1. Log in at https://developers.tiktok.com/
2. Open or create the app for Speaki Cuayo Publisher.
3. Add the Content Posting API product.
4. Enable Direct Post configuration if available.
5. Request only the needed scopes:
   - user.info.basic
   - video.upload
   - video.publish
6. Submit the app for review/audit with the text below and a real demo video.

## App Name

Speaki Cuayo Publisher

## Website URL

https://yangs777.github.io/speaki-cuayo-publisher/

## Terms of Service

https://yangs777.github.io/speaki-cuayo-publisher/terms.html

## Privacy Policy

https://yangs777.github.io/speaki-cuayo-publisher/privacy.html

## Data Deletion Instructions

https://yangs777.github.io/speaki-cuayo-publisher/data-deletion.html

## OAuth Redirect URIs

Use the URI that matches the app flow:

https://yangs777.github.io/speaki-cuayo-publisher/auth/callback/

Optional desktop callback if the portal allows multiple redirect URIs:

https://yangs777.github.io/speaki-cuayo-publisher/auth/callback/desktop/

## App Description

Speaki Cuayo Publisher is a web-based publishing assistant for creators who prepare, review, and publish original short-form videos to connected social channels. Approved creators can connect their TikTok account through TikTok Login Kit, select a video they own or have permission to publish, review captions and posting settings, and upload or publish that content through the TikTok Content Posting API.

## Product and Scope Explanation

### Login Kit

Login Kit is used so a creator can securely connect a TikTok account through TikTok's official authorization flow. The app uses the returned authorization code to obtain tokens and identify the connected account. The app does not ask for TikTok passwords and does not bypass TikTok's login or security systems.

### user.info.basic

This scope is used only to confirm which TikTok account was connected and to display basic account identity in the publishing workflow, such as account identifier, display name, and profile image when available.

### Content Posting API

The Content Posting API is used to upload or publish creator-selected short-form videos. The creator chooses the video file, caption, hashtags, privacy level, comment setting, duet setting, stitch setting, commercial content disclosure, and posting confirmation before the upload or publishing request is sent. The app supports creator-controlled publishing and can use draft/manual review behavior when direct publishing is not appropriate.

### video.upload

This scope is used to upload creator-selected video files to the connected TikTok account as drafts or inbox uploads for manual creator review when direct publishing is not appropriate.

### video.publish

This scope is used when the creator explicitly requests direct publishing from the app. The app sends only content selected and reviewed by the creator, with the creator's chosen caption and posting settings.

## Reviewer Note

This revision provides a public website, Terms of Service, Privacy Policy, and Data Deletion Instructions that accurately describe the app as a creator publishing assistant. These pages are available without login and are linked directly from the public website.

The app is not a scraping tool, analytics harvester, engagement bot, spam tool, credential storage utility, or bulk auto-posting tool for third-party accounts. It is a creator-controlled publishing workflow for original short-form video content, using only the TikTok permissions needed for account identification and content posting.

The demo flow shows the creator connecting TikTok through OAuth, selecting a creator-owned rendered video, reviewing/editing caption and hashtags, choosing TikTok-provided privacy options, confirming comment/duet/stitch settings, reviewing commercial content disclosure, seeing a preview, and explicitly confirming before the upload or publish action.

## Demo Video Checklist

The demo video should show all of these, because community rejection reports point to missing UX requirements as the main failure reason:

- Public website with Terms, Privacy Policy, and Data Deletion links visible.
- TikTok OAuth connection flow.
- Connected TikTok creator identity displayed after `creator_info/query`.
- A real rendered video selected by the creator, not a mock placeholder.
- Caption and hashtag edit field.
- Privacy options loaded dynamically from TikTok creator info, with no hard-coded invalid default.
- Comment, Duet, and Stitch controls shown and disabled if TikTok creator info requires it.
- Commercial content disclosure controls, including Your Brand / Branded Content behavior.
- Explicit creator consent before sending content to TikTok.
- Preview/review screen before upload or direct publish.
- Upload/post status tracking after submit.

## Community Findings To Remember

- Developers who passed reported that a real product demo, OAuth flow, media selection, caption editing, privacy selection, manual confirmation, verified media domain, and TikTok-specific Terms/Privacy sections mattered.
- Rejections often cite missing Content Sharing UX requirements, not backend API errors.
- Direct Post public publishing requires audit. Before audit, content may be restricted to private/self-only behavior.
