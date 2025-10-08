# Sora 2 Prompt Playbook

> **Author:** N.Sachin Deshik  
> **Repository:** [SORA-2-PROMPTS](https://github.com/sachin-deshik-10/SORA-2-PROMPTS)

Welcome to the refreshed Sora 2 prompt collection. This playbook distills the strategies, structures, and ready-to-run prompts used throughout the SORA-2-PROMPTS project so you can iterate faster, brief collaborators with clarity, and ship polished video concepts in minutes instead of hours.

## Table of Contents

1. [Sora 2 at a Glance](#1-sora-2-at-a-glance)
2. [How to Use this Playbook](#2-how-to-use-this-playbook)
3. [Prompt Design Framework](#3-prompt-design-framework)
4. [Prompt Formula Cheat Sheet](#4-prompt-formula-cheat-sheet)
5. [Building Blocks Library](#5-building-blocks-library)
6. [Output Controls and Parameters](#6-output-controls-and-parameters)
7. [Troubleshooting & Iteration Loop](#7-troubleshooting--iteration-loop)
8. [Prompt Library](#8-prompt-library)
    - [Cinematic Story Worlds](#cinematic-story-worlds)
    - [Lifestyle & Travel Diaries](#lifestyle--travel-diaries)
    - [Product & Commercial Spots](#product--commercial-spots)
    - [Animation & Stylized Looks](#animation--stylized-looks)
    - [Experimental & Conceptual](#experimental--conceptual)
    - [Social-First Micro Formats](#social-first-micro-formats)
9. [Remix Matrix](#9-remix-matrix)
10. [Glossary of Sora 2 Terms](#10-glossary-of-sora-2-terms)
11. [License](#11-license)

---

## 1. Sora 2 at a Glance

Sora 2 introduces sharper temporal coherence, volumetric lighting controls, and smarter camera pathing. The highlights you should reference in prompts include:

- **Adaptive Scene Layouts** – The model now honors multi-room or multi-zone descriptions without merging props.
- **Dynamic Motion Curves** – Smooth camera arcs, glide-cam feels, and parallax-ready reveals are more consistent.
- **Audio-Aware Staging** – If you call out ambience or foley moments, Sora 2 frames them with matching kinetic energy.
- **Resolution Scaling** – 16:9 up to 4K, portrait 9:16, and ultrawide 21:9 behave predictably when you state the spec.
- **Persistent Character Slots** – Refer to characters with consistent identifiers (e.g., "Hero", "Mentor") to keep wardrobe and facial continuity.

Use these capabilities proactively. When the model understands the cinematic intent, it performs with far less trial and error.

---

## 2. How to Use this Playbook

1. **Pick a Track** – Choose the prompt category closest to your project.
2. **Scan the Framework** – Borrow the structure or formula that matches your story beat.
3. **Drop in Variables** – Replace placeholder descriptors ("[Hero]", "[City]") with concrete details.
4. **Control the Output** – Set duration, aspect ratio, and finishing notes in the output controls section of the prompt.
5. **Iterate with Notes** – After your first render, annotate what changed, adjust one lever at a time, and re-run.

Save each prompt iteration with the same identifier so version history stays tidy.

---

## 3. Prompt Design Framework

Structure prompts around the "VISION" model used in SORA-2-PROMPTS:

| Step | Focus | Questions to Answer |
|------|-------|---------------------|
| **V**isual Goal | Shot, movement, lighting | What does the viewer see first, second, third? |
| **I**mmersion Layer | Sound, texture, world rules | What sensory cues make the world feel alive? |
| **S**tory Beat | Conflict, objective, outcome | Why is this moment happening? |
| **I**nteractivity | Audience POV, overlays, callouts | How should the camera involve the viewer? |
| **O**utput Specs | Duration, aspect ratio, fps | Where will the video live? |
| **N**otes for Tweaks | Risks, failsafes, alternates | What should Sora avoid or emphasize? |

Write your prompt in blocks using this framework. It keeps instructions modular and easy to remix.

---

## 4. Prompt Formula Cheat Sheet

Combine the following template sections to create bulletproof Sora 2 prompts:

```text
[Title or Intent]

SCENE OPENER: [Establishing shot + setting + time of day].
CAMERA & MOTION: [Primary camera move + speed + focal length vibe].
SUBJECT & ACTION: [Character or object] [performing action] with [emotion or style].
DETAIL ENRICHMENT: [Lighting], [color palette], [set dressing], [atmospherics].
INTERACTIVE MOMENT: [POV shift / transition / effect] to reinforce [story beat].
OUTPUT CONTROLS: duration [X s], aspect ratio [format], resolution [HD/4K], aesthetic tag [references].
FAILSAFES: Avoid [undesired elements], keep [continuity cues].
```

Use all caps labels for readability; Sora ignores them, but your collaborators will love you for it.

### JSON Prompt Envelope

Sora 2 also parses structured prompts reliably when you wrap the same instructions inside a JSON envelope. Each prompt in this playbook now ships with the following structure:

```json
{
   "title": "Short identifier",
   "id": "unique_slug_for_tracking",
   "version": "2.0",
   "tags": ["category", "tone"],
   "prompt": {
      "scene_opener": "...",
      "camera": { "shot": "...", "motion": "...", "lens": "...", "motion_curve": "ease-in-out" },
      "subjects": [ { "id": "Hero", "action": "...", "emotion": "..." } ],
      "details": { "lighting": "...", "color_palette": "...", "texture": "...", "atmosphere": "..." },
      "audio": { "ambience": "...", "score": "..." },
      "interactive_moment": "Describe viewer POV or transition"
   },
   "output": {
      "duration_seconds": 20,
      "aspect_ratio": "21:9",
      "resolution": "UHD",
      "frame_rate": 24,
      "delivery": "mp4"
   },
   "negative_prompt": ["items to avoid"],
   "continuity": ["Objects or cues to keep consistent"],
   "notes": "Optional iteration reminders"
}
```

Copy the JSON directly into Sora or into your automation scripts; swap out the values to match your project while keeping the field names intact.

---

## 5. Building Blocks Library

### 5.1 Camera Shots

- Establishing drone wide, close-focus macro, rack-focus portrait, split-diopter medium, tableau frontal wide, vertigo dolly, pov chase, static symmetrical.

### 5.2 Camera Motion

- Drift dolly forward, crane drop reveal, handheld jitter, steady gimbal orbit, whip-pan handoff, light-speed zoom burst, glidecam hallway run, parallax truck.

### 5.3 Lighting & Atmosphere

- Neon rim lighting, volumetric sun shafts, overcast diffuse, candlelit chiaroscuro, arctic blue moonlight, dusty golden hour, fashion strobe pulses, projector patterns.

### 5.4 Texture & Materials

- Weathered concrete, vaporwave chrome, tactile linen, holographic glass, wet asphalt reflections, desert sandstone, mossy biome, liquid metal shimmer.

### 5.5 Audio & Mood Cues

- Sub-bass rumble, distant city heartbeat, analog tape hiss, festival crowd roar, winter wind choir, synth arpeggio scoring, minimal piano, underwater muffled ambience.

Drop these nouns into your prompts whenever you need an instant vibe upgrade.

---

## 6. Output Controls and Parameters

| Parameter | Options | Tips |
|-----------|---------|------|
| **Duration** | 6s, 12s, 20s, 30s | Mention "tight pacing" or "linger" to adjust tempo. |
| **Aspect Ratio** | 16:9, 9:16, 1:1, 21:9 | Describe composition ("centered", "rule-of-thirds") to avoid awkward cropping. |
| **Resolution** | HD (1080p), UHD (4K) | Pair with lighting clarity requests for crisp surfaces. |
| **Framerate Feel** | cinematic 24fps, hyperreal 60fps | Framerate language helps motion blur realism. |
| **Color Grade** | teal & orange, bleach bypass, technicolor, pastel film | Mention film stock or LUT for consistent mood. |
| **Creative Restrictions** | no text overlays, no logo morphing, keep props period-accurate | Stops Sora from hallucinating extras. |

Always place these notes near the end of your prompt to anchor the render settings.

---

## 7. Troubleshooting & Iteration Loop

1. **Assess** – Log what succeeded (e.g., lighting) versus what drifted (e.g., wardrobe).
2. **Target** – Adjust only one or two elements per revision so the model understands your priority.
3. **Rephrase** – Swap adjectives for precise film language ("dolly" instead of "move") when needed.
4. **Compare** – Keep side-by-side stills to ensure continuity across cuts.
5. **Lock** – When happy, duplicate the prompt and mark it "final" with the delivery format.

Keep a "prompt lab" folder with your top three variants per concept for quick retrieval.

---

## 8. Prompt Library

Every prompt below follows the playbook structure. Replace bracketed elements with your specifics and export directly to Sora 2.

### Cinematic Story Worlds

1. **Noir Alley Stand-off**

   ```text
   SCENE OPENER: rain-soaked 1940s alley at midnight, glistening cobblestones under neon signage.
   CAMERA & MOTION: slow dolly toward [Detective] holding an umbrella, 50mm lens feel.
   SUBJECT & ACTION: [Detective] confronts [Informer] trading a coded envelope, tension in their eyes.
   DETAIL ENRICHMENT: chiaroscuro lighting, cigarette smoke curling, vintage sedans idling with headlights flaring.
   INTERACTIVE MOMENT: whip-pan to reveal a hidden silhouette on the rooftop aiming a revolver.
   OUTPUT CONTROLS: duration 20s, aspect ratio 21:9, UHD, desaturated teal + amber grade.
   FAILSAFES: avoid futuristic props, keep wardrobe authentically 1940s.
   ```

2. **Solarpunk Rooftop Garden**

   ```text
   SCENE OPENER: sunrise over [City], lush rooftop farms cascading down terraced glass towers.
   CAMERA & MOTION: crane rise from botanical canopy to aerial wide, capturing shimmering solar panels.
   SUBJECT & ACTION: [Engineer] calibrates wind turbines while robotic pollinators swirl.
   DETAIL ENRICHMENT: luminescent vines, reflective water features, soft lens flares.
   INTERACTIVE MOMENT: POV shift through a transparent walkway revealing pedestrians below.
   OUTPUT CONTROLS: 16s, 16:9, 4K, vibrant pastel color grade.
   FAILSAFES: exclude dystopian pollution, keep tech biodegradable.
   ```

3. **Desert Caravan Revelation**

   ```text
   SCENE OPENER: golden hour dunes with long shadows, distant silhouettes of camel caravans.
   CAMERA & MOTION: sweeping drone arc transitioning to handheld close-up.
   SUBJECT & ACTION: [Archaeologist] unveils an ancient star map etched into obsidian.
   DETAIL ENRICHMENT: swirling dust motes, embroidered robes, metallic percussion hits.
   INTERACTIVE MOMENT: match cut to night sky aligning with the map's constellations.
   OUTPUT CONTROLS: 18s, 2.39:1, UHD, warm desert grade.
   FAILSAFES: avoid modern vehicles, keep props practical.
   ```

4. **Submerged City Awakening**

   ```text
   SCENE OPENER: underwater metropolis with bioluminescent architecture glowing turquoise.
   CAMERA & MOTION: glidecam swim-through following schools of translucent fish.
   SUBJECT & ACTION: [Researcher] activates a coral reactor igniting the city's power grid.
   DETAIL ENRICHMENT: rays of sunlight piercing water, holographic signs flickering, floating kelp banners.
   INTERACTIVE MOMENT: tilt up transitioning into star trail time-lapse.
   OUTPUT CONTROLS: 22s, 16:9, UHD, cool cyan-magenta palette.
   FAILSAFES: keep physics fluid, no surface waves within city limits.
   ```

5. **Victorian Time-Lattice**

   ```text
   SCENE OPENER: foggy 1890s London street where clocktower gears hover mid-air forming portals.
   CAMERA & MOTION: steadicam weave through pedestrians wearing copper goggles.
   SUBJECT & ACTION: [Inventor] tosses pocketwatch shards that freeze and rewind passing carriages.
   DETAIL ENRICHMENT: brass filigree, steam plumes, warm lamplight.
   INTERACTIVE MOMENT: dolly-zoom as a portal expands, revealing a mirror image of the street in daylight.
   OUTPUT CONTROLS: 24s, 4:3, UHD, sepia tint with subtle bloom.
   FAILSAFES: avoid digital screens, maintain period-accurate signage.
   ```

### Lifestyle & Travel Diaries

1. **Micro Cabin Morning**

   ```text
   SCENE OPENER: misty pine forest, micro cabin with panoramic window.
   CAMERA & MOTION: gentle dolly from coffee steam to sunrise panorama.
   SUBJECT & ACTION: [Creator] journals while kettle whistles, dog stretching nearby.
   DETAIL ENRICHMENT: warm wool textures, sunbeams, subtle vinyl crackle audio.
   INTERACTIVE MOMENT: POV of hands opening sliding door to reveal vast lake.
   OUTPUT CONTROLS: 15s, 16:9, 4K, cozy amber grade.
   FAILSAFES: avoid visible drones, keep atmosphere calm.
   ```

2. **Tokyo Night Cyclist**

   ```text
   SCENE OPENER: neon alley in Shinjuku during a drizzle, reflective pavement.
   CAMERA & MOTION: handheld follow-cam trailing [Cyclist] weaving through pedestrians.
   SUBJECT & ACTION: [Cyclist] delivers a flower bouquet with focused energy.
   DETAIL ENRICHMENT: holographic signage, ramen steam, bokeh tail lights.
   INTERACTIVE MOMENT: slow-motion drift around a turn, bouquet petals catching rain.
   OUTPUT CONTROLS: 12s, 9:16, UHD, punchy magenta-cyan grade.
   FAILSAFES: avoid signage in non-Japanese scripts, keep pace fluid.
   ```

3. **Mediterranean Rooftop Supper**

   ```text
   SCENE OPENER: twilight over terracotta rooftops, coastal breeze moving string lights.
   CAMERA & MOTION: crane down to table styled with tapas and clay ceramics.
   SUBJECT & ACTION: [Friends group] clinks glasses, laughter overlapping waves.
   DETAIL ENRICHMENT: olive trees, linen table runner, acoustic guitar ambience.
   INTERACTIVE MOMENT: rack focus to distant fireworks celebrating local festival.
   OUTPUT CONTROLS: 18s, 16:9, UHD, warm film grain.
   FAILSAFES: keep wardrobe casual modern, avoid heavy wind noise.
   ```

4. **Urban Sketcher Daybreak**

   ```text
   SCENE OPENER: sunrise over [City landmark], empty streets turning gold.
   CAMERA & MOTION: time-lapse tilt from sky to artist's sketchbook.
   SUBJECT & ACTION: [Sketcher] paints watercolor strokes translating skyline into abstract shapes.
   DETAIL ENRICHMENT: pigment puddles, light reflections, gentle busker piano.
   INTERACTIVE MOMENT: end card with question sticker space.
   OUTPUT CONTROLS: 14s, 4:5, 4K, soft pastel grade.
   FAILSAFES: avoid corporate logos, keep sketch legible.
   ```

5. **Sahara Star Camp**

   ```text
   SCENE OPENER: nocturnal desert glamping site with lanterns and dunes.
   CAMERA & MOTION: drone pull-back revealing galaxy above.
   SUBJECT & ACTION: [Traveler] sets telescope while narration notes constellations.
   DETAIL ENRICHMENT: embroidered rugs, ember fire pits, cool ambient scoring.
   INTERACTIVE MOMENT: tilt up transitioning into star trail time-lapse.
   OUTPUT CONTROLS: 16s, 21:9, UHD, deep blue grade.
   FAILSAFES: avoid city light pollution, keep camp minimal.
   ```

### Product & Commercial Spots

1. **Minimalist Smartwatch Reveal**

   ```text
   SCENE OPENER: matte white cyclorama with floating product pedestals.
   CAMERA & MOTION: robotic arm orbit around [Smartwatch] with macro focus.
   SUBJECT & ACTION: watch face lights up showcasing health metrics.
   DETAIL ENRICHMENT: soft specular highlights, vapor mist pulses to beats.
   INTERACTIVE MOMENT: transition to lifestyle clip of [Athlete] sprinting through tunnel.
   OUTPUT CONTROLS: 12s, 16:9, UHD, clean monochrome grade.
   FAILSAFES: avoid generic UI text, keep branding minimal.
   ```

2. **Artisan Coffee Dripper Launch**

   ```text
   SCENE OPENER: rustic kitchen studio, morning haze through windows.
   CAMERA & MOTION: top-down to 45° tilt as water spirals through dripper.
   SUBJECT & ACTION: close-up of bloom phase, steam swirling.
   DETAIL ENRICHMENT: walnut counter, linen towels, analog scale beeps.
   INTERACTIVE MOMENT: insert overlay showing flavor notes.
   OUTPUT CONTROLS: 14s, 16:9, UHD, warm cinematic LUT.
   FAILSAFES: avoid plastic accessories, keep pour smooth.
   ```

3. **Electric Car Pop-Up**

   ```text
   SCENE OPENER: futuristic pop-up showroom in city plaza.
   CAMERA & MOTION: jib down to car exterior, neon grid reflections.
   SUBJECT & ACTION: [Driver] taps start, headlights ripple like aurora.
   DETAIL ENRICHMENT: kinetic LED floor, minimal crowd, soundtrack of synth pulses.
   INTERACTIVE MOMENT: match cut to highway drive during sunset.
   OUTPUT CONTROLS: 20s, 21:9, UHD, cool-silver grade.
   FAILSAFES: avoid racing behavior, keep signage bilingual English/Metric.
   ```

4. **Wellness App Storyboard**

   ```text
   SCENE OPENER: airy apartment, morning yoga mat laid out.
   CAMERA & MOTION: handheld follow of [User] opening app.
   SUBJECT & ACTION: UI projection floats mid-air showing personalized routine.
   DETAIL ENRICHMENT: indoor plants, sun-kissed textures, subtle drop shadows.
   INTERACTIVE MOMENT: over-the-shoulder view of breathing exercise animation.
   OUTPUT CONTROLS: 15s, 9:16, UHD, pastel gradient grade.
   FAILSAFES: keep fonts sans-serif, avoid cluttered overlays.
   ```

5. **Luxury Fragrance Atmosphere**

   ```text
   SCENE OPENER: dramatic black void with hanging crystal prisms.
   CAMERA & MOTION: slow-motion dolly through prisms to perfume bottle pedestal.
   SUBJECT & ACTION: liquid mist envelops bottle while gold particles swirl.
   DETAIL ENRICHMENT: harp glissando, deep bass hits, reflective floor.
   INTERACTIVE MOMENT: flash cuts to sensory memories—ocean cliff, velvet lounge.
   OUTPUT CONTROLS: 18s, 16:9, 4K, high-contrast noir grade.
   FAILSAFES: avoid literal flowers, keep vibe mysterious.
   ```

### Animation & Stylized Looks

1. **Cel-Shaded Arcade Chase**

   ```text
   SCENE OPENER: retro arcade city rendered in cel-shaded neon.
   CAMERA & MOTION: kinetic follow-cam behind pixelated hoverboarder.
   SUBJECT & ACTION: [Hero] dodges voxel obstacles, sparks flying.
   DETAIL ENRICHMENT: scanline overlays, synthwave score, HUD elements.
   INTERACTIVE MOMENT: 2D-to-3D flip as camera swings to side profile.
   OUTPUT CONTROLS: 16s, 16:9, UHD, vivid magenta-blue palette.
   FAILSAFES: maintain consistent cel lines, avoid realism.
   ```

2. **Stop-Motion Forest Spirits**

   ```text
   SCENE OPENER: handcrafted woodland set with felt trees.
   CAMERA & MOTION: incremental push-in mimicking stop-motion cadence.
   SUBJECT & ACTION: clay spirit creatures light lanterns.
   DETAIL ENRICHMENT: tactile textures, miniature fog, xylophone chimes.
   INTERACTIVE MOMENT: overhead shot revealing constellations shaped like leaves.
   OUTPUT CONTROLS: 18s, 4:3, UHD, warm analog grain.
   FAILSAFES: avoid smooth interpolation, keep motion deliberately jerky.
   ```

3. **Studio Ghibli Homage Train Ride**

   ```text
   SCENE OPENER: watercolor countryside with floating pollen.
   CAMERA & MOTION: lateral tracking shot following vintage train.
   SUBJECT & ACTION: [Protagonist child] gazes out window, cheeks puffed with wonder.
   DETAIL ENRICHMENT: whimsical creatures in fields, soft orchestral swell.
   INTERACTIVE MOMENT: interior cabin shifts to dream realm with gentle color shift.
   OUTPUT CONTROLS: 20s, 16:9, 4K, pastel watercolor grade.
   FAILSAFES: avoid technology beyond 1950s, maintain painterly edges.
   ```

4. **Vector Pop Infographic**

   ```text
   SCENE OPENER: bold flat-color background with geometric shapes.
   CAMERA & MOTION: simulated swipe transitions left to right.
   SUBJECT & ACTION: each card features minimal animation, supporting b-roll in picture-in-picture.
   DETAIL ENRICHMENT: branded icon set, subtle drop shadows, per-card sound cue.
   INTERACTIVE MOMENT: final card CTA "SAVE FOR LATER" with arrow down.
   OUTPUT CONTROLS: 10s, 1:1, 4K, vibrant pop-art palette.
   FAILSAFES: avoid gradients, keep icons consistent thickness.
   ```

5. **Ink Wash Duel**

   ```text
   SCENE OPENER: parchment backdrop with sumi-e brush strokes forming mountains.
   CAMERA & MOTION: swirling ink transitions from wide landscape to duel close-up.
   SUBJECT & ACTION: two samurai silhouettes clash, strokes splattering dynamically.
   DETAIL ENRICHMENT: ink droplets, subtle shakuhachi flute.
   INTERACTIVE MOMENT: freeze-frame brush stamp sealing scene.
   OUTPUT CONTROLS: 14s, 21:9, UHD, monochrome with crimson accents.
   FAILSAFES: avoid modern weapons, keep brushwork organic.
   ```

### Experimental & Conceptual

1. **Gravity Reversal Atrium**

   ```text
   SCENE OPENER: minimalist museum atrium where sculptures float upward.
   CAMERA & MOTION: inverted crane shot rotating 180° mid-sequence.
   SUBJECT & ACTION: visitors walk on ceiling while hair flows downward.
   DETAIL ENRICHMENT: ambient choir, refracted sunlight, particle dust.
   INTERACTIVE MOMENT: camera passes through mirrored floor revealing alternate physics.
   OUTPUT CONTROLS: 16s, 16:9, 4K, cool minimal palette.
   FAILSAFES: avoid comedic tone, keep faces serene.
   ```

2. **Data Bloom Metaverse**

   ```text
   SCENE OPENER: endless black expanse with blooming voxels representing data clusters.
   CAMERA & MOTION: orbit around central sphere emitting aurora streams.
   SUBJECT & ACTION: avatars sculpt data into living garden forms.
   DETAIL ENRICHMENT: glitched particle trails, binaural blips.
   INTERACTIVE MOMENT: first-person dive into data bloom, macroscale fractals.
   OUTPUT CONTROLS: 18s, 16:9, 4K, iridescent gradient.
   FAILSAFES: avoid corporate branding, keep avatars androgynous.
   ```

3. **Time-Lapse Origami City**

   ```text
   SCENE OPENER: blank table that rapidly folds into skyline.
   CAMERA & MOTION: overhead hyperlapse peppered with snap-zoom to key pieces.
   SUBJECT & ACTION: paper vehicles glide through origami streets.
   DETAIL ENRICHMENT: crisp paper textures, tactile folding sounds.
   INTERACTIVE MOMENT: camera dives into a single paper window revealing bustling office.
   OUTPUT CONTROLS: 12s, 16:9, UHD, high-contrast white + accent color.
   FAILSAFES: no human hands present, keep origami precise.
   ```

4. **Aurora Choir Installation**

   ```text
   SCENE OPENER: Arctic cliffside stage with vertical light pillars synced to vocals.
   CAMERA & MOTION: sweeping drone capturing choir silhouettes against aurora.
   SUBJECT & ACTION: voices crescendo, light pillars respond in choreography.
   DETAIL ENRICHMENT: frost particles, ethereal harmony, flowing fabrics.
   INTERACTIVE MOMENT: camera enters light pillar, revealing abstract soundwave tunnel.
   OUTPUT CONTROLS: 20s, 21:9, UHD, cool spectrum grade.
   FAILSAFES: avoid city intrusions, keep tech elegant.
   ```

5. **Quantum Lab Dreamscape**

   ```text
   SCENE OPENER: futuristic lab where chalkboard equations manifest as holograms.
   CAMERA & MOTION: steadicam weaving through suspended formulas.
   SUBJECT & ACTION: [Physicist] plucks equation out of air, converting into mini-universe bubble.
   DETAIL ENRICHMENT: shimmer particles, ambient synth pads, reflective floor.
   INTERACTIVE MOMENT: macro close-up inside bubble showing galaxies birthing.
   OUTPUT CONTROLS: 22s, 16:9, UHD, ultraviolet neon grade.
   FAILSAFES: avoid cluttered wires, keep tone elegant.
   ```

### Social-First Micro Formats

1. **5-Second Hook Reel**

   ```text
   SCENE OPENER: bold typography "WAIT FOR IT" in kinetic type.
   CAMERA & MOTION: snap-zoom onto [Headline moment].
   SUBJECT & ACTION: [Creator] triggers unexpected reveal (e.g., color-change jacket).
   DETAIL ENRICHMENT: quick whoosh sfx, bright key lighting, stacked text overlays.
   INTERACTIVE MOMENT: split-second freeze with CTA arrow pointing to caption.
   OUTPUT CONTROLS: 6s, 9:16, 1080x1920, saturated punchy grade.
   FAILSAFES: keep text within safe margins, avoid slow intro.
   ```

2. **Side-by-Side Transformation**

   ```text
   SCENE OPENER: screen split in half, left "BEFORE", right "AFTER".
   CAMERA & MOTION: static tripod with subtle push-in over time.
   SUBJECT & ACTION: [Room makeover / outfit change] transitions via match cuts.
   DETAIL ENRICHMENT: overlay progress labels, upbeat clap track.
   INTERACTIVE MOMENT: mid-sequence time-lapse acceleration to highlight effort.
   OUTPUT CONTROLS: 12s, 9:16, HD, clean modern grade.
   FAILSAFES: avoid jitter, keep labels minimal.
   ```

3. **Captioned Mini-Doc**

   ```text
   SCENE OPENER: bold caption ribbon introducing topic.
   CAMERA & MOTION: mix of b-roll establishing shots and direct-to-camera vlog segments.
   SUBJECT & ACTION: [Subject] shares key insight while overlay infographics animate.
   DETAIL ENRICHMENT: subtitles in branded colors, gentle ambient bed.
   INTERACTIVE MOMENT: end card with question sticker space.
   OUTPUT CONTROLS: 30s, 9:16, UHD, editorial neutral grade.
   FAILSAFES: keep subtitles high-contrast, avoid fast pans.
   ```

4. **Looping Food Boomerang**

   ```text
   SCENE OPENER: macro of [Dish] being plated.
   CAMERA & MOTION: high-speed capture loop reversed seamlessly.
   SUBJECT & ACTION: sauce drizzle arcs mid-air then rewinds.
   DETAIL ENRICHMENT: sizzling audio, warm highlights, sparkling toppings.
   INTERACTIVE MOMENT: text overlay "REPLAY" synced to loop.
   OUTPUT CONTROLS: 8s, 1:1, UHD, rich warm grade.
   FAILSAFES: ensure loop seam invisible, avoid messy backdrop.
   ```

5. **Quick Tip Carousel**

   ```text
   SCENE OPENER: card 1 with bold headline "3 TIPS TO [Goal]".
   CAMERA & MOTION: simulated swipe transitions left to right.
   SUBJECT & ACTION: each card features minimal animation, supporting b-roll in picture-in-picture.
   DETAIL ENRICHMENT: branded icon set, subtle drop shadows, per-card sound cue.
   INTERACTIVE MOMENT: final card CTA "SAVE FOR LATER" with arrow down.
   OUTPUT CONTROLS: 15s, 4:5, HD, clean pastel palette.
   FAILSAFES: maintain padding, avoid complex backgrounds.
   ```

---

## 9. Remix Matrix

Use this grid to cross-pollinate ideas. Pick one item from each column for instant variations.

| Mood | Camera Move | Palette | Texture | Hook |
|------|-------------|---------|---------|------|
| hopeful dawn | orbit reveal | sunrise pastels | brushed metal | whispered narration |
| high-energy | whip-pan relay | neon electric | iridescent fabric | jump-cut typography |
| meditative | slow dolly inward | muted earth tones | natural wood | ASMR sound design |
| dramatic noir | crane drop | silver & shadow | rain-soaked surfaces | lightning strike |
| surreal dream | floating POV | ultraviolet glow | liquid glass | reverse-motion reveal |

Combine rows: e.g., "meditative + slow dolly inward + muted earth tones + natural wood + ASMR" to spin up spa or mindfulness visuals.

---

## 10. Glossary of Sora 2 Terms

- **Temporal Pinning** – Language that keeps character outfits and props locked between cuts.
- **Motion Curve** – Descriptor for acceleration profile (e.g., "ease-in, whip-out").
- **Atmos Layer** – The ambient particles, fog, or rain you request to boost depth cues.
- **Continuity Anchor** – An object or gesture repeated so Sora maintains scene logic.
- **Prompt Capsule** – A saved template with annotated swap-in variables for your team.

Keep these references handy when communicating with collaborators.

---

## 11. License

This playbook is shared under the Creative Commons Attribution-ShareAlike 4.0 International License. Remix it, credit **N.Sachin Deshik**, and link back to the [SORA-2-PROMPTS repository](https://github.com/sachin-deshik-10/SORA-2-PROMPTS) so the community can keep improving it.
