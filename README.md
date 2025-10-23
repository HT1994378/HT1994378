# Hi, I'm Hannah 👋

I build mobile and web apps. I'm drawn to problems that need solutions and I take particular care with UX and scalability. Until recently I've been building for fun and for improving my skillset. Now, I'm working on turning my latest project, OliveAI, into a startup business.

## What I Build

I build mobile and web applications across consumer social and B2B SaaS. My projects span youth safety tech, fandom communities, and AI-powered workplace tools.

**Current Focus:** OliveAI - Building a 24/7 AI workplace companion that bridges the gap between employees and HR through empathetic support and intelligent automation.

## Featured Projects

### 🤖 [OliveAI](https://github.com/HT1994378/oliveai) (In Development)
B2B workplace companion with mobile app for employees and web dashboard for HR. Live on TestFlight, awaiting App Store approval.
- AI-powered coaching, mediation, and escalation routing
- Company policy integration via Supabase
- Custom prompt engineering with intelligent classification system

#### Technical Approach
- Flutter mobile, AWS Amplify backend
- Claude API with custom prompt routing
- Supabase for policy storage, Parameter Store for prompts

### 🌍 [wrld](https://github.com/HT1994378/wrld)
Consumer social app creating custom digital spaces for fandoms.
- Modular architecture: Flutter shell pulling fandom-specific content from S3
- Built and deployed Harry Potter wrld as proof of concept

#### Technical Approach
- Flutter shell architecture
- Custom AWS: Cognito, AppSync, DynamoDB, GraphQL
- S3 for dynamic content delivery

### 👥 [SQUAD & SQUAD Parent](https://github.com/HT1994378/SQUAD)
Dual-app system for safer social media for young people with parental oversight.
- Age verification via Persona facial scanning
- Real-time content moderation using Sightengine
- Parental controls with usage insights and remote app freezing
  
#### Technical Approach
- Flutter with Firebase backend
- Persona, Sightengine, Spotify, Resend APIs

## Architecture Decisions I thought were interesting

**Keeping wrld lightweight:** Started by hardcoding the Harry Potter wrld, realized it wasn't scalable. Pivoted to a shell architecture where the Flutter app pulls wrld-specific content from S3.

**OliveAI's routing system:** Built a chat handler Lambda with a prompt router that uses keyword matching + sentiment analysis to channel requests into specialized pools. When confidence is <90%, it routes to me via Telegram for manual classification - deliberately high threshold during prompt engineering phase.

**SQUAD's safety layers:** Multi-tiered approach combining automated content moderation (Sightengine) with human review dashboard for edge cases. Parents can freeze the app instantly through Firebase.

## Let's Connect

I'm always up for collab talks or just to riff on whatever it is you're working on. Add me on Telegram @hannahkingswood.
