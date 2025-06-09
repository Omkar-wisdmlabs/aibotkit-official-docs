---
layout: default
title: Installation Guide
category: guides
---

# 🚀 Installation Guide - Getting AI BotKit Up and Running

Welcome to AI BotKit! Let's get your intelligent chatbot installed and ready to amaze your website visitors. Think of this as setting up your new digital assistant - we'll make sure everything is perfect! ✨

---

## ✅ Prerequisites - What You Need Before Starting

Before installing AI BotKit, make sure your website meets these requirements. It's like checking if your house is ready before moving in new furniture! 🏠

### 🌐 **WordPress Requirements**
- **WordPress 5.8 or higher** 📊
  - *Why?* We use modern WordPress features for the best performance
  - *How to check:* Go to your WordPress admin → Dashboard → At a Glance

### 🔧 **Server Requirements**
- **PHP 7.4 or higher** ⚡
  - *Why?* AI BotKit uses advanced PHP features for speed and security
  - *How to check:* Ask your hosting provider or use a plugin like "WP Server Info"

- **MySQL 5.6 or higher** 💾
  - *Why?* We need modern database features to store conversations and analytics
  - *How to check:* Contact your hosting provider for database version

### 🔒 **Security Requirements**
- **SSL Certificate (HTTPS)** 🛡️
  - *Why?* AI providers require secure connections for API communication
  - *How to check:* Your website URL should start with `https://` (not `http://`)
  - *Don't have SSL?* Most hosting providers offer free SSL certificates!

### 💡 **Quick Prerequisites Check**

**✅ All Good?** You should see:
- WordPress admin shows version 5.8+ 
- Your website URL starts with `https://`
- No PHP errors in your error logs

**❌ Need Help?** Contact your hosting provider to upgrade:
- WordPress version
- PHP version  
- MySQL version
- SSL certificate installation

---

## 📥 Installation Methods

Choose the method that works best for you! Both lead to the same amazing result. 🎯

---

## 🎯 Method 1: WordPress Admin Panel (Recommended)

This is the easiest way - perfect for beginners! WordPress does all the heavy lifting for you. 🏋️‍♀️

### 📝 Step-by-Step Instructions

#### **Step 1: Access Your WordPress Admin** 🔑
1. Open your website in a browser
2. Add `/wp-admin` to your URL (e.g., `https://yoursite.com/wp-admin`)
3. Log in with your administrator credentials

#### **Step 2: Navigate to Plugins** 🔌
1. In your WordPress dashboard, look for **"Plugins"** in the left sidebar
2. Click on **"Add New"**
3. You'll see the WordPress plugin repository

#### **Step 3: Upload AI BotKit** 📤
1. Click the **"Upload Plugin"** button at the top
2. Click **"Choose File"** and select your `ai-botkit.zip` file
3. Click **"Install Now"**

*🎬 You'll see a progress bar - grab some coffee while WordPress works its magic!*

#### **Step 4: Activate the Plugin** ⚡
1. Once upload completes, click **"Activate Plugin"**
2. You'll see a success message: *"Plugin activated successfully!"*
3. Look for **"AI BotKit"** in your left sidebar - that's your new control center! 🎮

#### **Step 5: Verify Installation** ✅
1. Click on **"AI BotKit"** in your WordPress sidebar
2. You should see the welcome dashboard
3. If you see the interface, congratulations! 🎉

### 🎯 **Why We Recommend This Method:**
- ✅ **Automatic file permissions** - WordPress handles everything
- ✅ **Built-in error checking** - WordPress validates the plugin
- ✅ **Easy updates** - Future updates are one-click
- ✅ **Rollback friendly** - Easy to deactivate if needed

---

## 🛠️ Method 2: Manual Installation via FTP/File Manager

For advanced users who want full control over the installation process. 💪

### 📁 **What You'll Need:**
- FTP client (like FileZilla) OR hosting file manager
- Your website's FTP credentials
- Basic file management skills

### 📝 **Step-by-Step Instructions**

#### **Step 1: Prepare the Plugin Files** 📦
1. Download the `ai-botkit.zip` file to your computer
2. **Extract/unzip** the file - you'll get a folder named `ai-botkit`
3. Keep this folder handy for uploading

#### **Step 2: Access Your Website Files** 🌐
**Option A: Using FTP Client**
1. Open your FTP client (FileZilla, WinSCP, etc.)
2. Connect using your FTP credentials
3. Navigate to your website's root directory
4. Go to `/wp-content/plugins/`

**Option B: Using Hosting File Manager**
1. Log into your hosting control panel (cPanel, Plesk, etc.)
2. Open **"File Manager"**
3. Navigate to `public_html/wp-content/plugins/`

#### **Step 3: Upload the Plugin** 📤
1. Upload the entire `ai-botkit` folder to `/wp-content/plugins/`
2. Make sure the folder structure looks like:
   ```
   /wp-content/plugins/ai-botkit/
   ├── ai-botkit.php
   ├── includes/
   ├── admin/
   ├── public/
   └── (other files...)
   ```

#### **Step 4: Set Proper Permissions** 🔧
Set these permissions (ask your hosting provider if unsure):
- **Folders**: 755 or 750
- **Files**: 644 or 640

#### **Step 5: Activate via WordPress** ⚡
1. Go to your WordPress admin panel
2. Navigate to **Plugins → Installed Plugins**
3. Find **"AI BotKit"** in the list
4. Click **"Activate"**

### ⚠️ **Manual Installation Tips:**
- 🔍 **Double-check folder names** - case-sensitive on some servers
- 📁 **Verify file structure** - main plugin file should be directly accessible
- 🔒 **Check permissions** - wrong permissions cause activation failures
- 💾 **Backup first** - always backup before manual installations

---

## 🎉 Post-Installation Setup

Congratulations! AI BotKit is installed. Now let's get it configured! 🚀

### **Immediate Next Steps:**

#### **1. First-Time Setup Wizard** 🧙‍♂️
1. Click on **"AI BotKit"** in your WordPress sidebar
2. Follow the setup wizard to configure basic settings
3. The wizard will guide you through essential configuration

#### **2. API Configuration** 🔑
1. Navigate to **AI BotKit → Settings**
2. Add your OpenAI, Anthropic, or Google AI API keys
3. Test the connection to ensure everything works

#### **3. Knowledge Base Setup** 📚
1. Go to **AI BotKit → Knowledge Base**
2. Upload your first documents or import content
3. Wait for processing to complete

#### **4. Test Your Chatbot** 🧪
1. Use the built-in testing interface
2. Ask a few questions to verify responses
3. Check that your knowledge base is working

### **📋 Post-Installation Checklist:**
- [ ] Plugin activated successfully
- [ ] AI BotKit menu appears in WordPress sidebar
- [ ] API keys configured and tested
- [ ] First knowledge base content added
- [ ] Test conversation completed successfully
- [ ] No error messages in WordPress admin

---

## 🔧 Troubleshooting Common Installation Issues

Don't panic if something goes wrong! Here are solutions to common problems. 🛠️

### 😱 **"Plugin could not be activated"**

**Possible Causes & Solutions:**

**🔴 PHP Version Too Old**
- *Problem:* Your server runs PHP below 7.4
- *Solution:* Contact hosting provider to upgrade PHP
- *Check:* WordPress admin → Tools → Site Health

**🔴 WordPress Version Too Old**
- *Problem:* WordPress below 5.8
- *Solution:* Update WordPress via Dashboard → Updates
- *Warning:* Backup your site before major WordPress updates!

**🔴 File Permissions Issues**
- *Problem:* Incorrect file permissions (manual installation)
- *Solution:* Set folders to 755, files to 644
- *Help:* Contact hosting provider for permission assistance

### 😵 **"Plugin not appearing in admin menu"**

**Quick Fixes:**
1. **Hard refresh** your browser (Ctrl+F5 or Cmd+Shift+R)
2. **Clear caching** plugins if you use any
3. **Deactivate and reactivate** the plugin
4. **Check user permissions** - you need administrator access

### 🌐 **"SSL Certificate Required" Error**

**Solutions:**
1. **Get free SSL** from your hosting provider
2. **Enable HTTPS** in WordPress settings
3. **Force HTTPS** using plugins like "Really Simple SSL"
4. **Contact support** if you can't enable SSL

### 💾 **"Database Error" During Installation**

**Steps to Fix:**
1. **Check MySQL version** with hosting provider
2. **Verify database permissions** - WordPress user needs CREATE TABLE rights
3. **Ensure sufficient disk space** for database growth
4. **Contact hosting support** for database issues

### 🔄 **"Installation Incomplete" or Stuck**

**Troubleshooting:**
1. **Increase PHP memory limit** (ask hosting provider)
2. **Check for plugin conflicts** - deactivate other plugins temporarily
3. **Clear browser cache** and try again
4. **Use alternative installation method** (switch between Method 1 and 2)

---

## 🆘 Getting Help

If you're still having trouble, don't worry! Help is available. 🤝

### **📞 Support Channels:**
1. **Plugin Documentation** - Check our other guides
2. **WordPress Forums** - Community support
3. **Hosting Provider** - For server-related issues
4. **AI BotKit Support** - For plugin-specific problems

### **📊 Information to Provide When Seeking Help:**
- WordPress version
- PHP version  
- Plugin version
- Error messages (exact text)
- Steps you've already tried
- Hosting provider name

### **🔍 Debug Information:**
Enable WordPress debug mode to get detailed error information:
1. Edit your `wp-config.php` file
2. Add: `define('WP_DEBUG', true);`
3. Check error logs for specific issues

---

## 🎯 Best Practices for Installation

### **✅ Before Installing:**
- 🔄 **Backup your website** - always backup before installing new plugins
- 🧪 **Test on staging site** - if you have one available
- 📊 **Check server resources** - ensure adequate memory and storage
- 🔒 **Verify SSL certificate** - test HTTPS functionality

### **✅ During Installation:**
- 🕐 **Allow sufficient time** - don't rush the process
- 🌐 **Stable internet connection** - avoid interruptions
- 👀 **Watch for error messages** - address issues immediately
- 📱 **Avoid browser switching** - complete installation in one session

### **✅ After Installation:**
- 🧪 **Test thoroughly** - verify all functionality works
- 📊 **Monitor performance** - check site speed impact
- 🔄 **Configure backups** - include plugin data in backups
- 📈 **Plan for updates** - keep plugin updated for security

---

## 🎊 Welcome to AI BotKit!

You've successfully installed AI BotKit! 🎉 Your website now has the power of advanced AI chatbot technology.

### **🚀 What's Next?**
1. **[Configure Your API Keys](add-LLM.md)** - Connect to AI providers
2. **[Set Up Knowledge Base](add-knowledge-base.md)** - Add your content
3. **[Customize Settings](../Explanation/advanced-settings.md)** - Optimize performance
4. **[Create Your Chatbot](create-chatbot.md)** - Build your AI assistant

### **💡 Pro Tip:**
Take your time with the initial setup. A well-configured chatbot will serve your users better and save you time in the long run! 

Ready to create an amazing AI assistant for your website? Let's go! 🚀

---

*Need help with the next steps? Check out our [LLM Configuration Guide](add-LLM.md) to get your AI providers connected!* 💪 