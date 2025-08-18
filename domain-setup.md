# 🌐 JAM Campaign Website Domain Setup Guide

## 📋 **Current Status**
- ✅ Website deployed on Vercel
- ✅ Cloudflare DNS management active
- ✅ Domain: `jamtalk.co` ready for configuration
- 🎯 **Using Subdomain**: `free.jamtalk.co` (recommended approach)

## 🚀 **Vercel Domain Configuration**

### **Step 1: Add Custom Domain in Vercel**
1. Go to your Vercel dashboard: https://vercel.com/dashboard
2. Select your `jam-free-month-campaign` project
3. Go to **Settings** → **Domains**
4. Click **Add Domain**
5. Enter: `free.jamtalk.co`
6. Click **Add**

### **Step 2: Vercel DNS Configuration**
Vercel will provide you with these DNS records to add to Cloudflare:

```
Type: A
Name: free
Value: 76.76.19.76
TTL: Auto
Proxy: DNS only (gray cloud)

Type: A
Name: free
Value: 76.76.21.76
TTL: Auto
Proxy: DNS only (gray cloud)
```

## ☁️ **Cloudflare DNS Configuration**

### **Step 3: Update Cloudflare DNS Records**
1. Go to Cloudflare dashboard for `jamtalk.co`
2. Navigate to **DNS** → **Records**
3. **Keep existing Worker records** (they won't conflict with subdomain)
4. **Add Vercel A records** for `free.jamtalk.co` (see above)
5. **Ensure Proxy status is OFF** (gray cloud, not orange)

### **Current Cloudflare Setup (Keep These):**
- `jamtalk.co` → **Worker: `jam-website`** ✅ (Main website)
- `api.jamtalk.co` → **Worker: `openai-gateway`** ✅ (API functionality)
- `free.jamtalk.co` → **Vercel A records** 🆕 (Campaign website)

### **Step 4: Verify DNS Propagation**
- Wait 5-10 minutes for DNS changes to propagate
- Check with: https://dnschecker.org
- Test: `ping free.jamtalk.co` should resolve to Vercel IPs

## 🔒 **Security & Performance Settings**

### **Cloudflare Settings to Configure:**
1. **SSL/TLS**: Set to "Full (strict)" for Vercel
2. **Security Level**: Medium or High
3. **Browser Integrity Check**: Enabled
4. **Always Use HTTPS**: Enabled
5. **Auto Minify**: CSS, JS, HTML enabled

### **Vercel Security Headers:**
Already configured in `vercel.json`:
- X-Content-Type-Options: nosniff
- X-Frame-Options: DENY
- X-XSS-Protection: 1; mode=block

## 📱 **Testing Your Setup**

### **After DNS Configuration:**
1. Visit `https://free.jamtalk.co` (should show your campaign site)
2. Test admin panel: `https://free.jamtalk.co?admin=true`
3. Verify mobile responsiveness
4. Check QR code functionality
5. Test form submission and redemption flow

## 🎯 **Subdomain Benefits**

### **Why `free.jamtalk.co` is Perfect:**
- ✅ **No conflicts** with existing Workers
- ✅ **Easy to remember** for marketing campaigns
- ✅ **Professional appearance** (free.jamtalk.co)
- ✅ **Separate from main site** (jamtalk.co)
- ✅ **Easy to manage** independently
- ✅ **Future campaigns** can use other subdomains

### **Marketing Advantages:**
- **Clear purpose**: "free" indicates free month offer
- **Brand consistency**: jamtalk.co domain
- **Easy sharing**: Simple URL for social media
- **Tracking**: Separate analytics from main site

## 🚨 **Important Notes**

### **No Conflicts Expected:**
- `jamtalk.co` → Worker (main website)
- `api.jamtalk.co` → Worker (API functionality)
- `free.jamtalk.co` → Vercel (campaign website)

### **Recommendations:**
1. **Keep all existing Workers** running
2. **Add Vercel A records** for `free.jamtalk.co`
3. **Test thoroughly** before launching campaign
4. **Monitor performance** of both main site and campaign

## 🔧 **Troubleshooting**

### **Common Issues:**
- **DNS Propagation**: Wait 5-10 minutes after changes
- **SSL Issues**: Cloudflare SSL mode must be "Full (strict)" for Vercel
- **Cache Issues**: Clear Cloudflare cache after DNS changes

### **Support Resources:**
- Vercel Documentation: https://vercel.com/docs/domains
- Cloudflare Help: https://support.cloudflare.com

---

**Status**: Ready for subdomain configuration
**Campaign URL**: `https://free.jamtalk.co`
**Next Step**: Add custom domain in Vercel dashboard
**Estimated Time**: 15-30 minutes for full setup
**Conflicts**: None expected with existing Workers
