# JAM Campaign Website

A promotional campaign website for JAM - AI-powered English speaking coach app.

## 🎯 Overview

This campaign website allows users to:
- Fill out a form with their English learning goals
- Receive a free 1-month JAM Pro redemption code
- Join WeChat/WhatsApp user groups via QR codes

## 📁 Project Structure

```
├── jam-campaign-site.html          # Main campaign website
├── JAM - promo code管理 - Sheet2.csv  # Promo codes database
├── README.md                        # This file
└── .gitignore                      # Git ignore rules
```

## ✨ Features

### User Experience
- **Neural Brutalist Design** - Matches JAM app's visual style
- **Two-Page Flow** - Form submission → Success with redemption code
- **Mobile Responsive** - Works on all devices
- **Chinese Language** - Simplified Chinese interface
- **Animated Confetti** - Celebration effects on success page

### Admin Features
- **User Data Capture** - Automatic form submission tracking
- **CSV Export** - Download user data and promo code usage
- **Promo Code Management** - Add new codes via admin panel
- **Real-time Statistics** - Usage tracking and analytics

### Technical Features
- **200+ Promo Codes** - Pre-loaded redemption codes
- **Local Storage** - Browser-based data persistence
- **Automatic URL Generation** - App Store links for new codes
- **Data Validation** - Form and code format validation

## 🔧 Admin Access

### Methods to Access Admin Panel:
1. **URL Parameter**: `?admin=true`
2. **Keyboard Shortcut**: `Ctrl+Shift+A`
3. **Console Command**: `showAdminPanel()`

**Admin Password**: `jam2025admin`

### Admin Functions:
- 📊 Export user data to CSV
- ➕ Add single promo codes
- 📝 Bulk import promo codes  
- 📋 Export all promo codes
- 🗑️ Clear user data
- 🔄 Reset additional codes

## 🚀 Deployment

1. Upload `jam-campaign-site.html` to any web server
2. Ensure the CSV file is in the same directory (for reference)
3. Share the website URL with your audience

## 📊 Data Management

### User Data Captured:
- Name, Email, Contact info
- Current & Target English levels
- Daily practice commitment
- Personal motivation statement
- Assigned promo code & timestamp
- Browser metadata

### Export Formats:
- **User Data CSV**: Complete form submissions
- **Promo Codes CSV**: Usage tracking and status

## 🎨 Design System

### Colors:
- **Primary Blue**: #0147FE (JAM brand color)
- **Accent Yellow**: #FFCC00 (Highlights)
- **Success Green**: #61BA47 (Success states)
- **Error Red**: #FF3B30 (Error states)
- **Neutral Gray**: #5C5C5C (Text)

### Typography:
- **Font Family**: -apple-system, BlinkMacSystemFont, sans-serif
- **Weights**: 400 (regular), 600 (medium), 700 (bold), 900 (black)

## 🔄 Version History

- **Build 1** (2025-01-08): Initial release with full campaign functionality

## 📞 Support

For technical issues or questions:
- **Email**: bear@beartalking.com
- **Website**: Jamtalk.co

---

Built with ❤️ for JAM English Learning Community
