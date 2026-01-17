# Video Integration Guide for Supplier Portal User Guide

## 📹 Video Embedding Recommendations

This guide explains the best ways to add your recorded videos to the website.

---

## 🎯 **Recommended Options (Ranked)**

### **Option 1: YouTube Embedding** ⭐ **BEST FOR DEMOS**
**Pros:**
- ✅ Free and easy to use
- ✅ Automatic video optimization
- ✅ Works on all devices
- ✅ Easy to update/replace videos
- ✅ Analytics available
- ✅ No server storage needed
- ✅ Professional appearance

**Cons:**
- ❌ Requires YouTube account (can be unlisted/private)
- ❌ Internet connection required

**How to Use:**
1. Upload your video to YouTube (set as "Unlisted" for privacy)
2. Copy the video ID from the URL (e.g., `youtube.com/watch?v=ABC123xyz`)
3. Replace `VIDEO_ID` in the HTML with your actual video ID
4. Uncomment the YouTube iframe code in the HTML

**Example:**
```html
<iframe 
    src="https://www.youtube.com/embed/ABC123xyz" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>
```

---

### **Option 2: Local Video Files** ⭐ **BEST FOR OFFLINE/INTERNAL USE**
**Pros:**
- ✅ Works offline
- ✅ Full control over videos
- ✅ No external dependencies
- ✅ Good for internal demos

**Cons:**
- ❌ Large file sizes
- ❌ Requires server storage
- ❌ Slower loading
- ❌ Need to optimize videos manually

**How to Use:**
1. Create a `videos` folder in the same directory as your HTML file
2. Place your video files in the folder (recommended: MP4 format)
3. Optimize videos (keep under 50MB per video for web)
4. Uncomment the `<video>` tag in the HTML
5. Update the `src` path to match your video filename

**Example Folder Structure:**
```
project-folder/
├── scrap-supplier-user-guide.html
└── videos/
    ├── activation-process.mp4
    ├── first-login.mp4
    ├── password-reset.mp4
    └── ...
```

**Example HTML:**
```html
<video controls poster="videos/activation-thumbnail.jpg">
    <source src="videos/activation-process.mp4" type="video/mp4">
    <source src="videos/activation-process.webm" type="video/webm">
    Your browser does not support the video tag.
</video>
```

**Video Optimization Tips:**
- **Format:** MP4 (H.264 codec) - most compatible
- **Resolution:** 1280x720 (720p) or 1920x1080 (1080p)
- **File Size:** Keep under 50MB per video
- **Duration:** Keep videos concise (2-5 minutes ideal)
- **Tools:** Use HandBrake, FFmpeg, or online compressors

---

### **Option 3: Vimeo Embedding**
**Pros:**
- ✅ Professional appearance
- ✅ Good privacy controls
- ✅ No ads
- ✅ High quality

**Cons:**
- ❌ Free plan has limitations
- ❌ Requires Vimeo account

**How to Use:**
1. Upload to Vimeo
2. Get embed code from video settings
3. Use the iframe code provided

---

### **Option 4: Cloud Video Hosting (AWS S3, Cloudflare, etc.)**
**Pros:**
- ✅ Professional solution
- ✅ Scalable
- ✅ Good performance

**Cons:**
- ❌ Requires setup
- ❌ May have costs
- ❌ More technical

---

## 📋 **Quick Setup Checklist**

### For YouTube (Recommended):
- [ ] Create YouTube account (or use existing)
- [ ] Upload videos to YouTube (set as "Unlisted")
- [ ] Get video IDs from YouTube URLs
- [ ] Replace `VIDEO_ID` in HTML for each video
- [ ] Test all videos load correctly

### For Local Files:
- [ ] Create `videos` folder
- [ ] Optimize all video files (MP4, under 50MB)
- [ ] Place videos in folder
- [ ] Update HTML with correct file paths
- [ ] Test videos play correctly
- [ ] Ensure videos folder is included when sharing

---

## 🎬 **Video Naming Convention**

Suggested naming for consistency:
- `activation-process.mp4`
- `first-login.mp4`
- `password-reset.mp4`
- `portal-navigation.mp4`
- `profile-documents.mp4`
- `payments-invoices.mp4`
- `vehicles-management.mp4`
- `employees-management.mp4`
- `offline-auctions.mp4`
- `resources-overview.mp4`

---

## 💡 **Best Practices**

1. **Video Quality:**
   - Record in 720p or 1080p
   - Use clear audio
   - Good lighting and screen clarity

2. **Video Length:**
   - Keep each video focused (2-5 minutes)
   - One topic per video
   - Clear, concise narration

3. **File Management:**
   - Use consistent naming
   - Keep backups of original videos
   - Document which video goes where

4. **Testing:**
   - Test on different browsers
   - Test on mobile devices
   - Check video loading speed
   - Verify all videos work before demo

---

## 🔧 **Troubleshooting**

**Video won't play:**
- Check file path is correct
- Verify video format (MP4 recommended)
- Check browser compatibility
- Ensure file size isn't too large

**Video loads slowly:**
- Compress video file
- Use lower resolution
- Consider YouTube hosting instead

**YouTube video not showing:**
- Verify video ID is correct
- Check video is not private (use Unlisted)
- Ensure internet connection

---

## 📝 **Current Video Sections in HTML**

The website has video placeholders for:
1. Account Activation Walkthrough
2. Portal Overview
3. First Login Walkthrough
4. Password Reset and Change Process
5. Portal Navigation Walkthrough
6. Viewing Supplier Profile and Documents
7. Payments and Invoices Walkthrough
8. Creating and Managing Vehicles
9. Creating and Managing Employees
10. Offline Auction Subscription Flow
11. Central Resources and Documentation Overview

---

## ✅ **My Recommendation**

**For your demo with the Supplier persona, I recommend:**

1. **Use YouTube (Unlisted videos)** - Easiest to manage, professional, and works reliably
2. **Keep videos short and focused** - 2-4 minutes per topic
3. **Test before the demo** - Make sure all videos load quickly
4. **Have a backup plan** - Keep local copies just in case

This approach gives you:
- ✅ Easy updates if you need to change videos
- ✅ Professional appearance
- ✅ Reliable playback
- ✅ Works on any device
- ✅ No file size concerns

---

## 🚀 **Quick Start**

1. Record your videos
2. Upload to YouTube (Unlisted)
3. Copy video IDs
4. Open `scrap-supplier-user-guide.html`
5. Find each video section
6. Uncomment the YouTube iframe code
7. Replace `VIDEO_ID` with your actual video ID
8. Save and test!

Good luck with your demo! 🎉

