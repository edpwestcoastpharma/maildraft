# WC Voice Draft – Setup (sirf 3 kaam)

Outlook me bolo, ChatGPT mail likhega aur draft ready karega. Kuch bhi auto-send nahi hota.

## 1. Files online daalo (5 min)
Is folder ko (zip extract karke) kisi bhi static hosting par daalo:

- **Netlify (sabse aasaan):** app.netlify.com/drop kholo, `wc-voice-draft` folder drag-drop karo. URL mil jayega jaise `https://xyz.netlify.app`
- **Vercel:** folder ko GitHub repo me push karo, phir vercel.com → Add New → Project → repo import → Deploy (koi build setting nahi chahiye)

## 2. Outlook me add karo
1. Browser me apna URL kholo (jaise `https://xyz.netlify.app`) → **Download manifest.xml** dabao.
   (Yeh file apne aap aapke URL ke hisaab se ban jaati hai, kuch edit nahi karna.)
2. outlook.office.com kholo → koi bhi mail kholo → **Apps / Get Add-ins** → **My add-ins** → **Add a custom add-in → Add from file** → `manifest.xml` chuno.

## 3. API key daalo (ek hi baar)
Koi mail kholo → **Voice Draft** button → ⚙ Settings → OpenAI API key, naam, signature → Save.
Key: platform.openai.com → API keys. Billing me thoda credit hona chahiye.

## Use kaise karein
- **New mail / Reply window:** Voice Draft → capsule dabao → bolo → dobara dabao. Mail body me draft aa jayega.
- **Aaya hua mail padhte waqt:** Voice Draft → bolo "inko bolo hum Friday tak dispatch kar denge" → reply draft khul jayega (Reply / Reply all choose kar sakte ho).
- Bolne ke baad text box me aapki baat dikhegi. Badalna ho to edit karke **Make draft** dabao.
- Hindi, Gujarati, English, Hinglish – kuch bhi bolo. Mail ki language Settings me choose karo.

## Problem aaye to
- **Mic blocked:** browser/Outlook me mic Allow karo. Classic Outlook desktop me na chale to Outlook Web ya New Outlook use karo. Tab tak text box me type karke bhi kaam chalega.
- **API key is wrong / credit over:** Settings me key check karo, OpenAI billing me credit daalo.
- **Button nahi dikh raha:** add karne ke baad 5–10 min lag sakte hain; Outlook refresh karo.

## Company ke sabhi logon ke liye
Microsoft 365 Admin Center → Settings → Integrated apps → Upload custom apps → wahi `manifest.xml`.
Har user apni API key apne Settings me daalega (ya ek common key sabko de do).

## Cost (andaza)
gpt-4o-mini + whisper-1 ke saath ek mail lagbhag ₹0.10–0.50.
