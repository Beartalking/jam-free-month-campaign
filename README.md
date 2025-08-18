# JAM Campaign Website 🎯

A modern, neural brutalist campaign website for JAM's free one-month pro membership promotion.

## 🌟 Features

### Core Functionality
- **Two-Page Campaign Flow**: Form submission → Contract & redemption
- **Promo Code Management**: 200 initial codes with dynamic addition capability
- **User Data Capture**: Complete form data with CSV export functionality
- **Custom Hero Banners**: Upload and manage campaign visuals via admin panel

### Admin Panel Features
- **Password Protected**: Access via `?admin=true` or `Ctrl+Shift+A`
- **User Analytics**: View submission stats and export user data
- **Code Management**: Add single/bulk promo codes, export all codes
- **Visual Management**: Upload custom hero banners with auto-optimization
- **Data Export**: CSV downloads for users and promo codes

### Technical Highlights
- **Single File Architecture**: Complete website in one HTML file
- **Client-Side Storage**: localStorage for persistent data and settings
- **Image Processing**: Canvas API for banner optimization and compression
- **Responsive Design**: Mobile-first approach with neural brutalist styling
- **Form Validation**: Complete input validation with user feedback

## 🎨 Design

**Style**: Neural Brutalist with JAM brand colors
- **Primary**: #FFCC00 (Yellow)
- **Accent**: #0147FE (Blue), #FF3B30 (Red)
- **Typography**: Bold, modern system fonts
- **Layout**: Card-based with strong borders and shadows

## 🚀 Deployment

### Local Development
```bash
# Serve locally
python3 -m http.server 8000
# Visit: http://localhost:8000
```

### Production Deployment
- **Hosting**: Vercel (recommended)
- **Domain**: Custom domain support
- **SSL**: Automatic HTTPS
- **CDN**: Global content delivery

## 🔧 Admin Panel

**Access**: Add `?admin=true` to URL or press `Ctrl+Shift+A`
**Password**: `jam2025admin`

### Admin Features:
- 📊 **Dashboard**: User stats, code usage analytics
- 👥 **User Management**: Export user data to CSV
- 🎫 **Code Management**: Add/export promo codes
- 🖼️ **Visual Management**: Upload custom hero banners
- 🗑️ **Data Management**: Clear data, reset codes

## 📱 Campaign Features

### Form Fields
- Name, email, contact (phone/WeChat)
- Current & target English levels
- Daily practice commitment
- Personal motivation statement

### Redemption Experience
- Personalized contract with user data
- One-click App Store redemption
- QR codes for WeChat/WhatsApp groups
- Confetti celebration effects

## 🛠️ Technical Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Storage**: Browser localStorage
- **Image Processing**: Canvas API
- **Export**: Blob API for CSV generation
- **Styling**: Custom CSS with neural brutalist design

## 📦 File Structure

```
jam-campaign-site.html          # Complete website (1,500+ lines)
JAM - promo code管理 - Sheet2.csv  # Initial promo codes
README.md                       # This documentation
.gitignore                      # Git ignore rules
```

## 🔄 Version History

- **build-1**: Initial release with core campaign functionality
- **build-1.0.1**: Added custom hero banner upload feature
- **latest**: Removed watermark, improved image display

## 📄 License

All rights reserved - Jamtalk.co

## 🤝 Support

For technical support or questions about the campaign, contact the development team.

---

**Built with ❤️ for JAM - Your AI-powered English speaking coach**