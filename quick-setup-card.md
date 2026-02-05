# EmailJS Quick Setup Reference Card
## 5-Minute Setup Guide

---

## 📝 STEP-BY-STEP CHECKLIST

### □ Step 1: Create Account
- Go to: **https://www.emailjs.com/**
- Click "Sign Up Free"
- Verify email

### □ Step 2: Add Email Service
- Dashboard → "Email Services"
- Click "Add New Service"
- Choose Gmail (easiest)
- **SAVE SERVICE ID**: `service_________`

### □ Step 3: Create Template
- Dashboard → "Email Templates"  
- Click "Create New Template"
- **SAVE TEMPLATE ID**: `template_________`

### □ Step 4: Get Public Key
- Dashboard → "Account" → "General"
- **SAVE PUBLIC KEY**: `_________________`

### □ Step 5: Update HTML (3 Locations)

**Location 1** (~line 1420):
```javascript
emailjs.init('YOUR_PUBLIC_KEY');
```

**Location 2** (~line 1440):
```javascript
emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', form)
```

### □ Step 6: Test
- Open portfolio in browser
- Fill out contact form
- Click "Send Message"
- Check your email!

---

## 📋 YOUR CREDENTIALS

Write your IDs here for easy reference:

```
PUBLIC KEY:   _________________________________

SERVICE ID:   _________________________________

TEMPLATE ID:  _________________________________
```

---

## 🎯 TEMPLATE EXAMPLE

**Subject:**
```
New Contact: {{subject}}
```

**Body:**
```
From: {{from_name}}
Email: {{reply_to}}
Subject: {{subject}}

Message:
{{message}}
```

**To Email:** your-email@example.com

---

## ⚡ QUICK TROUBLESHOOTING

❌ **"EmailJS is not defined"**
→ Check EmailJS script in `<head>` tag

❌ **"Invalid public key"**  
→ Copy exact key from EmailJS dashboard

❌ **"Service not found"**
→ Verify Service ID matches dashboard

❌ **"Template not found"**
→ Verify Template ID matches dashboard

❌ **Emails not arriving**
→ Check spam folder
→ Verify template "To Email" setting

---

## 📱 FREE PLAN INCLUDES

✅ 200 emails/month
✅ Unlimited services
✅ Unlimited templates
✅ No credit card required

**Perfect for portfolios!**

---

## 🔗 USEFUL LINKS

**EmailJS Dashboard:**
https://dashboard.emailjs.com/

**Documentation:**
https://www.emailjs.com/docs/

**Support:**
support@emailjs.com

---

## ✅ FINAL CHECKLIST

- [ ] Account created
- [ ] Email service connected
- [ ] Template created  
- [ ] All 3 IDs copied
- [ ] HTML updated in 3 places
- [ ] Tested successfully
- [ ] Email received

**🎉 DONE! Your contact form is live!**
