# ⚙️ Advanced Settings Guide

## What Are Advanced Settings?

Once you've set up your API keys, AI BotKit offers several advanced settings that control how your chatbot processes content and interacts with users. Think of these as the "fine-tuning knobs" that help you optimize your chatbot's performance and behavior.

**💡 Good News:** The default settings work well for most websites! You only need to adjust these if you have specific requirements or want to optimize performance.

---

## 📋 Complete Settings Overview

| Setting | What It Does | Default Value | When To Change |
|---------|--------------|---------------|----------------|
| **Admin Email** | Receives important notifications | WordPress admin email | For dedicated AI admin |
| **Chunk Size** | How AI reads your content | 1000 characters | For very long or short documents |
| **Chunk Overlap** | Content context preservation | 200 characters | For better answer continuity |
| **Rate Limit Window** | Time period for usage limits | 60 seconds | For high-traffic sites |
| **Rate Limit Max Requests** | Maximum requests per window | 60 requests | For cost control or performance |

---

## 📧 Admin Email

### What It Does:
The email address that receives important notifications about your AI BotKit, including:
- System alerts and errors
- Usage warnings
- Performance notifications
- Security alerts

### Default Setting:
Uses your WordPress admin email address.

### When To Change:
✅ **You want a dedicated person to manage AI notifications**  
✅ **Your WordPress admin email gets too much mail**  
✅ **You have a team managing the chatbot**  

### Recommended Settings:
- **Small sites:** Keep default WordPress admin email
- **Business sites:** Use dedicated email like `ai-admin@yoursite.com`
- **Team management:** Use group email or support email

---

## 📄 Chunk Size

### What It Does:
When AI BotKit processes your documents, it breaks them into smaller pieces called "chunks." Think of it like cutting a book into chapters - each chunk contains related information that the AI can understand and reference.

**Simple Analogy:** If your document is a pizza, chunk size determines how big each slice is.

### How It Works:
- **Larger chunks** = More context per piece, but fewer total pieces
- **Smaller chunks** = More precise targeting, but less context per piece

### Default Setting:
**1000 characters** (roughly 150-200 words)

### Range:
- **Minimum:** 100 characters
- **Maximum:** 2000 characters
- **Step:** 100 characters

### When To Adjust:

#### **Increase Chunk Size (1200-1500) When:**
✅ **Your content has long explanations** (tutorials, detailed guides)  
✅ **You want more context in answers**  
✅ **Your documents have complex, interconnected topics**  
✅ **You're getting fragmented or incomplete answers**  

#### **Decrease Chunk Size (600-800) When:**
✅ **Your content is mostly short FAQs**  
✅ **You want more precise, focused answers**  
✅ **Your documents have many separate topics**  
✅ **You're getting overly long or unfocused answers**  

### Real-World Examples:

**E-commerce Store (Recommend: 800-1000)**
- Product descriptions are usually concise
- Users ask specific questions about features

**Educational Site (Recommend: 1200-1500)**
- Content is detailed and explanatory
- Concepts build on each other

**FAQ Site (Recommend: 600-800)**
- Each answer is typically standalone
- Users want quick, direct responses

---

## 🔗 Chunk Overlap

### What It Does:
This setting ensures that important information doesn't get "lost" between chunks. It's like having overlapping sections in a book so you don't miss the connection between chapters.

**Simple Analogy:** If chunk size is how big each pizza slice is, overlap is how much each slice shares with its neighbors.

### How It Works:
- Takes the last X characters from one chunk
- Includes them at the beginning of the next chunk
- Ensures context continuity between chunks

### Default Setting:
**200 characters** (roughly 30-40 words)

### Range:
- **Minimum:** 0 characters (no overlap)
- **Maximum:** 200 characters (20% of default chunk size)

### When To Adjust:

#### **Increase Overlap (300-400) When:**
✅ **Your content has lots of cross-references**  
✅ **Topics are highly interconnected**  
✅ **You're getting answers that miss important connections**  
✅ **Your content has step-by-step processes**  

#### **Decrease Overlap (50-100) When:**
✅ **Your content is mostly independent sections**  
✅ **You want to reduce processing time**  
✅ **Your content has clear topic boundaries**  
✅ **Storage/cost optimization is important**  

### Impact on Performance:
- **More overlap** = Better context but higher processing costs
- **Less overlap** = Faster processing but potential context loss

---

## ⏱️ Rate Limit Window

### What It Does:
Controls the time period for counting API requests. Think of it as a "rolling window" that tracks how many requests users make.

**Simple Analogy:** Like having a timer that resets every X seconds to count fresh requests.

### How It Works:
- Tracks requests made in the last X seconds
- When window expires, counter resets
- Prevents abuse and controls costs

### Default Setting:
**60 seconds** (1 minute)

### Range:
- **Minimum:** 1 second
- **Maximum:** 3600 seconds (1 hour)

### When To Adjust:

#### **Increase Window (300-900 seconds) When:**
✅ **You want longer-term usage tracking**  
✅ **Your site has steady, consistent traffic**  
✅ **You prefer hourly rather than minute-based limits**  
✅ **You want to smooth out traffic spikes**  

#### **Decrease Window (15-30 seconds) When:**
✅ **You want strict, immediate rate limiting**  
✅ **Your site gets sudden traffic bursts**  
✅ **You want to prevent rapid-fire requests**  
✅ **Cost control is critical**  

---

## 🚦 Rate Limit Max Requests

### What It Does:
Sets the maximum number of chatbot requests allowed within the rate limit window. This is your primary tool for controlling usage and costs.

**Simple Analogy:** Like setting a speed limit - it determines how fast users can make requests.

### Default Setting:
**60 requests** per window (1 request per second on average)

### Range:
- **Minimum:** 1 request
- **Maximum:** 1000 requests

### When To Adjust:

#### **Increase Limit (100-200) When:**
✅ **You have high-traffic periods**  
✅ **Multiple users chat simultaneously**  
✅ **You want to provide unlimited-feeling experience**  
✅ **Your AI budget is flexible**  

#### **Decrease Limit (20-40) When:**
✅ **You want to control AI costs strictly**  
✅ **Your site has mostly single users**  
✅ **You're testing the chatbot initially**  
✅ **You want to prevent abuse**  

### Usage Scenarios:

**Small Blog (Recommend: 30-50 requests)**
- Few concurrent users
- Casual interaction patterns

**Business Website (Recommend: 60-100 requests)**
- Moderate traffic
- Standard business hours usage

**E-commerce Store (Recommend: 100-200 requests)**
- High traffic during sales
- Multiple customer service interactions

**Educational Platform (Recommend: 150-300 requests)**
- Students asking many questions
- Peak usage during class times

---

## 🎯 Choosing The Right Settings For Your Site

### 📝 **Content-Heavy Blog or Documentation Site**
```
Chunk Size: 1200-1500 characters
Chunk Overlap: 250-300 characters
Rate Limit Window: 60 seconds
Max Requests: 80-120
```
**Why:** Long-form content benefits from larger chunks with good overlap for context.

### 🛒 **E-commerce Product Catalog**
```
Chunk Size: 800-1000 characters
Chunk Overlap: 150-200 characters
Rate Limit Window: 60 seconds
Max Requests: 100-200
```
**Why:** Product info is concise, but you need to handle customer service spikes.

### ❓ **FAQ or Support Site**
```
Chunk Size: 600-800 characters
Chunk Overlap: 100-150 characters
Rate Limit Window: 60 seconds
Max Requests: 60-100
```
**Why:** FAQs are usually standalone, so smaller chunks work better.

### 🎓 **Educational or Training Platform**
```
Chunk Size: 1300-1600 characters
Chunk Overlap: 300-400 characters
Rate Limit Window: 120 seconds
Max Requests: 150-250
```
**Why:** Educational content is interconnected, students ask many questions.

### 💼 **Professional Services Site**
```
Chunk Size: 1000-1200 characters
Chunk Overlap: 200-250 characters
Rate Limit Window: 60 seconds
Max Requests: 40-80
```
**Why:** Professional content needs context, but traffic is usually moderate.

---

## 🧪 Testing Your Settings

### Step 1: Start with Defaults
Begin with default settings and monitor performance for a week.

### Step 2: Monitor Key Metrics
- **Response Quality:** Are answers complete and accurate?
- **Response Speed:** How fast does the chatbot respond?
- **User Experience:** Do users get frustrated with limits?
- **Costs:** Are AI expenses within budget?

### Step 3: Adjust Gradually
Change one setting at a time and observe the impact:

1. **If answers seem incomplete:** Increase chunk size
2. **If answers lose context:** Increase chunk overlap
3. **If users hit rate limits:** Increase max requests or window
4. **If costs are too high:** Decrease max requests or chunk size

### Step 4: Monitor for 24-48 Hours
Give each change time to show its effects before making additional adjustments.

---

## 💰 Impact on Costs

### Settings That Increase Costs:
- **Larger chunk sizes** (more tokens processed)
- **Higher chunk overlap** (more redundant content)
- **Higher rate limits** (more API calls allowed)

### Settings That Decrease Costs:
- **Smaller chunk sizes** (fewer tokens per request)
- **Lower chunk overlap** (less redundant processing)
- **Lower rate limits** (fewer API calls allowed)

### Cost Optimization Tips:
1. **Start conservative** with limits and increase gradually
2. **Monitor usage patterns** in provider dashboards
3. **Set spending alerts** in your AI provider account
4. **Use smaller chunks** for simple content types
5. **Consider time-based restrictions** during low-value hours

---

## 🚨 Troubleshooting Common Issues

### "Answers seem incomplete or cut off"
**Solution:** Increase chunk size to 1200-1500 characters

### "Chatbot loses context between related topics"
**Solution:** Increase chunk overlap to 250-300 characters

### "Users complain about rate limiting"
**Solution:** Increase max requests or extend the time window

### "AI costs are too high"
**Solution:** Decrease max requests and optimize chunk sizes

### "Responses are too slow"
**Solution:** Decrease chunk size and overlap, check rate limits

### "Getting irrelevant answers"
**Solution:** Decrease chunk size for more precise targeting

---

## 🔧 Advanced Tips for Power Users

### Seasonal Adjustments:
- **Increase rate limits** during sales periods or events
- **Adjust chunk sizes** based on content updates
- **Monitor and adjust** based on traffic patterns

### A/B Testing Settings:
- Test different chunk sizes with a portion of users
- Compare response quality and user satisfaction
- Gradually roll out optimal settings

### Content-Type Specific Settings:
- Use different chatbots with different settings for different content types
- Technical documentation vs. marketing content may need different approaches

### Monitoring and Alerts:
- Set up monitoring for rate limit hits
- Track response quality over time
- Monitor cost trends and set budgets

---

## 📞 When To Seek Help

Contact support or consider professional setup if:
- Your costs are unexpectedly high despite optimization
- Users consistently report poor answer quality
- You're experiencing frequent rate limiting issues
- Your content has unique requirements not covered here

**Remember:** These settings can always be adjusted! Start with defaults, monitor performance, and fine-tune based on your specific needs and user feedback.

---

## 🚀 Quick Start Recommendations

### For Most Users (Recommended Starting Point):
```
Admin Email: [Your preferred email]
Chunk Size: 1000 characters (default)
Chunk Overlap: 200 characters (default)
Rate Limit Window: 60 seconds (default)
Max Requests: 60 requests (default)
```

### After One Week, Consider:
- Reviewing usage patterns in your AI provider dashboard
- Checking user feedback on answer quality
- Monitoring any rate limiting issues
- Adjusting one setting at a time based on observations

**The key is to start simple and optimize based on real usage data rather than trying to perfect settings before launch!** 