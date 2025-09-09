# BlueHost Deployment Instructions

## Important Notes for BlueHost Hosting

This document contains essential information to ensure your website works correctly on BlueHost servers.

### Image Path Requirements

**CRITICAL:** BlueHost servers are case-sensitive and require specific path formatting.

#### ✅ Correct Image Paths (Already Fixed)
- Use `./images/` prefix for all local images
- Example: `<img src="./images/photo.jpg">`
- Example: `background-image: url('./images/background.jpg')`

#### ❌ Incorrect Paths (Will Cause Issues)
- Capital "Images" folder: `Images/photo.jpg`
- Missing relative path: `images/photo.jpg`
- Absolute paths without proper structure

### File Structure for BlueHost

```
website-root/
├── index.html
├── portfolio.html
├── images/           (lowercase 'i')
│   ├── about-img.jpg
│   ├── bbgg.png
│   ├── mbbg.jpg
│   ├── honda.png
│   ├── promotional.mp4
│   ├── promotional.webm
│   └── [all gallery images]
└── [other files]
```

### Deployment Checklist

1. **Before Upload:**
   - [ ] Verify all image paths use `./images/` format
   - [ ] Check that images folder is lowercase
   - [ ] Test locally to ensure images load

2. **During Upload:**
   - [ ] Upload all files to public_html directory
   - [ ] Maintain folder structure exactly as shown above
   - [ ] Ensure file permissions are set correctly (644 for files, 755 for directories)

3. **After Upload:**
   - [ ] Test website functionality
   - [ ] Verify all images display correctly
   - [ ] Check responsive design on mobile devices
   - [ ] Test video playback if applicable

### Common BlueHost Issues and Solutions

**Problem:** Images not displaying
**Solution:** Check that:
- Image paths use `./images/` format
- Images folder is lowercase
- File names match exactly (case-sensitive)

**Problem:** Website looks broken
**Solution:** 
- Clear browser cache
- Check file permissions on server
- Verify all CSS and JS files uploaded correctly

### File Permissions on BlueHost

- HTML files: 644
- Image files: 644
- Directories: 755
- CSS/JS files: 644

### Support

If you encounter issues:
1. Check this deployment guide first
2. Verify file paths and permissions
3. Contact BlueHost support if server-related issues persist

---

**Last Updated:** Created for BlueHost optimization
**Files Modified:** index.html, portfolio.html
**Status:** Ready for deployment