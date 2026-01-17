# Quick Video Setup Guide

## 🎬 How to Add Videos to Your Website

### ✅ **Option 1: YouTube (Recommended)**

**Step 1:** Upload your video to YouTube
- Go to YouTube.com
- Click "Create" → "Upload video"
- Upload your video file
- Set visibility to **"Unlisted"** (so only people with the link can see it)

**Step 2:** Get your Video ID
- After uploading, your video URL will look like: `https://www.youtube.com/watch?v=ABC123xyz`
- The **Video ID** is the part after `v=` → `ABC123xyz`

**Step 3:** Add to HTML
- Open `scrap-supplier-user-guide.html`
- Find the video section you want (e.g., "Account Activation")
- Look for the commented code that says `<!-- <iframe ...>`
- Uncomment it (remove `<!--` and `-->`)
- Replace `VIDEO_ID` with your actual video ID

**Example:**
```html
<!-- Before -->
<!--
<iframe 
    src="https://www.youtube.com/embed/VIDEO_ID" 
    ...
</iframe>
-->

<!-- After (with your video ID) -->
<iframe 
    src="https://www.youtube.com/embed/ABC123xyz" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>
```

**That's it!** Just replace `VIDEO_ID` in each section with your actual YouTube video ID.

---

### 📁 **Option 2: OneDrive**

**Important:** OneDrive doesn't work exactly like YouTube. You need to get an **embed link**, not just a share link.

**Step 1:** Upload to OneDrive
- Upload your video to a OneDrive folder
- Right-click the video → "Share" → "Embed"
- Copy the embed code provided

**Step 2:** Add to HTML
- Find the video section in the HTML
- Replace the entire iframe `src` with your OneDrive embed URL

**Example:**
```html
<iframe 
    src="YOUR_ONEDRIVE_EMBED_URL_HERE" 
    frameborder="0" 
    allowfullscreen>
</iframe>
```

**Note:** OneDrive embed links can be long and complex. Make sure you copy the full embed URL from OneDrive's "Embed" option.

---

## 📋 **Video Sections in Your Website**

You have **11 video sections** to fill:

1. ✅ Account Activation Walkthrough
2. ✅ Portal Overview
3. ✅ First Login Walkthrough
4. ✅ Password Reset and Change Process
5. ✅ Portal Navigation Walkthrough
6. ✅ Viewing Supplier Profile and Documents
7. ✅ Payments and Invoices Walkthrough
8. ✅ Creating and Managing Vehicles
9. ✅ Creating and Managing Employees
10. ✅ Offline Auction Subscription Flow
11. ✅ Central Resources and Documentation Overview

---

## 🚀 **Quick Steps Summary**

### For YouTube:
1. Upload video → Get Video ID
2. Open HTML file
3. Find video section
4. Uncomment the iframe code
5. Replace `VIDEO_ID` with your ID
6. Save and test!

### For OneDrive:
1. Upload video → Get Embed link
2. Open HTML file
3. Find video section
4. Uncomment the iframe code
5. Replace entire `src` URL with OneDrive embed URL
6. Save and test!

---

## 💡 **Tips**

- **Test each video** after adding it
- **Keep videos short** (2-5 minutes)
- **Use consistent naming** for your YouTube videos
- **Set YouTube videos to "Unlisted"** for privacy
- **Have a backup plan** - keep local copies of videos

---

## ❓ **Troubleshooting**

**Video not showing?**
- Check you uncommented the code (removed `<!--` and `-->`)
- Verify the Video ID is correct
- Make sure YouTube video is set to "Unlisted" or "Public"
- Check internet connection

**OneDrive not working?**
- Make sure you're using the **Embed** link, not the Share link
- Check the video permissions allow embedding
- Try the YouTube method instead (easier!)

---

**Good luck with your demo! 🎉**

