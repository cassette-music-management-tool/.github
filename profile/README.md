# 🎵 Cassette MVP — User Stories & Requirements

This document describes the initial MVP scope for Cassette, a web application for musicians to manage their releases.

---

## 🎯 Overview

Cassette will allow musicians to:
- Upload and organize audio, artwork, and promo assets
- Track release metadata
- Store notes and references
- Manage vertical videos for social media
- Authenticate via Google or Apple
- Subscribe to a Pro plan via Stripe

---

## 🟢 1. Authentication

**User Story**

> As a musician, I want to sign in securely with my Google or Apple account, so I can access my releases without managing passwords.

**Capabilities**
- Sign in with Google
- Sign in with Apple
- Show loading state during login
- Display logged-in user email or avatar
- Sign out option

---

## 🟢 2. Dashboard / Home Screen

**User Story**

> As a musician, I want to see a list of all my releases, so I can quickly access and manage them.

**Capabilities**
- List all releases with:
  - Name
  - Release date
  - Basic progress indicator or status
- Button to create new release
- Click to open release details
- Show Free / Pro status badge

---

## 🟢 3. Create Release

**User Story**

> As a musician, I want to create a new release project, so I can start uploading materials and tracking progress.

**Capabilities**
- Form fields:
  - Release Name (required)
  - Release Date (optional)
  - Multilink URL (optional)
  - Notes (optional)
- Create Release button
- On success:
  - Create Google Drive folder
  - Show confirmation

---

## 🟢 4. Manage Audio Files

**User Story**

> As a musician, I want to upload and organize different versions of my audio files, so I can track progress from demo to final master.

**Capabilities**
- Section: Audio Files
- Upload New File button
- Required label for each file (Demo, Intermediate Mix, Final Mix)
- Optional notes per file
- List of files:
  - File name
  - Label
  - Uploaded date
  - Download link
- (Optional) Audio preview

---

## 🟢 5. Manage Artwork

**User Story**

> As a musician, I want to upload artwork file and have it available in different sizes, so I have them ready for all platforms.

**Capabilities**
- Section: Artwork
- Upload Artwork button
- List of files:
  - File name
  - Label
  - Uploaded date
  - Download link
  - Download medium sized\small sized
---

## 🟢 6. Manage Promo Materials

**User Story**

> As a musician, I want to upload promo assets, so I can easily share them with services like Musosoup.

**Capabilities**
- Section: Promo Materials
- Upload File button
- Label or notes per file
- List of files with download links

---

## 🟢 7. Manage Vertical Video Assets

**User Story**

> As a musician, I want to upload vertical videos for reels and TikToks, so I can track which videos are ready to post.

**Capabilities**
- Section: Vertical Videos
- Upload Video button
- Metadata fields:
  - Label (e.g., Teaser Clip)
  - Notes
  - (Optional) Checkbox: Final Reel
- List of videos:
  - File name
  - Label
  - Uploaded date
  - Download link

---

## 🟢 8. Notes & References

**User Story**

> As a musician, I want to add notes and reference links about each release, so I don’t lose important ideas.

**Capabilities**
- Section: Notes
- Rich text field
- Save button
- Display saved notes
- Links clickable

---

## 🟢 9. Subscription / Payment Management

**User Story**

> As a musician, I want to upgrade to a Pro plan, so I can create more releases and unlock advanced features.

**Capabilities**
- Display current plan status (Free / Pro)
- Upgrade to Pro button (Stripe Checkout)
- After payment, update subscription status in UI
- (Optional) Link to Stripe customer portal for managing subscription

---

## 🟢 10. Access Control & Security

**User Story**

> As a musician, I want to be sure my data is secure and only accessible to me.

**Capabilities**
- All API requests require valid Firebase token
- Only show releases belonging to authenticated user
- Logout clears session

---

## 🟢 11. Notifications (Optional MVP)

**User Story**

> As a musician, I want to get an email notification when a collaborator uploads new files.

**Capabilities**
- Basic email sent when new audio or artwork files are uploaded
- Toggle notifications on/off
- *This feature can be deferred if needed*

---

## ✨ MVP Feature Summary

**Core Features**
- Authentication (Google/Apple)
- Dashboard listing releases
- Create release
- Upload/manage:
  - Audio files
  - Artwork
  - Promo materials
  - Vertical videos
- Metadata fields
- Notes & references
- Subscription upgrade flow (Stripe)
- Basic access control

**Optional Features**
- Email notifications
- Audio previews

---

