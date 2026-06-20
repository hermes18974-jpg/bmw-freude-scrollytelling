# BMW FREUDE — Scrollytelling Project
## Complete Pipeline Archive

**Created:** 2026-06-20  
**Concept:** FREUDE — A Scroll Through Time  
**Subject:** BMW 60-year history (1961 → 1970s → 2025+)  
**Pipeline:** Scrollytelling Website Pipeline v1.0

---

## PROJECT OVERVIEW

A BMW scrollytelling website where the user scrolls through 60 years of driving philosophy on one continuous alpine road. Three acts: The Awakening (1961), The Icon (1970s), The Silence (2025+). Scroll-driven canvas frame engine with GSAP ScrollTrigger + Lenis + frame interpolation.

## THE 7 STAGES EXECUTED

### Stage 1: Concept & Research
- Researched BMW design philosophy (monolithic design, Neue Klasse)
- Researched "Freude am Fahren" slogan history (60 years, born 1965)
- Researched BMW design DNA (Hofmeister kink, kidney grille, L-shaped taillights, Angel Eyes)
- Designed "one road through time" concept — same alpine pass, evolving light
- 3 acts: The Awakening (1961), The Icon (1970s), The Silence (2025+)

### Stage 2: Keyframe Images (GPT Image 2 via Codex auth)
- 3 keyframes generated at 1536×1024 (16:9 landscape)
- Same alpine pass in all 3: jagged Dolomite peak left, rounded dome right, valley center, stone bollards
- Act I: Golden dawn, BMW 1500 (9/10)
- Act II: Night, BMW E9 3.0 CS (9/10)  
- Act III: Electric blue dawn, Neue Klasse iX3 (8.5/10)

### Stage 3: Videos (Veo 3.1 Fast i2v via VicSee)
- 3 videos generated at 1080p, 8 seconds, 24fps
- Image-to-video: keyframe as first frame
- Act I: Slow dolly forward (40 credits)
- Act II: Crane up tracking shot (40 credits)
- Act III: Ground-level push-in (40 credits)
- Total: 120 credits

### Stage 4: Frame Extraction
- 576 frames extracted (192 per act, every frame at 24fps)
- Resolution: 960×540, JPEG quality 3
- Frame size: ~80-120KB each
- Total: ~52MB frames

### Stage 5: Development
- Single-file HTML (index.html)
- GSAP ScrollTrigger + Lenis + Canvas frame engine
- Frame interpolation with crossfade
- rAF render loop decoupled from scroll
- Progressive loading (Act 1 first, rest in background)
- 12 premium UI elements (custom cursor, sound toggle, nav dots, etc.)

### Stage 6: Optimization
- Video compression: 20MB → 2.4MB each (88% reduction)
- Keyframe compression: 1.8MB PNG → 188KB JPEG (90% reduction)
- Frame optimization: 960×540 q3 (~100KB each)
- CDN URL verification (caught Lenis 404 bug)

### Stage 7: Launch
- Cloudflare tunnel deployment
- Live preview URL
- (GitHub Pages permanent deployment pending)

## PROMPTS

See `prompts/` folder for all image and video prompts used.
## LIVE URL

**Tunnel (temporary):** https://vital-videos-selecting-skill.trycloudflare.com/
**GitHub Pages:** (pending permanent deployment)

## SKILL

The complete pipeline is saved as a Hermes skill: `scrollytelling-website-pipeline`
Location: `~/.hermes/skills/creative/scrollytelling-website-pipeline/SKILL.md`
Trigger: Next time anyone asks for a 'scrollytelling website', the skill auto-loads.
