# 🔑 Setting Up Your AI Provider (LLM Configuration)

## What Are API Keys and Why Do You Need Them?

Think of API keys as your "membership cards" to use powerful AI services like OpenAI, Google, or Anthropic. These companies provide the intelligent "brains" that power your chatbot, but you need to have your own account and API key to access their services.

**Why do you need your own API key?**
- It ensures you have direct access to the latest AI models
- You only pay for what you use (usually very affordable for most websites)
- You get better performance and reliability
- You maintain control over your AI usage

## 🎯 Step-by-Step Setup Guide

### Step 1: Choose Your AI Provider

AI BotKit supports three leading AI providers. You only need to set up **ONE** of them:

| **Provider** | **Best For** | **Popular Models** | **Typical Cost** |
|--------------|--------------|-------------------|------------------|
| **🤖 OpenAI** | Most popular, great all-around performance | GPT-4, GPT-3.5 | $0.01-$0.03 per 1000 words |
| **🧠 Anthropic (Claude)** | Helpful, safe responses | Claude 3.5 Sonnet, Claude 3 Opus | $0.01-$0.075 per 1000 words |
| **🔍 Google AI** | Fast and efficient | Gemini Pro, Gemini Ultra | $0.001-$0.05 per 1000 words |

**💡 Recommendation for beginners:** Start with **OpenAI** as it's the most popular and well-documented.

---

## 🔧 Setting Up OpenAI (Recommended for Beginners)

### Step 1: Create Your OpenAI Account
1. Go to [https://platform.openai.com](https://platform.openai.com)
2. Click **"Sign up"** and create your account
3. Verify your email address
4. Add your phone number for verification

### Step 2: Add Payment Method
1. Once logged in, go to **"Billing"** in the left sidebar
2. Click **"Add payment method"**
3. Add your credit card (don't worry - you won't be charged much!)
4. Set a **spending limit** (start with $5-10 for testing)

### Step 3: Create Your API Key
1. Go to **"API Keys"** in the left sidebar
2. Click **"Create new secret key"**
3. Give it a name like "My Website Chatbot"
4. **Important:** Copy the key immediately! You won't be able to see it again
5. It will look like: `sk-proj-abc123...` (keep this safe!)

### Step 4: Configure in AI BotKit
1. In your WordPress admin, go to **AI BotKit > Settings**
2. Select **"OpenAI"** from the AI Engine dropdown
3. Paste your API key in the **"OpenAI API Key"** field
4. Click **"Verify"** to test the connection
5. If it shows a green checkmark, you're all set! ✅
6. Click **"Save Changes"**

**Organization ID (Optional):** If you're part of an OpenAI organization, you can add the Organization ID. Most users can leave this blank.

---

## 🤖 Setting Up Anthropic (Claude)

### Step 1: Create Your Anthropic Account
1. Go to [https://console.anthropic.com](https://console.anthropic.com)
2. Click **"Sign Up"** and create your account
3. Verify your email address

### Step 2: Add Credits
1. In the console, go to **"Credits"**
2. Click **"Purchase credits"**
3. Start with $5 in credits for testing

### Step 3: Generate API Key
1. Go to **"API Keys"** in the left menu
2. Click **"Create Key"**
3. Give it a name like "Website Chatbot"
4. Copy the key (it starts with `sk-ant-...`)

### Step 4: Get VoyageAI Key (For Embeddings)
Anthropic uses VoyageAI for embeddings (understanding document content):
1. Go to [https://dash.voyageai.com](https://dash.voyageai.com)
2. Sign up and verify your account
3. Go to **"API Keys"** and create a new key
4. Copy this key too

### Step 5: Configure in AI BotKit
1. In WordPress admin, go to **AI BotKit > Settings**
2. Select **"Anthropic"** from the AI Engine dropdown
3. Enter your **Anthropic API Key**
4. Enter your **VoyageAI API Key**
5. Click **"Verify"** to test both connections
6. Click **"Save Changes"**

---

## 🔍 Setting Up Google AI

### Step 1: Get Google AI Studio Access
1. Go to [https://makersuite.google.com](https://makersuite.google.com)
2. Sign in with your Google account
3. Accept the terms of service

### Step 2: Create API Key
1. Click **"Get API Key"** in the left sidebar
2. Click **"Create API Key"**
3. Select your Google Cloud project (or create a new one)
4. Copy the generated API key

### Step 3: Configure in AI BotKit
1. In WordPress admin, go to **AI BotKit > Settings**
2. Select **"Google"** from the AI Engine dropdown
3. Enter your **Google API Key**
4. Click **"Verify"** to test the connection
5. Click **"Save Changes"**

---

## ⚙️ Choosing the Right Models

After setting up your API keys, you can choose specific models:

### Chat Models (The "Brain" of Your Chatbot)
- **GPT-4 Turbo** (OpenAI): Most advanced, best for complex questions
- **GPT-3.5 Turbo** (OpenAI): Faster and cheaper, good for most use cases
- **Claude 3.5 Sonnet** (Anthropic): Great balance of speed and intelligence
- **Gemini Pro** (Google): Fast and efficient for straightforward questions

### Embedding Models (For Understanding Your Content)
- **Text Embedding 3 Small** (OpenAI): Good balance of cost and performance
- **Voyage 3 Large** (Anthropic): High-quality content understanding
- **Embedding 001** (Google): Efficient for basic content processing

**💡 Recommendation:** Start with the default selections - they work well for most websites!

---

## 💰 Understanding Costs

**Don't worry - AI costs are typically very low for most websites!**

### Typical Monthly Costs:
- **Small blog** (100 visitors, 50 questions): $1-3
- **Medium business site** (1000 visitors, 500 questions): $5-15
- **Large e-commerce** (5000 visitors, 2000 questions): $20-50

### Cost Factors:
- **Number of questions asked**
- **Length of responses**
- **Amount of content you've uploaded** (for initial processing)

### Money-Saving Tips:
1. Start with cheaper models (GPT-3.5 instead of GPT-4)
2. Set spending limits in your AI provider account
3. Monitor usage in the first month
4. Only upload essential documents initially

---

## 🔍 Testing Your Setup

### Quick Test:
1. Go to **AI BotKit > Settings**
2. Click **"Verify"** next to your API key
3. Look for a green checkmark ✅

### Full Test:
1. Create a simple chatbot
2. Add some basic content
3. Ask it a test question
4. If it responds intelligently, you're all set!

---

## 🚨 Troubleshooting Common Issues

### "Invalid API Key" Error
- ✅ Double-check you copied the key correctly (no extra spaces)
- ✅ Make sure the key hasn't expired
- ✅ Verify you have credits/billing set up

### "Rate Limit" Error
- ✅ You're making too many requests - wait a few minutes
- ✅ Check your provider's usage limits
- ✅ Consider upgrading your account tier

### "Insufficient Credits" Error
- ✅ Add more credits to your AI provider account
- ✅ Check your spending limits

### Connection Timeout
- ✅ Check your internet connection
- ✅ Try again in a few minutes
- ✅ Contact your hosting provider if issues persist

---

## 🔐 Security Best Practices

### Protecting Your API Keys:
✅ **Never share your API keys** with anyone  
✅ **Set spending limits** to avoid unexpected charges  
✅ **Regenerate keys** if you suspect they've been compromised  
✅ **Use different keys** for different projects  
✅ **Monitor usage** regularly in your provider dashboard  

### In AI BotKit:
- Your API keys are stored securely in WordPress
- They're encrypted and never displayed in plain text
- Only administrators can access them

---

## 🆘 Need Help?

### If You Get Stuck:
1. **Check the provider's documentation:**
   - [OpenAI Help Center](https://help.openai.com)
   - [Anthropic Support](https://support.anthropic.com)
   - [Google AI Studio Help](https://support.google.com/ai-studio)

2. **Verify your account setup:**
   - Confirm email verification
   - Check billing/credits
   - Review spending limits

3. **Test with simple examples first**
   - Try a basic question
   - Check the verification button
   - Monitor provider dashboards

**Remember:** The initial setup might seem complex, but once it's done, your chatbot will work automatically! Most users find the setup takes just 10-15 minutes, and then they never have to think about it again.

---

## 🚀 What's Next?

Once your API keys are configured:
1. ✅ **Create your first chatbot** → [Chatbot Creation Guide](create-chatbot.md)
2. ✅ **Add your content** → [Knowledge Base Guide](add-knowledge-base.md)
3. ✅ **Customize the appearance** → [Customization Guide](customization.md)

**Congratulations!** You've just connected your website to cutting-edge AI technology! 🎉 