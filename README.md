# Kornél Varga

**AI Automation Engineer.** I build voice agents, CRMs and the automations between them, and I ship them to production myself.

Hungarian, based in the Netherlands. Open to remote roles across the EU, or on site in Budapest.

**[kornelvarga.com](https://kornelvarga.com)** · [LinkedIn](https://www.linkedin.com/in/kornel-varga-430005227/) · [varga.kornel03@gmail.com](mailto:varga.kornel03@gmail.com)

> **Skip the CV, call my AI:** +31 970 0653 3490. It's an agent I built that knows my work and can book a call with me. You can also [talk to it in the browser](https://kornelvarga.com).

## What these repos are

Everything here runs **VargaFlow**, a marketing and automation system for home service contractors (plumbers, roofers, HVAC). I built it and I run it alone, around a full-time job. It isn't a demo: over 11,000 real messages have gone out through it.

| Repo | What it is | Commits |
|---|---|---|
| [ai-voice-receptionist](https://github.com/kornelvarga1/ai-voice-receptionist) | AI phone receptionists on Retell + Twilio: one prompt template and a config per business, emergency triage with a safety carve-out, real Google Calendar booking. [Call a demo line](https://kornelvarga.com#demos) | clean public copy |
| [vargaflow-admin](https://github.com/kornelvarga1/vargaflow-admin) | The CRM and automation engine: pipeline, SMS/email sequences from a cron-driven queue, two-way inbox with an AI text agent, browser calling, self-built booking on Google Calendar | 291 |
| [vargaflow-client](https://github.com/kornelvarga1/vargaflow-client) | The multi-tenant app contractors use: their customers, messaging, browser calling, review requests, referral follow-ups, missed-call text-back | 232 |
| [vargaflow-website](https://github.com/kornelvarga1/vargaflow-website) | The lead-gen site, prerendered for search, with forms that feed straight into the CRM's automations | 257 |
| [contractor-website-template](https://github.com/kornelvarga1/contractor-website-template) | One codebase that builds a separate website per client from a config file | 101 |

## In production

Counted from the production database, March to September 2026:

- **11,000+ SMS sent** through the queue, **600+ replies** handled in the two-way inbox
- **~6,000 contacts** in the pipeline
- **600+ messages held back** by quiet-hours rules and **280+ numbers** suppressed on the do-not-contact list, enforced at send time
- **57 edge functions** handling webhooks from Twilio, Retell and Google, scheduled jobs and the message queue

## Stack

**Voice:** Retell AI, ElevenLabs, SIP trunking · **Telephony:** Twilio Voice and SMS, A2P 10DLC · **Backend:** Supabase, PostgreSQL with row-level security, Deno edge functions · **Frontend:** React, TypeScript, Vite, Tailwind · **Deploys:** Vercel

## How I work

I wrote my first line of code in March 2026 and I build with AI coding tools, heavily and on purpose. That's how one person shipped all of this in six months. What I bring is the judgement: what to build, which trade-off to take, when something is wrong, and getting it live in front of real users. The commit history is public, including the fixes. I'm happy to walk through any of it.
