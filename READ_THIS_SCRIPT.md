# LeoConnect Speaking Script
## Just Read This - Word for Word

---

## SLIDE 1: TITLE (30 seconds)

Hello everyone! We're Team Rexosphere from the University of Moratuwa.

Today, we're excited to present LeoConnect — a platform built specifically for Leo Multiple District 306.

Our theme is "Strive to Thrive" — because when Leo Clubs work together, their impact multiplies.

---

## SLIDE 2: TEAM (30 seconds)

We are Team Rexosphere — a group of four developers passionate about solving real problems with smart engineering.

Our team consists of Ifaz Ikram, Kalana Liyanage, Sangeeth Kariyapperuma, and Suhas Dissanayake.

Together, we bring expertise in mobile development, backend architecture, and AI integration — all from the University of Moratuwa.

---

## SLIDE 3: THE PROBLEM (1 minute 30 seconds)

Before we show our solution, let's understand the scale of Leo MD 306.

Leo MD 306 spans 12 Districts — D1 through D12 — covering the entirety of Sri Lanka and extending to the Maldives.

There are over 200 clubs and more than 4000 active members serving communities across these regions.

This is a massive, powerful network.

**[PAUSE]**

But here's the problem... there's no unified platform.

Communication is fragmented across WhatsApp groups and Facebook pages. Important updates get buried. Information is scattered.

Members in District 1 cannot easily discover what clubs in District 7 are doing. There's no visibility across districts.

Events are planned in isolation. Clubs don't know about each other's activities. Overlapping dates. Missed opportunities for collaboration.

And most critically — inter-club collaboration is limited. Despite being part of one movement, clubs work alone.

We asked ourselves: How can we unite this incredible movement digitally?

---

## SLIDE 4: SOLUTION (1 minute)

Introducing LeoConnect — the unified platform designed specifically for Leo Clubs.

Social Feed — posts, likes, comments. Everyone sees updates in one place. No more scattered WhatsApp messages.

Club Discovery — browse all 12 districts, over 90 clubs. A member in Colombo can now see what clubs in Jaffna are doing.

Events plus RSVP — that's Répondez S'il Vous Plaît, or simply "respond please" — create events, publish them, let members respond. Coordinated, not chaotic.

Leo AI — an AI-powered assistant that understands Leo context. Not a generic chatbot — a Leo-specific guide.

Messaging — real-time direct messages. Keep communication inside one platform.

Notifications — push alerts for events, messages, updates. Nothing important gets missed.

Verified Accounts — 30 plus official Leo leaders already verified. Trusted communication, no impersonation.

Cross-Platform — works on mobile AND desktop. Accessible anywhere.

One app to connect Colombo to Jaffna, even Malé!

---

## SLIDE 5: ARCHITECTURE (1 minute)

Before we show the demo, let me walk you through how LeoConnect is built.

At the top, we have Client Apps built with Kotlin Multiplatform — or KMP — which lets us write one shared codebase for multiple platforms. That's Android — at only around 6 megabytes — plus iOS, Desktop, and Web.

We also have a separate Admin Dashboard built with Vue.js and Vite for managing users, clubs, and analytics.

Both connect to our Cloudflare Edge Backend. Code runs close to users — not in one faraway server — which is why we achieve sub-50 millisecond latency.

Data is stored in D1 SQL for structured information, and R2 CDN for media delivery worldwide.

Powering our intelligence layer is Leo AI — using Gemini 2.0 Flash with a RAG architecture. That means the AI answers using a Leo-specific knowledge base, not random hallucinations.

The result? Less than 50 milliseconds latency across 300 plus CDN cities worldwide. One codebase. Four platforms.

---

## SLIDE 6: VIDEO DEMO (7 minutes)

Now that you understand the architecture, let's see LeoConnect in action.

**[CLICK PLAY OR FULLSCREEN - VIDEO RUNS FOR 7 MINUTES]**

---

## SLIDE 7: TECHNICAL INNOVATION (1 minute)

What makes our tech stack innovative?

First, Kotlin Multiplatform.

Normally, you'd need 3 separate codebases — one for Android, one for iOS, one for Desktop. That's triple the work, triple the bugs.

With KMP, we have one shared codebase. Fix a bug once — it's fixed everywhere. This is why we can support 4 platforms as a small team.

Our competitors? Mobile only. We have Desktop too.

Second, Cloudflare Edge Computing.

Traditional servers respond in around 200 milliseconds. We respond in under 50 milliseconds — four times faster.

Our backend runs in 300 plus cities worldwide. Automatic serverless scaling. Zero DevOps. Pay only for what we use.

---

## SLIDE 8: DESKTOP OAUTH (1 minute)

Here's something unique that sets us apart — Desktop Google OAuth with PKCE, which stands for Proof Key for Code Exchange.

The challenge: How do you do Google OAuth on a desktop app? Web apps have callback URLs. Mobile apps have deep links. But desktop apps? No native callback mechanism.

Most teams avoid this problem entirely. We solved it.

Our PKCE solution works like this: One, generate a secure code verifier. Two, open the real browser for Google login — no fake screens. Three, start a localhost HTTP server inside the app. Four, receive the callback and exchange securely. Five, show a success page in the browser.

Why does this matter?

It's secure — PKCE prevents token interception. Even if someone steals the auth code, they can't use it.

It's seamless — the user just clicks login. They see no technical complexity.

And it's unique — our competitors have NO desktop support. We do.

---

## SLIDE 9: REAL DATA (45 seconds)

LeoConnect isn't just a demo — it runs on real Leo MD 306 data.

We cover all 12 Districts. We've seeded over 90 clubs. More than 30 verified officials are already in the system. And our API latency is consistently under 50 milliseconds.

We've implemented a complete set of Core APIs: Authentication, User Profiles, Posts and Likes, Comments, Follow System.

Plus advanced Feature APIs: Events with RSVP, Clubs, Messages, Notifications, and Image Upload.

This is a complete ecosystem, not a partial prototype.

---

## SLIDE 10: JUDGING CRITERIA (1 minute)

We designed LeoConnect with the judging criteria in mind.

Functionality at 40 percent — the highest weight. We're feature-complete: Feed, Events, AI, Verified Accounts, and Direct Messages. All working.

Innovation at 30 percent — Kotlin Multiplatform, Cloudflare Edge computing, and secure PKCE Desktop OAuth. Real engineering innovation, not buzzwords.

Performance at 10 percent — Sub-50 millisecond latency, skeleton loading for smooth UX, R2 CDN for fast media delivery.

Scalability at 10 percent — Cloudflare auto-scaling, fully serverless architecture. This can handle growth beyond the competition.

Presentation at 10 percent — Real data. 12 districts. 90 plus clubs. Not mockups — reality.

Our key differentiators: 4 Platforms. Fastest Backend. AI Assistant.

---

## SLIDE 11: WHAT WE BUILT (1 minute)

Let me summarize what we've built.

Core Features: Feed plus Explore tabs. Multi-photo posts up to 4 images. Events with RSVP. Leo AI with Gemini 2.0 and RAG. Club and District discovery. User profiles and following. Real-time messaging. And Notifications.

Technical Excellence: 4 platforms from one codebase. Full Admin Dashboard in Vue.js. 30 plus verified officials. Search across posts, clubs, and districts. Double-tap to like. Haptic feedback. And rate limiting with security built in.

This isn't a prototype. LeoConnect is ready for production deployment across Leo MD 306.

---

## SLIDE 12: THANK YOU (30 seconds)

Thank you for your time.

We believe LeoConnect can truly make a difference for Leo clubs across Sri Lanka and the Maldives.

You can reach us at hello@rexosphere.com, or find our code on github.com/Rexosphere.

**[PAUSE - MAKE EYE CONTACT]**

We're ready for any questions.

---

# TOTAL TIME: ~17 minutes (with 7-minute video)
# WITHOUT VIDEO: ~10 minutes

---

# IF JUDGES ASK QUESTIONS:

**Q: How is this different from WhatsApp?**
WhatsApp is general-purpose. LeoConnect is Leo-specific — with club discovery, verified officials, event coordination, and an AI that understands Leo context. It's purpose-built for the movement.

**Q: Why Kotlin Multiplatform instead of Flutter?**
KMP gives us native performance with shared business logic. Flutter uses a rendering engine; KMP uses actual platform UI. For a social app with complex interactions, native feel matters.

**Q: Is the AI useful or just for show?**
Our AI uses RAG architecture — it retrieves from a Leo knowledge base before answering. It's not generic ChatGPT; it understands Leo terminology, districts, and processes.

**Q: How would you handle 4000+ users?**
Our Cloudflare Edge backend auto-scales serverlessly. We've already tested with seeded data and maintain under 50ms latency. The architecture is designed for growth.

**Q: Is this secure?**
Yes. We use OAuth 2.0 with PKCE for desktop — the recommended flow for public clients. Rate limiting prevents abuse. All API endpoints are protected.

---

*Good luck! 🦁*
