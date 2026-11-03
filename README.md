# WC Voice Draft – Setup

Outlook me bolo, AI mail likhega aur draft ready karega. Kuch bhi auto-send nahi hota.
Default: **Groq (FREE)**. Chaho to Settings me OpenAI (paid) bhi chun sakte ho.

## Pehle se install hai? (sirf update)
1. Is folder ki saari files Vercel project me replace karo (GitHub push) – naya file `record.html` bhi zaroor daalna.
2. `manifest.xml` dobara install NAHI karna.
3. Outlook me Ctrl + Shift + R → WC Voice Draft kholo → ⚙ Settings.

## Naya install
1. Folder Vercel/Netlify par daalo → apna URL kholo → **Download manifest.xml**.
2. Outlook Web → aka.ms/olksideload → My add-ins → Add a custom add-in → Add from file → manifest.xml.

## Free API key (Groq)
1. console.groq.com → Google se sign in.
2. API Keys → Create API Key → `gsk_...` copy karo.
3. Outlook → WC Voice Draft → ⚙:
   - AI service: **Groq (free)**
   - API key: `gsk_...`
   - Writing model: `llama-3.3-70b-versatile` (better writing chahiye to `openai/gpt-oss-120b`)
   - Voice model: `whisper-large-v3`
   - Signature: khali chhodo agar Outlook khud signature lagata hai
   - Save

## Use
- Capsule dabao → bolo → dobara dabao → draft mail me aa jayega.
- Aaya hua mail: Voice Draft → bolo → reply draft khulega (Reply / Reply all).
- Text box me edit karke **Make draft** se dobara bana sakte ho.

## Mic blocked?
Tool apne aap ek chhoti **pop-up recorder window** khol dega (ya link dabao:
"Mic not working? Record in a pop-up window"). Pop-up me mic Allow karo.
Outlook "allow pop-up" pooche to Allow dabao.
Phir bhi na chale: Windows Settings → Privacy & security → Microphone → ON.

## Limits
Groq free: voice 20/min, 2000/day – roz ke mail ke liye kaafi.
