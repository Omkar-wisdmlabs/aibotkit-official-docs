---
layout: default
title: Creating Your First Chatbot
category: guides
---

# 🤖 Creating Your First Chatbot: Complete Step-by-Step Guide

## What You'll Create

By the end of this guide, you'll have a fully functional AI chatbot that:
- ✅ Knows about your business and content
- ✅ Matches your website's style and branding
- ✅ Provides intelligent answers to visitors' questions
- ✅ Can be easily added to any page on your website

**Total Time Required:** 15-30 minutes (depending on how much you customize)

---

## 🚀 Getting Started

### **Before You Begin:**
1. **✅ API Keys Configured** - Make sure you've set up your AI provider (OpenAI, Anthropic, or Google)
2. **✅ Knowledge Base Ready** - Have some content prepared (documents, URLs, or WordPress posts)
3. **✅ Clear Purpose** - Know what you want your chatbot to help visitors with

### **How to Start Creating:**
1. Go to your WordPress admin dashboard
2. Click on **"AI BotKit"** in the left menu
3. Select the **"Chatbots"** tab
4. Click the **"Create New Bot"** button

---

# 📋 The 5-Step Creation Process

## Step 1: General Settings 🎯
*Foundation of your chatbot's identity*

### **What You'll Configure:**

#### **🏷️ Bot Name**
- **What it is:** The name visitors will see when chatting
- **Best practices:** 
  - Keep it friendly and professional: "Support Assistant", "Help Bot", "Sarah"
  - Avoid generic names like "Bot" or "AI"
  - Match your brand personality

#### **🎭 Bot Introduction/Personality**
- **What it is:** How your bot introduces itself and behaves
- **Default:** "helpful website assistant"
- **Examples:**
  - **E-commerce:** "friendly shopping assistant who helps customers find products"
  - **Service Business:** "knowledgeable consultant who guides clients through our services"
  - **Support:** "patient support representative who solves customer problems"

#### **⚡ Activate Chatbot**
- **When to check:** Only when you're ready to go live
- **Tip:** Leave unchecked while testing, check when ready for visitors

#### **🎨 Bot Tone**
Choose the personality that matches your brand:

| Tone | Best For | Example Response Style |
|------|----------|----------------------|
| **Professional** | B2B, Legal, Finance | "I'd be happy to assist you with that inquiry." |
| **Friendly** | Small Business, Community | "Great question! I'm here to help you out." |
| **Casual** | Startups, Creative, Youth | "Hey! Sure thing, let me help you with that." |

### **✅ Step 1 Checklist:**
- [ ] Choose a memorable bot name
- [ ] Write a clear personality description
- [ ] Select the right tone for your audience
- [ ] Leave "Activate" unchecked for now (we'll turn it on after testing)

---

## Step 2: Training Your Bot 📚
*Teaching your chatbot what it needs to know*

### **Why This Step Matters:**
Without training, your chatbot can only give generic answers. With proper training, it becomes an expert on YOUR specific business, products, and services.

### **Three Training Methods:**

#### **📝 Method 1: Import from WordPress**
**Best for:** Using content already on your website

**Step-by-Step:**
1. **Select Content Types**
   - Check boxes for content types you want (Posts, Pages, Products, etc.)
   - Use "Select All" for everything or pick specific types

2. **Preview Content**
   - Click "Preview Content" to see what will be imported
   - Review the list of posts/pages
   - Check boxes next to content you want to include

3. **Import Selected**
   - Click "Import Content"
   - Watch as content is processed (usually takes 1-2 minutes)

**💡 Smart Selection Tips:**
- **Include:** About pages, service descriptions, FAQ content, product information
- **Skip:** Contact forms, outdated posts, draft content
- **Start small:** Pick 5-10 high-quality pieces initially

#### **📚 Method 2: Select from Knowledge Base**
**Best for:** Using documents you've already uploaded

**How to Use:**
1. Search through your existing knowledge base
2. Check boxes next to relevant documents
3. Selected items automatically train your bot

#### **📄 Method 3: Upload New Content**
**Best for:** Adding specific documents for this chatbot

**Document Upload:**
- **Drag & drop** PDF files or **click to browse**
- **File limits:** Max 10 MB per file
- **Supported formats:** PDF (primary), TXT, MD
- **Add clear titles** for each document

**URL Addition:**
- **Paste complete URLs** (https://yoursite.com/page)
- **Add descriptive titles** for each URL
- **System automatically extracts** the main content

### **🎯 Training Strategy by Business Type:**

#### **For E-commerce Stores:**
- ✅ Product descriptions and specifications
- ✅ Shipping and return policies
- ✅ Size guides and FAQs
- ✅ Customer support documentation

#### **For Service Businesses:**
- ✅ Service descriptions and pricing
- ✅ Process explanations
- ✅ About us and team information
- ✅ Client testimonials and case studies

#### **For Content/Blog Sites:**
- ✅ Best performing blog posts
- ✅ About and mission pages
- ✅ Resource guides
- ✅ Contact and collaboration info

### **✅ Step 2 Checklist:**
- [ ] Import your most important WordPress content
- [ ] Upload key documents (if any)
- [ ] Add important URLs (if any)
- [ ] Verify content is processing (watch for "Completed" status)

---

## Step 3: Interface Configuration 💬
*Customizing how your bot communicates*

### **What You'll Set Up:**

#### **👋 Initial Greeting Message**
- **Purpose:** First thing visitors see when they open the chat
- **Default:** "Hi there! How can I help you today?"
- **Customization Tips:**
  - Make it specific to your business: "Welcome to [Company]! How can I assist you today?"
  - Include what you can help with: "Hi! I can help you with orders, product info, and support questions."
  - Keep it friendly and inviting

**Examples by Business Type:**
- **E-commerce:** "Welcome to our store! I can help you find products, check orders, or answer questions about shipping."
- **Service Business:** "Hello! I'm here to help you learn about our services and get your questions answered."
- **Support:** "Hi there! I can help troubleshoot issues, explain features, or connect you with the right team."

#### **🤔 Fallback Message**
- **Purpose:** Shown when the bot can't answer a question
- **Default:** "I don't have an answer for that. Can you rephrase your question?"
- **Better Examples:**
  - "I don't have information about that yet. You can try rephrasing your question or contact our team at [email]."
  - "That's outside my knowledge area. Let me connect you with someone who can help: [contact info]."
  - "I'm still learning about that topic! You can reach our support team at [contact] for more help."

#### **👍 Enable Feedback**
- **What it does:** Adds thumbs up/down buttons to bot responses
- **Benefits:** 
  - Learn what responses work well
  - Identify knowledge gaps
  - Improve bot performance over time
- **Recommendation:** Keep this enabled (it's checked by default)

### **✅ Step 3 Checklist:**
- [ ] Write a welcoming, specific greeting message
- [ ] Create a helpful fallback message with contact information
- [ ] Keep feedback enabled to improve your bot
- [ ] Test messages to ensure they sound natural

---

## Step 4: Model Configuration ⚙️
*Fine-tuning your AI's performance*

### **Understanding AI Models:**
Think of this like choosing the "brain power" for your chatbot. More powerful models give better answers but cost more per conversation.

### **Settings Explained:**

#### **🧠 AI Model Selection**
**Available models depend on your AI provider:**

**OpenAI Models:**
- **GPT-4o Mini** - Fast, cost-effective, good for simple questions
- **GPT-4o** - Balanced performance and cost
- **GPT-4 Turbo** - Most capable, best for complex questions

**Model Selection Guide:**
| Use Case | Recommended Model | Why |
|----------|------------------|-----|
| Simple FAQ bot | GPT-4o Mini | Cost-effective, fast responses |
| General customer support | GPT-4o | Good balance of capability and cost |
| Complex technical support | GPT-4 Turbo | Best understanding of complex queries |

#### **💬 Max Messages (Default: 5)**
- **What it controls:** How much chat history the AI remembers
- **Higher numbers:** Better context understanding, higher costs
- **Lower numbers:** Less context, lower costs
- **Sweet spot:** 3-7 messages for most use cases

#### **📄 Max Context Chunks (Default: 3)**
- **What it controls:** How many knowledge base documents the AI can reference per response
- **Higher numbers:** More comprehensive answers, higher costs
- **Lower numbers:** Focused answers, lower costs
- **Sweet spot:** 2-5 chunks for most use cases

#### **🔤 Max Tokens (Default: 1000)**
- **What it controls:** Maximum length of AI responses
- **1000 tokens ≈ 750 words**
- **Recommendations:**
  - **Short answers:** 500 tokens
  - **Detailed responses:** 1000-1500 tokens
  - **Very detailed:** 2000+ tokens

### **💰 Cost Optimization Tips:**
1. **Start conservative:** Use default settings initially
2. **Monitor usage:** Check your AI provider's usage dashboard
3. **Adjust based on needs:** Increase limits only if responses are too short/limited
4. **Test thoroughly:** Higher settings = higher costs per conversation

### **✅ Step 4 Checklist:**
- [ ] Select appropriate AI model for your use case
- [ ] Set conversation memory (3-7 messages recommended)
- [ ] Configure context chunks (2-5 recommended)
- [ ] Set response length (500-1500 tokens recommended)

---

## Step 5: Styles & Appearance 🎨
*Making your chatbot match your brand*

### **Visual Customization Options:**

#### **🎨 General Settings**

**Bot Avatar:**
- **Upload custom image:** 256x256 pixels recommended
- **File formats:** JPG, PNG, GIF
- **Tips:** Use your logo, mascot, or professional headshot
- **Fallback:** Robot emoji (🤖) if no image uploaded

**Primary Color:**
- **What it affects:** Chat bubble, send button, user messages
- **How to choose:** Match your website's main color
- **Color picker:** Click to select or enter hex code (#007fff)

**Font Settings:**
- **Font Family:** Inter, Roboto, Open Sans, Lato
- **Font Size:** 12-20 pixels (14px recommended)
- **Tip:** Match your website's typography

#### **🖼️ Header Settings**
**Background Color:**
- **Default:** White (#FFFFFF)
- **Custom:** Match your website header

**Font/Icon Color:**
- **Default:** Black (#000000)
- **Ensure contrast:** Make sure text is readable

#### **💬 Popup ChatBox Settings**
**Dimensions:**
- **Width:** 300-500 pixels (424px default)
- **Max Height:** 400-800 pixels (700px default)
- **Mobile tip:** Smaller widths work better on mobile

#### **🎯 Chat Window Settings**

**Background Colors:**
- **Chat window:** Usually white or light gray
- **AI messages:** Light blue or gray (#007fff1a)
- **User messages:** Your brand color (#007fff)

**Font Colors:**
- **AI message text:** Dark gray (#1C1C1C)
- **User message text:** White or dark (ensure readability)

#### **🔵 Chat Widget Bubble**
**Size Settings:**
- **Height & Width:** 40-80 pixels (55px default)
- **Keep proportional:** Same height and width for perfect circle

**Position:**
- **Bottom Right:** Most common, doesn't interfere with navigation
- **Bottom Left:** Good if you have other widgets on the right

### **🎨 Style Strategy by Brand:**

#### **Professional/Corporate:**
- **Colors:** Blues, grays, subtle
- **Font:** Roboto or Open Sans
- **Avatar:** Logo or professional headshot
- **Size:** Standard dimensions

#### **Creative/Fun:**
- **Colors:** Bright, brand-specific
- **Font:** Inter or Lato
- **Avatar:** Mascot or character
- **Size:** Slightly larger for visibility

#### **Minimalist:**
- **Colors:** Monochrome or single accent
- **Font:** Inter, clean
- **Avatar:** Simple logo or icon
- **Size:** Smaller, unobtrusive

### **📱 Mobile Optimization Tips:**
- **Test width:** Preview on mobile devices
- **Check colors:** Ensure readability on small screens
- **Position:** Bottom right usually works best
- **Size:** Don't make bubble too large

### **✅ Step 5 Checklist:**
- [ ] Upload bot avatar (optional but recommended)
- [ ] Set primary color to match your brand
- [ ] Configure font family and size
- [ ] Customize header colors
- [ ] Set chat window dimensions
- [ ] Choose bubble position (bottom right recommended)
- [ ] Test colors for readability and contrast

---

## 🎉 Final Steps: Testing & Launch

### **Before Going Live:**

#### **1. Save Your Chatbot**
- Click **"Save Chatbot"** button
- Wait for confirmation message
- Don't activate yet - test first!

#### **2. Test Your Chatbot**
**How to Test:**
1. Copy the shortcode: `[ai_botkit_chat id="your-bot-id"]`
2. Add it to a test page
3. Ask various questions to test responses
4. Check the knowledge and personality

**What to Test:**
- ✅ **Basic questions:** Ask about your business/services
- ✅ **Knowledge base:** Questions about uploaded content
- ✅ **Personality:** Check if tone matches expectations
- ✅ **Fallback:** Ask questions it shouldn't know
- ✅ **Appearance:** Check colors, sizing, positioning

#### **3. Refine if Needed**
**Common adjustments:**
- **Add more training content** if responses are too generic
- **Adjust personality** if tone doesn't match
- **Modify colors/sizing** if appearance needs tweaking
- **Update messages** if greeting/fallback need improvement

#### **4. Activate Your Chatbot**
**When you're satisfied:**
1. Go back to your chatbot list
2. Click "Edit" on your chatbot
3. Check the "Activate Chatbot" box
4. Save changes

### **🚀 Adding to Your Website:**

#### **Method 1: Shortcode (Specific Pages)**
```
[ai_botkit_chat id="your-bot-id"]
```
- **Use for:** Specific pages or posts
- **How:** Add to any page content via WordPress editor

#### **Method 2: Widget Code (Site-wide)**
```html
<!-- Copy from your chatbot dashboard -->
<script>Your widget code here</script>
```
- **Use for:** Every page on your site
- **How:** Add to theme footer or use a plugin

#### **Method 3: WordPress Widget**
- **Use for:** Sidebar or footer areas
- **How:** Appearance > Widgets > Add AI BotKit Widget

---

## 📊 Monitoring Performance

### **After Launch:**

#### **Check Analytics:**
- **Conversations tab:** See how many people are using your bot
- **Message history:** Read actual conversations
- **Feedback scores:** Monitor thumbs up/down ratings

#### **Continuous Improvement:**
- **Add new content:** Keep knowledge base updated
- **Refine responses:** Based on user feedback
- **Monitor costs:** Check AI provider usage
- **Update settings:** Adjust based on performance

---

## 🔧 Troubleshooting Common Issues

### **"Bot gives generic answers"**
**Solutions:**
- Add more specific training content
- Increase context chunks (Step 4)
- Upload more detailed documents

### **"Responses are too short"**
**Solutions:**
- Increase max tokens (Step 4)
- Improve personality description (Step 1)
- Add more comprehensive training content

### **"Bot doesn't match my brand"**
**Solutions:**
- Adjust personality and tone (Step 1)
- Customize colors and fonts (Step 5)
- Update greeting messages (Step 3)

### **"High AI costs"**
**Solutions:**
- Use a smaller AI model (Step 4)
- Reduce max messages and context chunks
- Lower max tokens setting
- Review conversation volume

---

## 🎯 Success Tips

### **For Best Results:**

1. **Start Simple:** Begin with basic functionality, expand later
2. **Test Thoroughly:** Spend time testing before going live
3. **Monitor Regularly:** Check conversations and feedback weekly
4. **Keep Updated:** Add new content as your business grows
5. **Iterate Often:** Continuously improve based on user interactions

### **Expected Timeline:**
- **Initial Setup:** 15-30 minutes
- **Testing Phase:** 1-2 days
- **Launch:** Immediate after testing
- **Optimization:** Ongoing process

---

## 🚀 You're Ready to Launch!

Congratulations! You now have a fully functional AI chatbot that:
- ✅ Represents your brand professionally
- ✅ Knows about your business and content
- ✅ Provides helpful answers to visitors
- ✅ Matches your website's design
- ✅ Can be easily managed and updated

**Next Steps:**
1. Complete your chatbot creation
2. Test thoroughly
3. Launch when ready
4. Monitor and improve continuously

Your AI assistant is ready to help your visitors 24/7! 🤖✨ 