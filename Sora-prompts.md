# Sora 2 Prompt Playbook

> **Author:** N.Sachin Deshik  
> **Repository:** [SORA-2-PROMPTS](https://github.com/sachin-deshik-10/SORA-2-PROMPTS)

Welcome to the refreshed Sora 2 prompt collection. This playbook distills the strategies, structures, and ready-to-run prompts used throughout the SORA-2-PROMPTS project so you can iterate faster, brief collaborators with clarity, and ship polished video concepts in minutes instead of hours.

## 8. Prompt Library

Every prompt below is delivered in production-ready JSON. Swap out values inside the objects while keeping keys intact for smooth automation with Sora 2.

### Cinematic Story Worlds

```json
[
   {
      "title": "Noir Alley Stand-off",
      "id": "cinematic_noir_alley_standoff_v2",
      "version": "2.1",
      "tags": ["cinematic", "noir", "thriller", "night"],
      "prompt": {
         "scene_opener": "Rain-soaked 1940s alley at midnight; neon kanji reflections ripple across slick cobblestones while steam vents breathe in the background.",
         "camera": {
            "shot": "over-the-shoulder medium resolving into extreme close-up",
            "motion": "steadicam dolly-in with 12-degree arc sweep",
            "lens": "50mm anamorphic with soft halation filters",
            "sensor": "full-frame, f/1.8 depth of field",
            "movement_speed": "0.4 m/s",
            "motion_curve": "ease-in with 1-second hold at apex",
            "stabilization": "optical steady with 10% handheld jitter overlay"
         },
         "subjects": [
            {
               "id": "Detective",
               "description": "weathered private eye beneath black umbrella",
               "action": "extends coded envelope toward Informer while thumb flicks lighter flame",
               "emotion": "controlled fury",
               "wardrobe": "charcoal trenchcoat, pinstriped suit, fedora, leather gloves"
            },
            {
               "id": "Informer",
               "description": "nervous informant leaning against brick wall",
               "action": "accepts envelope with trembling hand while glancing upward",
               "emotion": "paranoid dread",
               "wardrobe": "damp tweed jacket, wool cap, loosened tie"
            },
            {
               "id": "Sniper",
               "description": "silhouetted figure perched on rooftop water tower",
               "action": "tracks encounter through scope, finger tightening on trigger",
               "emotion": "cold focus",
               "wardrobe": "matte-black tactical coat"
            }
         ],
         "details": {
            "lighting": "split-contrast sodium vapor mixed with cool cyan rim; hard backlight from headlights",
            "color_palette": "desaturated teals, amber highlights, deep obsidian blacks",
            "set_dressing": "puddles, vintage sedans with headlights, steam grates, neon bar signage flicker",
            "atmosphere": "steady drizzle with drifting cigarette smoke layers",
            "textures": "wet cobblestone glints, worn brick, reflective puddles, misty air"
         },
         "audio": {
            "ambience": "distant thunder rolls, gutter rainfall, occasional tire hiss",
            "score": "low brass noir motif with brushed snare rhythm",
            "foley": "lighter flick, umbrella drips, sniper bolt click"
         },
         "interactive_moment": "Whip-pan reveal to rooftop sniper at 12s with 18-degree tilt, then snap back to close-up of Detective's eyes."
      },
      "effects": {
         "transitions": "2-frame match cut between whip-pan and reaction shot",
         "speed_ramp": "5% slow-down during envelope hand-off",
         "post": "grain overlay level 35, subtle bloom on highlights"
      },
      "output": {
         "duration_seconds": 20,
         "aspect_ratio": "21:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes HQ",
         "render_style": "cinematic_film_noir"
      },
      "negative_prompt": [
         "modern vehicles",
         "daylight leaks",
         "cartoonish expressions",
         "text overlays"
      ],
      "continuity": [
         "Detective umbrella position maintained across cuts",
         "rain intensity constant",
         "neon signage flicker frequency locked"
      ],
      "notes": "If Sora over-saturates, phrase palette as 'muted cyan with amber highlights only'."
   },
   {
      "title": "Solarpunk Rooftop Garden",
      "id": "cinematic_solarpunk_rooftop_garden_v2",
      "version": "2.1",
      "tags": ["cinematic", "solarpunk", "utopian", "sunrise"],
      "prompt": {
         "scene_opener": "Sunrise over biophilic megacity with terraced rooftop farms cascading down glass towers and morning mist lifting.",
         "camera": {
            "shot": "aerial establishing that settles into crane-descend hero framing",
            "motion": "crane drop from 40m altitude transitioning into glidecam sidestep",
            "lens": "24mm rectilinear wide",
            "sensor": "super35, T-stop 2.8",
            "movement_speed": "variable 1.2 m/s to 0.6 m/s",
            "motion_curve": "ease-out with subtle sinusoidal hover",
            "stabilization": "drone gimbal, horizon lock"
         },
         "subjects": [
            {
               "id": "Engineer",
               "description": "young sustainability engineer with augmented reality visor",
               "action": "calibrates wind micro-turbines while issuing hand-gesture commands",
               "emotion": "optimistic focus",
               "wardrobe": "recycled fiber jumpsuit with luminescent seams"
            },
            {
               "id": "PollinatorBots",
               "description": "hummingbird-sized robotics with shimmering wings",
               "action": "spiral around vertical gardens dispersing pollen",
               "emotion": "n/a",
               "wardrobe": "biopolymer chassis with daylight collectors"
            }
         ],
         "details": {
            "lighting": "golden-hour volumetric shafts breaking through dew haze",
            "color_palette": "fresh greens, warm sunrise gold, polished copper accents",
            "set_dressing": "hydroponic towers, solar leaves, reclaimed wood walkways, water channels",
            "atmosphere": "floating pollen motes, gentle mist, lens flares",
            "textures": "leaf microstructures, glass reflections, recycled composite panels"
         },
         "audio": {
            "ambience": "soft city hum, wind turbines, distant morning commuters",
            "score": "uplifting strings blended with modular synth pads",
            "foley": "bot wing flutter, tablet taps, gentle footsteps"
         },
         "interactive_moment": "POV visor overlay appears at 11s highlighting energy metrics, then camera passes through transparent walkway revealing pedestrians below."
      },
      "effects": {
         "transitions": "lambert crossfade from aerial to engineer close-up",
         "speed_ramp": "8% slow-mo during AR data burst",
         "post": "subtle anamorphic flare, mild chromatic aberration on edges"
      },
      "output": {
         "duration_seconds": 16,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "H.265 high profile",
         "render_style": "solarpunk_pastel"
      },
      "negative_prompt": [
         "pollution haze",
         "industrial smokestacks",
         "crowded traffic",
         "text labels outside AR overlay"
      ],
      "continuity": [
         "sun position locked at low horizon",
         "bot wing glow consistent",
         "AR interface uses teal glyph set"
      ],
      "notes": "If the walkway feels empty, request 'include two pedestrians in soft linen suits crossing bridge at 9s'."
   },
   {
      "title": "Desert Caravan Revelation",
      "id": "cinematic_desert_caravan_revelation_v2",
      "version": "2.1",
      "tags": ["cinematic", "adventure", "desert", "dusk"],
      "prompt": {
         "scene_opener": "Golden hour dunes stretching to horizon with long camel shadows etching patterns into sand ridges.",
         "camera": {
            "shot": "sweeping drone wide collapsing into handheld medium",
            "motion": "aerial arc at 35m radius descending to ground-level shoulder cam",
            "lens": "35mm prime with slight tele compression",
            "sensor": "full-frame, f/4 for layered depth",
            "movement_speed": "drone 4 m/s, handheld 0.6 m/s",
            "motion_curve": "arc ease-in, handheld natural sway",
            "stabilization": "gyro smoothing on drone, subtle handheld jitter preserved"
         },
         "subjects": [
            {
               "id": "Archaeologist",
               "description": "sunburned explorer with sand-scarred satchel",
               "action": "brushes sand from obsidian star map revealing glowing inlays",
               "emotion": "quiet awe",
               "wardrobe": "linen tunic, leather belts, protective goggles perched on head"
            },
            {
               "id": "Caravan",
               "description": "camel line cresting dune ridge",
               "action": "paces slowly with bells chiming, riders silhouetted",
               "emotion": "resolute",
               "wardrobe": "embroidered desert cloaks, patterned scarves"
            }
         ],
         "details": {
            "lighting": "low-angle amber sun casting elongated shadows, bounce from sand",
            "color_palette": "burnt orange, copper, deep indigo accents",
            "set_dressing": "half-buried ruins, meteorite shards, fluttering prayer flags",
            "atmosphere": "gentle sand motes, heat shimmer along horizon",
            "textures": "grainy sand ridges, polished obsidian, weathered fabric"
         },
         "audio": {
            "ambience": "wind brushing dunes, distant camel grunts, faint chimes",
            "score": "ethnic strings with cinematic percussion swells",
            "foley": "brush scraping stone, sand sliding, map clicking into alignment"
         },
         "interactive_moment": "Match cut from star map glowing lines to celestial night sky overlaying same pattern at 14s."
      },
      "effects": {
         "transitions": "match dissolve with luminance mask",
         "speed_ramp": "gentle 20% slow-mo during revelation moment",
         "post": "additive glow on star map etchings"
      },
      "output": {
         "duration_seconds": 18,
         "aspect_ratio": "2.39:1",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes LT",
         "render_style": "epic_adventure"
      },
      "negative_prompt": [
         "modern vehicles",
         "overexposed highlights",
         "storm-level wind",
         "text captions"
      ],
      "continuity": [
         "camel bell rhythm stays constant",
         "sun angle locked to golden hour",
         "obsidian map glows cobalt when fully exposed"
      ],
      "notes": "If dunes feel sparse, add 'distant mirage of ancient city shimmering on horizon at 17s'."
   },
   {
      "title": "Submerged City Awakening",
      "id": "cinematic_submerged_city_awakening_v2",
      "version": "2.1",
      "tags": ["cinematic", "sci-fi", "underwater", "bioluminescent"],
      "prompt": {
         "scene_opener": "Bioluminescent underwater metropolis; coral skyscrapers pulse turquoise against abyssal backdrop while manta-shaped trains glide along light rails.",
         "camera": {
            "shot": "immersive glide wide transitioning to medium close on reactor console",
            "motion": "neutrally buoyant glidecam with gentle S-curve path and 30-degree roll at midpoint",
            "lens": "18mm spherical dome port",
            "sensor": "full-frame, f/2.8 with focus breathing compensation",
            "movement_speed": "0.8 m/s",
            "motion_curve": "smooth constant velocity with slight ease-out near reactor",
            "stabilization": "hydrodynamic stabilization, zero jitter"
         },
         "subjects": [
            {
               "id": "Researcher",
               "description": "aquatic engineer in streamlined exosuit with illuminated glyphs",
               "action": "interfaces with coral reactor nodes, triggering cascading light pulses",
               "emotion": "confident wonder",
               "wardrobe": "iridescent exosuit, transparent helmet with HUD"
            },
            {
               "id": "CoralReactor",
               "description": "organic energy core grown from branching coral spires",
               "action": "awakens sequentially, sending power conduits across city",
               "emotion": "n/a",
               "wardrobe": "n/a"
            },
            {
               "id": "TransitStingray",
               "description": "manta-shaped public transport craft",
               "action": "passes overhead leaving bioluminescent wake",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "cool cyan bioluminescence with magenta accent pulses, crepuscular rays filtering from surface",
            "color_palette": "turquoise, indigo, magenta highlights",
            "set_dressing": "floating kelp banners, holographic signage, air bubble plazas",
            "atmosphere": "suspended particulate shimmer, gentle current sway",
            "textures": "porous coral, glass bubble domes, metallic conduits, fish scales"
         },
         "audio": {
            "ambience": "muffled ocean currents, distant whale calls, reactor hum",
            "score": "ethereal synth choir with sub bass swells",
            "foley": "HUD blips, water displacement, reactor resonance"
         },
         "interactive_moment": "Camera rolls 30 degrees following TransitStingray at 13s before snapping to Researcher's visor reflection of the awakening grid."
      },
      "effects": {
         "transitions": "light bloom wipe as reactor ignites",
         "speed_ramp": "brief 10% speed-up when stingray passes to convey momentum",
         "post": "biolumens enhanced with glow radius 0.3, add micro bubbles"
      },
      "output": {
         "duration_seconds": 22,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 30,
         "delivery": "H.265 10-bit",
         "render_style": "aquatic_scifi"
      },
      "negative_prompt": [
         "surface waves inside city",
         "murky visibility",
         "terrestrial wildlife",
         "text captions"
      ],
      "continuity": [
         "bioluminescent pulse cadence remains synchronized across shots",
         "Researcher HUD glyph color stays teal",
         "bubbles flow upward consistently"
      ],
      "notes": "If Sora darkens the reactor, add 'ensure reactor emits soft core light at 5000K'."
   },
   {
      "title": "Victorian Time-Lattice",
      "id": "cinematic_victorian_time_lattice_v2",
      "version": "2.1",
      "tags": ["cinematic", "steampunk", "period", "foggy"],
      "prompt": {
         "scene_opener": "Fog-cloaked 1890s London street where clocktower gears hover mid-air forming shimmering temporal portals above gas lamps.",
         "camera": {
            "shot": "steadicam weave wide slipping into dolly-zoom hero frame",
            "motion": "ground-level glide weaving between pedestrians with closing dolly push",
            "lens": "32mm anamorphic",
            "sensor": "full-frame, f/2.4",
            "movement_speed": "0.7 m/s",
            "motion_curve": "sinusoidal sway synced with hovering gears",
            "stabilization": "gyro-stabilized with slight mechanical wobble"
         },
         "subjects": [
            {
               "id": "Inventor",
               "description": "eccentric technologist wielding copper gauntlet",
               "action": "tosses pocketwatch shards upward, freezing and rewinding carriages",
               "emotion": "electrified curiosity",
               "wardrobe": "velvet waistcoat, brass goggles, patterned cravat"
            },
            {
               "id": "CarriageDriver",
               "description": "coachman startled beside suspended horses",
               "action": "reaches toward frozen reins",
               "emotion": "astonished confusion",
               "wardrobe": "tweed coat, leather gloves"
            }
         ],
         "details": {
            "lighting": "warm gas lamps mixed with cool portal glow",
            "color_palette": "sepia browns, brass highlights, teal time-energy",
            "set_dressing": "cobblestone street, newsboys, steam pipes, floating gear arrays",
            "atmosphere": "dense fog, occasional steam bursts, drifting soot",
            "textures": "patinated brass, wet stone, wool fabrics"
         },
         "audio": {
            "ambience": "steam hiss, distant church bells, horse snorts",
            "score": "clockwork ticking polyrhythm layered with strings",
            "foley": "gear clacks, portal hum, buckle jingles"
         },
         "interactive_moment": "Dolly-zoom at 16s as portal blossoms, revealing mirror daytime street inside lattice."
      },
      "effects": {
         "transitions": "time-slice ripple between frozen and rewound states",
         "speed_ramp": "reverse ramp on pocketwatch shards mid-air",
         "post": "add volumetric fog density 0.6, chromatic aberration on portal edges"
      },
      "output": {
         "duration_seconds": 24,
         "aspect_ratio": "4:3",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "steampunk_period"
      },
      "negative_prompt": [
         "electronic displays",
         "modern streetlights",
         "plastic materials",
         "anachronistic vehicles"
      ],
      "continuity": [
         "fog density consistent",
         "Inventor gauntlet glow amber",
         "portal gear rotation counter-clockwise"
      ],
      "notes": "If pedestrians vanish, add 'background extras in layered Victorian attire crossing frame left to right'."
   }
]
```

### Lifestyle & Travel Diaries

```json
[
   {
      "title": "Micro Cabin Morning",
      "id": "lifestyle_micro_cabin_morning_v2",
      "version": "2.1",
      "tags": ["lifestyle", "cozy", "forest", "sunrise"],
      "prompt": {
         "scene_opener": "Mist-laden pine forest enveloping micro cabin with floor-to-ceiling panoramic window and slow sunrise bloom.",
         "camera": {
            "shot": "intimate macro-to-wide push",
            "motion": "dolly slides from steaming mug to reveal panoramic window view",
            "lens": "35mm macro shifting to 24mm wide",
            "sensor": "full-frame, f/2.0 near, f/4 wide",
            "movement_speed": "0.5 m/s",
            "motion_curve": "ease-in then ease-out",
            "stabilization": "slider with micro-jitter suppressed"
         },
         "subjects": [
            {
               "id": "Creator",
               "description": "content creator journaling at wooden desk",
               "action": "writes slow strokes, pauses to inhale cabin air",
               "emotion": "calm gratitude",
               "wardrobe": "cream knit sweater, wool socks"
            },
            {
               "id": "CompanionDog",
               "description": "golden retriever stretching by hearth",
               "action": "yawns and pads toward window",
               "emotion": "sleepy contentment",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "soft amber sunrise filtering through fog, interior warm Edison bulbs",
            "color_palette": "earthy browns, pine greens, warm amber highlights",
            "set_dressing": "stacked firewood, enamel kettle, leather journal, woven blankets",
            "atmosphere": "floating dust motes, gentle hearth smoke",
            "textures": "rough-hewn timber, ceramic mug glaze, wool throws"
         },
         "audio": {
            "ambience": "forest birds, distant loon call, kettle whistle",
            "score": "minimal piano with analog tape hiss",
            "foley": "pen scratching, dog collar jingle, sip sound"
         },
         "interactive_moment": "POV hands sliding cabin door open at 11s revealing lake expanse with rolling fog."
      },
      "effects": {
         "transitions": "cozy cross-dissolve between interior and exterior",
         "speed_ramp": "subtle 10% slow-down on dog stretch",
         "post": "add light bloom inside window, grain level 15"
      },
      "output": {
         "duration_seconds": 15,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "H.265",
         "render_style": "cozy_lifestyle"
      },
      "negative_prompt": [
         "visible drones",
         "smartphone overlays",
         "crowded background",
         "harsh blue lighting"
      ],
      "continuity": [
         "journal pen ink remains black",
         "steam volume consistent",
         "dog fur stays dry"
      ],
      "notes": "If Sora removes the dog, add 'include golden retriever stretching in foreground at 6s'."
   },
   {
      "title": "Tokyo Night Cyclist",
      "id": "lifestyle_tokyo_night_cyclist_v2",
      "version": "2.1",
      "tags": ["lifestyle", "urban", "tokyo", "night"],
      "prompt": {
         "scene_opener": "Neon alley in Shinjuku slicked with rain; signage reflections pulsate across pavement as pedestrians carry transparent umbrellas.",
         "camera": {
            "shot": "handheld chase perspective",
            "motion": "follow-cam trailing cyclist with lateral whip at corners",
            "lens": "28mm with 1.3x squeeze",
            "sensor": "full-frame, f/1.4",
            "movement_speed": "cyclist 4 m/s, camera matching",
            "motion_curve": "constant velocity with sudden whip before turns",
            "stabilization": "body rig with micro jitter retained"
         },
         "subjects": [
            {
               "id": "Cyclist",
               "description": "courier balancing bouquet strapped to backpack",
               "action": "navigates alley, ring bell, drifts around corner",
               "emotion": "focused determination",
               "wardrobe": "rain shell jacket, reflective straps, slim jeans"
            },
            {
               "id": "Bouquet",
               "description": "burst of pastel flowers",
               "action": "petals flutter in rain during drift",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "magenta-cyan neon, practical shoplights, wet street reflections",
            "color_palette": "electric magenta, cobalt, warm amber accents",
            "set_dressing": "ramen steam, hanging lanterns, vending machines, signage in Japanese",
            "atmosphere": "light rain, drifting steam, bokeh tail lights",
            "textures": "wet asphalt, plastic umbrellas, chrome bicycle"
         },
         "audio": {
            "ambience": "rain patter, crowd murmur, crosswalk chimes",
            "score": "uptempo synthwave bassline",
            "foley": "bike tires slicing water, bell rings, bouquet rustle"
         },
         "interactive_moment": "Slow-motion drift at 9s with rain droplets suspended before snapping back to real-time delivery hand-off."
      },
      "effects": {
         "transitions": "whip-pan motion blur between alley segments",
         "speed_ramp": "40% slow-mo during drift, return to 100%",
         "post": "heightened neon bloom, selective color saturation boost"
      },
      "output": {
         "duration_seconds": 12,
         "aspect_ratio": "9:16",
         "resolution": "UHD",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "urban_neon"
      },
      "negative_prompt": [
         "non-Japanese signage",
         "empty streets",
         "helmetless rider",
         "lens fogging"
      ],
      "continuity": [
         "rain intensity steady",
         "bouquet color palette constant",
         "cyclist visor stays clear"
      ],
      "notes": "To emphasize destination, append 'arrive at vintage kissaten with warm interior glow at 11s'."
   },
   {
      "title": "Mediterranean Rooftop Supper",
      "id": "lifestyle_mediterranean_rooftop_supper_v2",
      "version": "2.1",
      "tags": ["lifestyle", "travel", "mediterranean", "evening"],
      "prompt": {
         "scene_opener": "Twilight washes over terracotta rooftops while coastal breeze twirls string lights above rustic dining table.",
         "camera": {
            "shot": "crane reveal into circular dolly around table",
            "motion": "descending crane from rooftop edge transitioning into 360-degree slider",
            "lens": "35mm prime",
            "sensor": "full-frame, f/2.8",
            "movement_speed": "0.3 m/s",
            "motion_curve": "continuous circle easing around guests",
            "stabilization": "gimbal stabilized crane"
         },
         "subjects": [
            {
               "id": "FriendsGroup",
               "description": "four friends sharing tapas and wine",
               "action": "clink glasses, laugh, pass plates",
               "emotion": "joyful camaraderie",
               "wardrobe": "light linen shirts, breezy dresses"
            }
         ],
         "details": {
            "lighting": "string lights, candlelight, residual sunset glow",
            "color_palette": "warm ambers, terracotta reds, deep blue horizon",
            "set_dressing": "olive trees in terracotta pots, woven runner, artisanal ceramics",
            "atmosphere": "sea breeze moving napkins, distant fireworks bokeh",
            "textures": "rough stone walls, glazed plates, linen cloth"
         },
         "audio": {
            "ambience": "gentle coastal waves, distant festival cheers",
            "score": "acoustic guitar with hand percussion",
            "foley": "glass clinks, laughter, cutlery"
         },
         "interactive_moment": "Rack focus at 13s from close wine pour to far fireworks exploding near lighthouse."
      },
      "effects": {
         "transitions": "warm bloom dissolve into final toast",
         "speed_ramp": "none",
         "post": "apply subtle film grain, glow on string lights"
      },
      "output": {
         "duration_seconds": 18,
         "aspect_ratio": "16:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "H.265",
         "render_style": "travel_cinematic"
      },
      "negative_prompt": [
         "strong wind",
         "plastic tableware",
         "harsh spotlights",
         "city skyscrapers"
      ],
      "continuity": [
         "string lights sway gently but stay intact",
         "wine color remains ruby",
         "sky gradient transitions smoothly to night"
      ],
      "notes": "Append 'add faint lighthouse beam sweep across horizon every 6 seconds' for extra ambiance."
   },
   {
      "title": "Urban Sketcher Daybreak",
      "id": "lifestyle_urban_sketcher_daybreak_v2",
      "version": "2.1",
      "tags": ["lifestyle", "art", "city", "sunrise"],
      "prompt": {
         "scene_opener": "Sunrise ignites city landmark silhouette while empty streets catch golden reflections leading toward lone artist bench.",
         "camera": {
            "shot": "time-lapse tilt morphing to macro detail",
            "motion": "start with tilt from sky to ground, blend into stop-motion macro of sketchbook",
            "lens": "24mm for wide, 60mm macro for detail",
            "sensor": "APS-C, f/8 wide, f/3.5 macro",
            "movement_speed": "time-lapse 12x, macro real-time",
            "motion_curve": "linear for time-lapse, gentle handheld sway macro",
            "stabilization": "tripod locked for wide, handheld stabilization for macro"
         },
         "subjects": [
            {
               "id": "Sketcher",
               "description": "artist in layered denim jacket",
               "action": "paints watercolor strokes capturing skyline abstraction",
               "emotion": "absorbed concentration",
               "wardrobe": "denim jacket, beanie, fingerless gloves"
            }
         ],
         "details": {
            "lighting": "soft sunrise wash, reflected light from puddles",
            "color_palette": "pastel oranges, lavender shadows, muted teal watercolors",
            "set_dressing": "open sketch kit, portable stool, thermos",
            "atmosphere": "gentle breeze fluttering pages, distant morning commuters",
            "textures": "rough watercolor paper, stone pavement, knit fabrics"
         },
         "audio": {
            "ambience": "sparrows, distant tram bell, quiet city hum",
            "score": "lofi beats with brushed percussion",
            "foley": "brush dabs, water swirls, page flips"
         },
         "interactive_moment": "Split-screen overlay at 10s showing real skyline on left, evolving watercolor on right."
      },
      "effects": {
         "transitions": "ink bleed wipe between frames",
         "speed_ramp": "accelerated playback of painting sequence",
         "post": "add subtle vignette, raise paper texture detail"
      },
      "output": {
         "duration_seconds": 14,
         "aspect_ratio": "4:5",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "H.265",
         "render_style": "artistic_lifestyle"
      },
      "negative_prompt": [
         "corporate logos",
         "graffiti tags",
         "tourist crowds",
         "overly saturated colors"
      ],
      "continuity": [
         "watercolor palette stays cohesive",
         "sun progression linear",
         "artist posture consistent"
      ],
      "notes": "Add 'include whisper of steam from nearby coffee cup at 6s' for extra mood."
   },
   {
      "title": "Sahara Star Camp",
      "id": "lifestyle_sahara_star_camp_v2",
      "version": "2.1",
      "tags": ["lifestyle", "desert", "night", "astronomy"],
      "prompt": {
         "scene_opener": "Nighttime desert glamping site dotted with lanterns; dunes fade into star-saturated sky with Milky Way arch overhead.",
         "camera": {
            "shot": "aerial pullback to sky tilt",
            "motion": "drone lifts from fire pit to reveal camp, then tilts upward into star trail time-lapse",
            "lens": "20mm wide with low-light sensitivity",
            "sensor": "full-frame, f/1.8",
            "movement_speed": "0.8 m/s initial, then locked for time-lapse",
            "motion_curve": "ease-in during ascent, static during star trails",
            "stabilization": "drone gimbal with astro tracking"
         },
         "subjects": [
            {
               "id": "Traveler",
               "description": "solo traveler aligning telescope",
               "action": "adjusts dials, gestures toward constellations, logs notes",
               "emotion": "tranquil wonder",
               "wardrobe": "lightweight desert cloak, wool scarf"
            }
         ],
         "details": {
            "lighting": "lantern warm light, fire glow, cool starlight",
            "color_palette": "deep blues, warm amber highlights, silver starlight",
            "set_dressing": "embroidered rugs, low tables with tea set, star charts",
            "atmosphere": "gentle embers, occasional breeze stirring sand",
            "textures": "woven fabric, sand ripples, polished telescope brass"
         },
         "audio": {
            "ambience": "distant desert wind, crackling fire, soft camel bells",
            "score": "ethereal pads with oud melodies",
            "foley": "telescope adjustments, tea pour, notebook page flips"
         },
         "interactive_moment": "Tilt to star trail time-lapse at 12s with constellation labels briefly superimposed."
      },
      "effects": {
         "transitions": "match dissolve from real-time to time-lapse",
         "speed_ramp": "time-lapse acceleration 800% for star trails",
         "post": "add subtle lens flare on lanterns, reduce noise via denoise level 0.2"
      },
      "output": {
         "duration_seconds": 16,
         "aspect_ratio": "21:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes LT",
         "render_style": "astro_travel"
      },
      "negative_prompt": [
         "city light pollution",
         "tourist crowds",
         "vehicles",
         "harsh windstorm"
      ],
      "continuity": [
         "lantern brightness stays warm",
         "fire pit remains lit",
         "sky clarity consistent"
      ],
      "notes": "If stars appear static, add 'enable subtle star twinkle prior to time-lapse transition'."
   }
]
```

### Product & Commercial Spots

```json
[
   {
      "title": "Minimalist Smartwatch Reveal",
      "id": "product_minimalist_smartwatch_reveal_v2",
      "version": "2.1",
      "tags": ["product", "tech", "minimalist"],
      "prompt": {
         "scene_opener": "Matte white cyclorama with levitating pedestals casting soft contact shadows around flagship smartwatch.",
         "camera": {
            "shot": "robotic arm orbit macro",
            "motion": "continuous 270-degree orbit with 15-degree tilt",
            "lens": "85mm macro",
            "sensor": "full-frame, f/4",
            "movement_speed": "0.35 m/s",
            "motion_curve": "constant velocity with micro ease at hero angles",
            "stabilization": "robotic precision"
         },
         "subjects": [
            {
               "id": "Smartwatch",
               "description": "matte black case with micro-perforated band",
               "action": "face animates health metrics in synced beats",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "soft key from overhead lightbox, rim from back strip",
            "color_palette": "monochrome whites and charcoals",
            "set_dressing": "floating pedestals, vapor mist pulses, minimal shadows",
            "atmosphere": "subtle mist bursts triggered by beats",
            "textures": "satin metal, silicone band, frosted glass"
         },
         "audio": {
            "ambience": "studio silence",
            "score": "pulsed electronic ticks",
            "foley": "UI blips, haptic buzz"
         },
         "interactive_moment": "Transition at 8s to lifestyle insert: athlete sprinting through tunnel with motion-tracked UI overlay."
      },
      "effects": {
         "transitions": "match cut from product to lifestyle clip via haptic pulse flash",
         "speed_ramp": "slight slow-mo on heartbeat metric reveal",
         "post": "add clean bloom on edges, remove noise"
      },
      "output": {
         "duration_seconds": 12,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "minimalist_product"
      },
      "negative_prompt": [
         "fingerprints",
         "excessive reflections",
         "heavy shadows",
         "busy background"
      ],
      "continuity": [
         "watch screen color stays cyan",
         "vapor pulses sync to score",
         "orbit direction clockwise"
      ],
      "notes": "Append 'use white seamless floor with soft gradient falloff' if floor seams appear."
   },
   {
      "title": "Artisan Coffee Dripper Launch",
      "id": "product_artisan_coffee_dripper_launch_v2",
      "version": "2.1",
      "tags": ["product", "coffee", "kitchen"],
      "prompt": {
         "scene_opener": "Rustic kitchen bathed in morning haze; pour-over dripper centered on walnut counter with sunbeams.",
         "camera": {
            "shot": "top-down tilt to 45-degree hero",
            "motion": "start overhead, then tilt and dolly toward bloom",
            "lens": "50mm macro",
            "sensor": "full-frame, f/3.5",
            "movement_speed": "0.25 m/s",
            "motion_curve": "ease-in during bloom",
            "stabilization": "motorized jib"
         },
         "subjects": [
            {
               "id": "CoffeeDripper",
               "description": "ceramic dripper with brass frame",
               "action": "coffee bloom swells with steam swirling",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "soft morning key from window, bounce fill with reflector",
            "color_palette": "warm ambers, dark walnut, cream ceramics",
            "set_dressing": "linen towels, analog scale, beans in copper scoop",
            "atmosphere": "steam plumes, dust motes",
            "textures": "ceramic glaze, grain wood, frothy bubbles"
         },
         "audio": {
            "ambience": "quiet kitchen, faint birds",
            "score": "light acoustic guitar",
            "foley": "water pour, kettle whistle decay, cup clink"
         },
         "interactive_moment": "Overlay at 9s displays flavor notes in elegant serif typography mapped to aroma trails."
      },
      "effects": {
         "transitions": "steam wipe into overlay",
         "speed_ramp": "slow 15% during bloom expansion",
         "post": "add micro-contrast on steam, film grain level 10"
      },
      "output": {
         "duration_seconds": 14,
         "aspect_ratio": "16:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "artisan_product"
      },
      "negative_prompt": [
         "plastic accessories",
         "modern espresso machine",
         "harsh shadows",
         "textured clutter"
      ],
      "continuity": [
         "steam intensity steady",
         "coffee color consistent",
         "overlay uses cream background"
      ],
      "notes": "If steam vanishes, add 'sustain visible steam plumes throughout pour sequence'."
   },
   {
      "title": "Electric Car Pop-Up",
      "id": "product_electric_car_popup_v2",
      "version": "2.1",
      "tags": ["product", "automotive", "future"],
      "prompt": {
         "scene_opener": "Futuristic pop-up showroom inside city plaza with holographic grid floor reflecting metallic EV.",
         "camera": {
            "shot": "jib descend to hero profile",
            "motion": "start overhead, jib down and push toward front quarter",
            "lens": "24-70mm zoom set at 35mm",
            "sensor": "full-frame, f/4",
            "movement_speed": "0.6 m/s",
            "motion_curve": "ease-out as headlights ignite",
            "stabilization": "jib with dolly assist"
         },
         "subjects": [
            {
               "id": "EV",
               "description": "sleek electric coupe with dynamic LED fascia",
               "action": "headlights ripple like aurora, doors breathe open",
               "emotion": "n/a",
               "wardrobe": "n/a"
            },
            {
               "id": "Driver",
               "description": "young professional tapping start",
               "action": "activates vehicle, smiles toward camera",
               "emotion": "confident excitement",
               "wardrobe": "tailored techwear"
            }
         ],
         "details": {
            "lighting": "neon grid uplight, diffused key from overhead orb",
            "color_palette": "cool silver, cyan, deep navy",
            "set_dressing": "LED floor, holographic data columns, minimal crowd silhouettes",
            "atmosphere": "subtle haze for light beams",
            "textures": "polished metal, glass, carbon fiber"
         },
         "audio": {
            "ambience": "city murmur, light crowd",
            "score": "synth pulses with bass swells",
            "foley": "electric chime, door glides, footstep echo"
         },
         "interactive_moment": "Match cut at 11s to highway sunset driving shot with motion blur streaks."
      },
      "effects": {
         "transitions": "prismatic light streak wipe",
         "speed_ramp": "accelerate to 120% during highway reveal",
         "post": "enhance reflections via bloom, maintain highlight roll-off"
      },
      "output": {
         "duration_seconds": 20,
         "aspect_ratio": "21:9",
         "resolution": "4K",
         "frame_rate": 30,
         "delivery": "H.265 10-bit",
         "render_style": "futuristic_auto"
      },
      "negative_prompt": [
         "burnouts",
         "internal combustion exhaust",
         "crowded signage",
         "daytime lighting"
      ],
      "continuity": [
         "LED grid animation loops every 4 seconds",
         "driver outfit stays monochrome",
         "vehicle paint remains mirror-silver"
      ],
      "notes": "If crowd becomes dense, instruct 'limit background attendees to silhouettes'."
   },
   {
      "title": "Wellness App Storyboard",
      "id": "product_wellness_app_storyboard_v2",
      "version": "2.1",
      "tags": ["product", "app", "wellness", "mobile"],
      "prompt": {
         "scene_opener": "Airy apartment bathed in morning light; yoga mat centered with AR interface hovering above smartphone.",
         "camera": {
            "shot": "handheld lifestyle follow",
            "motion": "follow user from kitchen to mat, settle into over-the-shoulder",
            "lens": "35mm",
            "sensor": "APS-C, f/2.2",
            "movement_speed": "0.4 m/s",
            "motion_curve": "natural handheld sway",
            "stabilization": "IBIS with 5% micro jitter"
         },
         "subjects": [
            {
               "id": "User",
               "description": "wellness enthusiast in athleisure",
               "action": "launches app, mirrors breathing exercise",
               "emotion": "relaxed focus",
               "wardrobe": "sage green leggings, beige top"
            },
            {
               "id": "ARCoach",
               "description": "holographic guide silhouette",
               "action": "demonstrates breathing cycle synchronized with user",
               "emotion": "calm support",
               "wardrobe": "translucent light trails"
            }
         ],
         "details": {
            "lighting": "diffused morning sunlight, bounce fill from white walls",
            "color_palette": "pastel greens, sand neutrals, soft blues",
            "set_dressing": "plants, water carafe, journal",
            "atmosphere": "floating dust, gentle lens haze",
            "textures": "matte walls, woven mat, glass"
         },
         "audio": {
            "ambience": "soft apartment hush, distant city",
            "score": "ambient pads with soft bells",
            "foley": "tap on phone, inhale/exhale, mat rustle"
         },
         "interactive_moment": "Over-the-shoulder at 9s with AR overlay labeling breathing cadence and heart rate trend."
      },
      "effects": {
         "transitions": "L-cut audio into UI close-ups",
         "speed_ramp": "none",
         "post": "apply pastel LUT, add soft glow to AR coach"
      },
      "output": {
         "duration_seconds": 15,
         "aspect_ratio": "9:16",
         "resolution": "UHD",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "wellness_mobile"
      },
      "negative_prompt": [
         "cluttered overlays",
         "harsh lighting",
         "visible noise",
         "distracting reflections"
      ],
      "continuity": [
         "app UI colors remain teal and cream",
         "breathing cycle stays synced",
         "AR coach transparency consistent"
      ],
      "notes": "If AR overlay drifts, specify 'lock AR coach to mat center'."
   },
   {
      "title": "Luxury Fragrance Atmosphere",
      "id": "product_luxury_fragrance_atmosphere_v2",
      "version": "2.1",
      "tags": ["product", "fragrance", "luxury"],
      "prompt": {
         "scene_opener": "Infinite black void with suspended crystal prisms refracting pinspot beams onto perfume pedestal.",
         "camera": {
            "shot": "slow-motion dolly through prisms",
            "motion": "dolly push with slight arc through crystal forest",
            "lens": "100mm macro",
            "sensor": "full-frame, f/5.6",
            "movement_speed": "0.2 m/s",
            "motion_curve": "ease-in, hold on bottle, ease-out",
            "stabilization": "motion-control slider"
         },
         "subjects": [
            {
               "id": "FragranceBottle",
               "description": "faceted glass flacon with gold atomizer",
               "action": "mist envelops bottle as gold particles orbit",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "pinspot beams, underlighting from mirrored floor, high-contrast",
            "color_palette": "deep blacks, gold highlights, subtle plum accents",
            "set_dressing": "hanging crystals, velvet lounge inserts, ocean cliff flashbacks",
            "atmosphere": "atomized mist, floating gold dust",
            "textures": "cut crystal, polished gold, velvet"
         },
         "audio": {
            "ambience": "dark room hush",
            "score": "harp glissando over deep sub bass",
            "foley": "atomizer spray, gemstone clink"
         },
         "interactive_moment": "Flash cuts at 10s to sensory memory vignettes (ocean cliff, velvet lounge) before returning to bottle hero."
      },
      "effects": {
         "transitions": "strobe flash into memory scenes",
         "speed_ramp": "slow 40% for mist reveal",
         "post": "add bloom on highlights, vignetting 20%"
      },
      "output": {
         "duration_seconds": 18,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "ProRes 4444",
         "render_style": "luxury_noir"
      },
      "negative_prompt": [
         "literal flower close-ups",
         "bright white backgrounds",
         "text overlays",
         "crowded props"
      ],
      "continuity": [
         "mist density consistent",
         "gold particle swirl clockwise",
         "crystal reflections stay golden"
      ],
      "notes": "If bottle reflections clip, add 'soften specular intensity to 80%'."
   }
]
```

### Animation & Stylized

```json
[
   {
      "title": "Neon Sketch Parkour Rush",
      "id": "animation_neon_sketch_parkour_rush_v2",
      "version": "2.1",
      "tags": ["animation", "stylized", "parkour", "neon"],
      "prompt": {
         "scene_opener": "Hand-drawn neon cityscape pulses to life as cel-shaded athlete lands atop graffiti-splashed rooftop.",
         "camera": {
            "shot": "dynamic chase following rooftop run",
            "motion": "whip between 2D parallax layers with faux 3D depth shifts",
            "lens": "virtual 32mm",
            "sensor": "virtual APS-C, f/2.4",
            "movement_speed": "0.9 m/s with elastic acceleration",
            "motion_curve": "ease-in whip with snappy decel",
            "stabilization": "hand-drawn smear frames"
         },
         "subjects": [
            {
               "id": "Runner",
               "description": "cel-shaded freerunner with glowing sneaker trails",
               "action": "vaults across gaps, leaves neon sketch echoes",
               "emotion": "focused exhilaration",
               "wardrobe": "electric blue hoodie, reflective tape accents"
            }
         ],
         "details": {
            "lighting": "synthetic rim glow around characters",
            "color_palette": "cyan, magenta, midnight violet",
            "set_dressing": "floating graffiti panels, animated billboards",
            "atmosphere": "digital grain, animated speed lines",
            "textures": "2D toon ink with halftone overlays"
         },
         "audio": {
            "ambience": "distant city hum rendered in 8-bit",
            "score": "synthwave beat with sidechain pulses",
            "foley": "whoosh lines, sneaker skids, parkour impacts"
         },
         "interactive_moment": "Glitch smear at 9s morphs runner into wireframe silhouette before resolving back to inked form."
      },
      "effects": {
         "transitions": "digital wipe with pixel scatter",
         "speed_ramp": "subtle ramp to 120% during rooftop launch",
         "post": "add chromatic fringe and animated outline wobble"
      },
      "output": {
         "duration_seconds": 15,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "cel_neon"
      },
      "negative_prompt": [
         "realistic lighting",
         "live-action footage",
         "static background",
         "muddy color mixing"
      ],
      "continuity": [
         "neon sneaker trails remain cyan",
         "outline wobble amplitude consistent",
         "city signage loops every 4 seconds"
      ],
      "notes": "If parallax feels flat, add 'increase z-depth separation between foreground graffiti and skyline layers'."
   },
   {
      "title": "Stop-Motion Forest Spirits",
      "id": "animation_stop_motion_forest_spirits_v2",
      "version": "2.1",
      "tags": ["animation", "stop-motion", "fantasy", "forest"],
      "prompt": {
         "scene_opener": "Handcrafted woodland set with felt pines and glowing mushrooms surrounding central tree stump.",
         "camera": {
            "shot": "incremental push-in mimicking stop-motion cadence",
            "motion": "1cm per frame track on motion-control slider",
            "lens": "60mm macro",
            "sensor": "virtual full-frame, f/4",
            "movement_speed": "stop-motion stepped",
            "motion_curve": "jerky ease-in towards spirits",
            "stabilization": "locked stop-frame rig"
         },
         "subjects": [
            {
               "id": "SpiritTrio",
               "description": "clay woodland spirits with moss capes",
               "action": "light acorn lanterns one by one, exchange nods",
               "emotion": "gentle curiosity",
               "wardrobe": "felt cloaks, pine-needle belts"
            }
         ],
         "details": {
            "lighting": "practical fairy lights, warm edge from lanterns",
            "color_palette": "moss greens, amber gold, soft teal night",
            "set_dressing": "miniature ferns, pebble stream, carved rune stones",
            "atmosphere": "micro fog bursts, dust motes",
            "textures": "wool felt, clay fingerprints, carved bark"
         },
         "audio": {
            "ambience": "forest nocturnal hum, delicate wind chimes",
            "score": "celesta arpeggios with soft marimba",
            "foley": "lantern clicks, twig crunch, gentle footsteps"
         },
         "interactive_moment": "Overhead reveal at 12s shows constellations forming leaf shapes before returning to close-up."
      },
      "effects": {
         "transitions": "stop-frame light bloom between beats",
         "speed_ramp": "none",
         "post": "apply warm analog grain, preserve frame jitter"
      },
      "output": {
         "duration_seconds": 18,
         "aspect_ratio": "4:3",
         "resolution": "UHD",
         "frame_rate": 12,
         "delivery": "ProRes 4444",
         "render_style": "artisan_stop_motion"
      },
      "negative_prompt": [
         "smooth interpolation",
         "plastic sheen",
         "modern props",
         "overly bright key light"
      ],
      "continuity": [
         "lantern glow stays amber",
         "fog density remains subtle",
         "camera track direction constant"
      ],
      "notes": "Increase 'micro jitter amplitude' if motion feels too digital."
   },
   {
      "title": "Studio Ghibli Homage Train Ride",
      "id": "animation_ghibli_train_homage_v2",
      "version": "2.1",
      "tags": ["animation", "watercolor", "nostalgia", "train"],
      "prompt": {
         "scene_opener": "Watercolor countryside glows under golden hour while pollen drifts across horizon.",
         "camera": {
            "shot": "lateral tracking alongside vintage train",
            "motion": "parallax layers sliding to mimic multiplane camera",
            "lens": "virtual 40mm",
            "sensor": "watercolor simulation, f/4 equivalent",
            "movement_speed": "0.5 m/s",
            "motion_curve": "gentle ease throughout",
            "stabilization": "hand-painted wobble"
         },
         "subjects": [
            {
               "id": "ProtagonistChild",
               "description": "wide-eyed child in sailor outfit",
               "action": "presses face to window, breath fogs glass",
               "emotion": "joyful wonder",
               "wardrobe": "navy sailor suit, red necktie"
            },
            {
               "id": "ForestSpirits",
               "description": "semi-transparent whimsical creatures",
               "action": "frolic in fields paralleling train",
               "emotion": "playful curiosity",
               "wardrobe": "glowing leaf cloaks"
            }
         ],
         "details": {
            "lighting": "soft painterly sunset gradients",
            "color_palette": "pastel ochre, mint, blush pink",
            "set_dressing": "hand-painted train cabin, lace curtains, bento box on lap",
            "atmosphere": "floating pollen specks, watercolor bloom edges",
            "textures": "brushstroke granulation, paper grain"
         },
         "audio": {
            "ambience": "train wheel rhythm, distant meadow birds",
            "score": "orchestral strings with ocarina motifs",
            "foley": "window tap, fabric rustle, soft gasp"
         },
         "interactive_moment": "Interior shifts to dream realm at 13s with color palette shifting to twilight blues."
      },
      "effects": {
         "transitions": "watercolor bloom wipes",
         "speed_ramp": "none",
         "post": "enhance paper texture intensity to 70%"
      },
      "output": {
         "duration_seconds": 20,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "H.265",
         "render_style": "watercolor_story"
      },
      "negative_prompt": [
         "modern technology",
         "hard-edged outlines",
         "neon lighting",
         "harsh shadows"
      ],
      "continuity": [
         "pollen drift direction left to right",
         "train windows stay fogged lightly",
         "child wardrobe unchanged"
      ],
      "notes": "If spirits desync, add 'lock spirit silhouettes to move parallel with train speed'."
   },
   {
      "title": "Vector Pop Infographic",
      "id": "animation_vector_pop_infographic_v2",
      "version": "2.1",
      "tags": ["animation", "infographic", "vector", "pop-art"],
      "prompt": {
         "scene_opener": "Bold flat-color background snaps into place with geometric bursts and title typography.",
         "camera": {
            "shot": "simulated swipe transitions across cards",
            "motion": "left-to-right slides with overshoot easing",
            "lens": "orthographic",
            "sensor": "virtual",
            "movement_speed": "card swap every 2 seconds",
            "motion_curve": "anticipation and overshoot",
            "stabilization": "graph locked"
         },
         "subjects": [
            {
               "id": "CardSeries",
               "description": "stack of vector cards with iconography",
               "action": "animates icons and stat counters",
               "emotion": "energetic clarity",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "flat cel shading with drop shadows",
            "color_palette": "sunset orange, teal, royal purple",
            "set_dressing": "floating shapes, dotted halftones, diagonal stripes",
            "atmosphere": "clean graphic air",
            "textures": "vector flat with grain overlay"
         },
         "audio": {
            "ambience": "light sweep fx",
            "score": "funky bassline with claps",
            "foley": "icon pops, click swipes"
         },
         "interactive_moment": "Final CTA card pops forward with parallax and arrow pointing downward to caption."
      },
      "effects": {
         "transitions": "card swipe wipes",
         "speed_ramp": "micro ramp to 110% on CTA pop",
         "post": "apply subtle grain to avoid banding"
      },
      "output": {
         "duration_seconds": 10,
         "aspect_ratio": "1:1",
         "resolution": "4K",
         "frame_rate": 30,
         "delivery": "H.264",
         "render_style": "vector_pop"
      },
      "negative_prompt": [
         "complex gradients",
         "photographic elements",
         "low contrast",
         "crowded text"
      ],
      "continuity": [
         "icon line weight stays uniform",
         "card order remains headline, stat, CTA",
         "background color cycle loops twice"
      ],
      "notes": "Add 'maintain 12% drop shadow opacity' if depth reads too flat."
   },
   {
      "title": "Ink Wash Duel",
      "id": "animation_ink_wash_duel_v2",
      "version": "2.1",
      "tags": ["animation", "sumi-e", "samurai", "stylized"],
      "prompt": {
         "scene_opener": "Parchment backdrop blooms with sumi-e mountains before revealing two opposing figures.",
         "camera": {
            "shot": "swirling ink transition from wide to close",
            "motion": "brushstroke whip that settles into low angle",
            "lens": "virtual 50mm",
            "sensor": "ink simulation",
            "movement_speed": "rapid swirl then slow hold",
            "motion_curve": "ease-out into final clash",
            "stabilization": "painterly jitter"
         },
         "subjects": [
            {
               "id": "SamuraiOne",
               "description": "ink silhouette with crimson sash",
               "action": "draws blade with splash of red ink",
               "emotion": "calm intensity",
               "wardrobe": "flowing kimono"
            },
            {
               "id": "SamuraiTwo",
               "description": "opposing silhouette with dark indigo accent",
               "action": "counters with sweeping strike",
               "emotion": "focused resolve",
               "wardrobe": "layered robes"
            }
         ],
         "details": {
            "lighting": "ink wash gradients with subtle highlight ink",
            "color_palette": "monochrome sumi ink with single crimson accent",
            "set_dressing": "mountain silhouettes, distant torii gate",
            "atmosphere": "ink splatter particles, textured paper",
            "textures": "brushstroke bleed, paper fibers"
         },
         "audio": {
            "ambience": "wind gust through valley",
            "score": "shakuhachi flute with deep taiko hits",
            "foley": "sword unsheath, ink splash, footsteps"
         },
         "interactive_moment": "Freeze-frame at 12s stamps red seal before ink dissolves to black."
      },
      "effects": {
         "transitions": "ink splash wipes",
         "speed_ramp": "slow to 70% during clash",
         "post": "increase paper grain contrast"
      },
      "output": {
         "duration_seconds": 14,
         "aspect_ratio": "21:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "sumi_e_drama"
      },
      "negative_prompt": [
         "modern weapons",
         "full color scenes",
         "clean digital lines",
         "crowded backgrounds"
      ],
      "continuity": [
         "crimson accent only on SamuraiOne",
         "brush edge jitter stays subtle",
         "battlefield remains minimal"
      ],
      "notes": "If motion seems too smooth, set 'interpolate frames false'."
   }
]

### Experimental & Conceptual

```json
[
   {
      "title": "Gravity Reversal Atrium",
      "id": "experimental_gravity_reversal_atrium_v2",
      "version": "2.1",
      "tags": ["experimental", "conceptual", "architecture", "surreal"],
      "prompt": {
         "scene_opener": "Minimalist museum atrium where marble sculptures drift upward against inverted skylight.",
         "camera": {
            "shot": "inverted crane descending from ceiling to floor",
            "motion": "180-degree roll mid-way to reorient perspective",
            "lens": "24mm tilt-shift",
            "sensor": "full-frame, f/5.6",
            "movement_speed": "0.25 m/s",
            "motion_curve": "ease-in, pivot, ease-out",
            "stabilization": "gyro-stabilized crane"
         },
         "subjects": [
            {
               "id": "Visitors",
               "description": "serene patrons walking on inverted ceiling walkways",
               "action": "observe floating sculptures, hair defying gravity",
               "emotion": "calm awe",
               "wardrobe": "monochrome minimalist attire"
            }
         ],
         "details": {
            "lighting": "refracted skylight beams, cool ambient fill",
            "color_palette": "cool grays, icy blues, hints of alabaster",
            "set_dressing": "hovering sculptures tethered by light ribbons, mirrored floor",
            "atmosphere": "floating dust illuminated by beams",
            "textures": "polished concrete, glass, marble"
         },
         "audio": {
            "ambience": "hushed gallery air",
            "score": "ethereal choir pads",
            "foley": "footstep echoes, soft gasps"
         },
         "interactive_moment": "Camera passes through mirrored floor at 12s revealing alternate physics reality."
      },
      "effects": {
         "transitions": "mirror flip dissolve",
         "speed_ramp": "slow to 80% during rotation",
         "post": "accentuate light beams, add subtle particle glow"
      },
      "output": {
         "duration_seconds": 16,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "minimalist_surreal"
      },
      "negative_prompt": [
         "slapstick reactions",
         "messy lighting",
         "crowded signage",
         "visible camera rig"
      ],
      "continuity": [
         "gravity inversion remains consistent",
         "floating sculptures drift upward at slow pace",
         "visitor wardrobe maintains monochrome palette"
      ],
      "notes": "If orientation feels confusing, add 'include a rotating hanging mobile as gravity anchor at 6s'."
   },
   {
      "title": "Data Bloom Metaverse",
      "id": "experimental_data_bloom_metaverse_v2",
      "version": "2.1",
      "tags": ["experimental", "metaverse", "data", "abstract"],
      "prompt": {
         "scene_opener": "Endless black expanse with aurora-like voxel clusters blooming from central sphere.",
         "camera": {
            "shot": "orbit transitioning into first-person dive",
            "motion": "circular track around sphere then spline dive into core",
            "lens": "18mm fisheye",
            "sensor": "virtual, f/2.8",
            "movement_speed": "0.6 m/s orbit, 1.2 m/s dive",
            "motion_curve": "ease-in orbit, exponential dive",
            "stabilization": "virtual gimbal"
         },
         "subjects": [
            {
               "id": "AvatarGardeners",
               "description": "androgynous avatars weaving hand gestures",
               "action": "sculpt voxel blooms into living data flora",
               "emotion": "intent focus",
               "wardrobe": "iridescent holo-robes"
            }
         ],
         "details": {
            "lighting": "self-illuminated voxels casting prismatic refractions",
            "color_palette": "iridescent gradients of teal, magenta, gold",
            "set_dressing": "floating wireframe lattice, particle trails",
            "atmosphere": "low-lying volumetric haze with glitch sparks",
            "textures": "voxel blocks, holographic threads"
         },
         "audio": {
            "ambience": "binaural data hum",
            "score": "downtempo bass with glitch flourishes",
            "foley": "data chimes, gesture swooshes"
         },
         "interactive_moment": "First-person dive at 14s reveals macro fractal garden with blooming volumetric petals."
      },
      "effects": {
         "transitions": "pixel bloom crossfade",
         "speed_ramp": "accelerate to 140% on dive",
         "post": "add chromatic aberration on highlights"
      },
      "output": {
         "duration_seconds": 18,
         "aspect_ratio": "16:9",
         "resolution": "4K",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "glitch_bloom"
      },
      "negative_prompt": [
         "corporate logos",
         "gendered costumes",
         "flat lighting",
         "low poly artifacts"
      ],
      "continuity": [
         "central sphere remains anchor",
         "voxel bloom loops every 6 seconds",
         "avatar robes retain iridescent shimmer"
      ],
      "notes": "If dive feels dizzying, specify 'add guiding light trail toward core'."
   },
   {
      "title": "Time-Lapse Origami City",
      "id": "experimental_time_lapse_origami_city_v2",
      "version": "2.1",
      "tags": ["experimental", "origami", "timelapse", "city"],
      "prompt": {
         "scene_opener": "Blank white table folds itself into intricate paper skyline within seconds.",
         "camera": {
            "shot": "overhead hyperlapse with snap zoom inserts",
            "motion": "top-down slider with programmed pauses for snap zoom",
            "lens": "35mm",
            "sensor": "full-frame, f/8",
            "movement_speed": "hyperlapse 8x",
            "motion_curve": "stutter-stepped to feel handcrafted",
            "stabilization": "tripod locked between frames"
         },
         "subjects": [
            {
               "id": "PaperCity",
               "description": "modular origami buildings and vehicles",
               "action": "fold, unfold, glide along paper streets",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "clean studio top light with soft bounce",
            "color_palette": "white base with accent colors per district",
            "set_dressing": "folded river, parks, origami monorail",
            "atmosphere": "micro paper dust glints",
            "textures": "crisp paper fibers, scored folds"
         },
         "audio": {
            "ambience": "paper rustle loops",
            "score": "marimba rhythm with ticking metronome",
            "foley": "fold snaps, gentle whooshes, vehicle whispers"
         },
         "interactive_moment": "Snap zoom at 10s dives into office window revealing minuscule bustling interior."
      },
      "effects": {
         "transitions": "paper fold wipes",
         "speed_ramp": "brief slow to 90% during window reveal",
         "post": "boost micro-contrast on folds"
      },
      "output": {
         "duration_seconds": 12,
         "aspect_ratio": "16:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "origami_timelapse"
      },
      "negative_prompt": [
         "human hands",
         "messy background",
         "wrinkled paper",
         "uneven lighting"
      ],
      "continuity": [
         "fold direction remains clockwise",
         "accent colors assigned per district",
         "monorail loops every 5 seconds"
      ],
      "notes": "If folds appear sloppy, add 'increase crease sharpness to 85%'."
   },
   {
      "title": "Aurora Choir Installation",
      "id": "experimental_aurora_choir_installation_v2",
      "version": "2.1",
      "tags": ["experimental", "aurora", "choir", "installation"],
      "prompt": {
         "scene_opener": "Arctic cliffside stage with vertical light pillars echoing aurora above cloaked choir.",
         "camera": {
            "shot": "sweeping drone arc",
            "motion": "curved flight path hugging cliff edge",
            "lens": "20mm wide",
            "sensor": "full-frame, f/2.8",
            "movement_speed": "0.7 m/s",
            "motion_curve": "ease-in to crescendo",
            "stabilization": "cinema drone gimbal"
         },
         "subjects": [
            {
               "id": "Choir",
               "description": "silhouetted vocalists in flowing thermal robes",
               "action": "crescendo as light pillars pulse in sync",
               "emotion": "reverent power",
               "wardrobe": "deep navy cloaks"
            }
         ],
         "details": {
            "lighting": "aurora glow, pillar LEDs, moon rim light",
            "color_palette": "teal, indigo, icy whites",
            "set_dressing": "ice formations, minimal stage platform",
            "atmosphere": "frost particles, breath vapor",
            "textures": "snow crust, velvet robes, light haze"
         },
         "audio": {
            "ambience": "arctic wind",
            "score": "layered choral harmonies",
            "foley": "fabric sways, crunching snow"
         },
         "interactive_moment": "Drone enters light pillar at 14s transitioning into soundwave tunnel POV."
      },
      "effects": {
         "transitions": "light pillar wipe",
         "speed_ramp": "ramp to 110% during tunnel fly-through",
         "post": "add volumetric glow, maintain highlight roll-off"
      },
      "output": {
         "duration_seconds": 20,
         "aspect_ratio": "21:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 422",
         "render_style": "aurora_reverie"
      },
      "negative_prompt": [
         "city lights",
         "stage equipment clutter",
         "harsh strobes",
         "audience crowd"
      ],
      "continuity": [
         "light pillars pulse with choir dynamics",
         "choir robes remain navy",
         "aurora maintains teal gradient"
      ],
      "notes": "Add 'record light pillar timing to BPM 72' if sync drifts."
   },
   {
      "title": "Quantum Lab Dreamscape",
      "id": "experimental_quantum_lab_dreamscape_v2",
      "version": "2.1",
      "tags": ["experimental", "science", "dream", "lab"],
      "prompt": {
         "scene_opener": "Futuristic lab where chalkboard equations manifest as hovering holographic formulas.",
         "camera": {
            "shot": "steadicam weave through suspended equations",
            "motion": "figure-eight path with macro pause inside quantum bubble",
            "lens": "35mm",
            "sensor": "full-frame, f/2",
            "movement_speed": "0.5 m/s",
            "motion_curve": "smooth glide, micro push during bubble reveal",
            "stabilization": "Steadicam"
         },
         "subjects": [
            {
               "id": "Physicist",
               "description": "researcher in iridescent lab coat",
               "action": "plucks equation into mini-universe bubble",
               "emotion": "focused serenity",
               "wardrobe": "lab coat with fiber optic trim"
            },
            {
               "id": "QuantumBubble",
               "description": "floating orb containing nascent galaxies",
               "action": "swirls with cosmic dust as equations integrate",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "ultraviolet neon accents, soft white key",
            "color_palette": "violet, cyan, deep space black",
            "set_dressing": "floating chalkboards, crystalline consoles",
            "atmosphere": "micro particles, gentle lens fog",
            "textures": "polished metal, holographic glass, chalk dust"
         },
         "audio": {
            "ambience": "low-frequency lab hum",
            "score": "ambient synth pads with bell motifs",
            "foley": "chalk etch, hologram chime, fabric rustle"
         },
         "interactive_moment": "Macro close-up at 16s enters bubble showing galaxies forming with light flares."
      },
      "effects": {
         "transitions": "nebula swirl dissolve",
         "speed_ramp": "slow to 70% during bubble entry",
         "post": "add star glints, maintain noise floor"
      },
      "output": {
         "duration_seconds": 22,
         "aspect_ratio": "16:9",
         "resolution": "UHD",
         "frame_rate": 24,
         "delivery": "ProRes 4444",
         "render_style": "quantum_dream"
      },
      "negative_prompt": [
         "cluttered wires",
         "messy desktops",
         "overexposed highlights",
         "flat background"
      ],
      "continuity": [
         "equation glyphs glow cobalt",
         "bubble remains centered near desk",
         "physicist coat light pulses synchronized"
      ],
      "notes": "If lab feels cold, add 'introduce warm rim bounce from desk lamp at 8s'."
   }
]

### Social-First Micro Formats

```json
[
   {
      "title": "5-Second Hook Reel",
      "id": "social_hook_reel_v2",
      "version": "2.1",
      "tags": ["social", "short-form", "hook", "reel"],
      "prompt": {
         "scene_opener": "Kinetic typography blasts 'WAIT FOR IT' while confetti bursts in background.",
         "camera": {
            "shot": "snap zoom toward headline moment",
            "motion": "rapid push with handheld jitter",
            "lens": "28mm",
            "sensor": "APS-C, f/2",
            "movement_speed": "1.5 m/s",
            "motion_curve": "aggressive ease-in",
            "stabilization": "digital stabilization with micro shake"
         },
         "subjects": [
            {
               "id": "Creator",
               "description": "energetic host revealing color-changing jacket",
               "action": "snaps fingers to trigger unexpected reveal",
               "emotion": "playful surprise",
               "wardrobe": "neutral tee under iridescent jacket"
            }
         ],
         "details": {
            "lighting": "bright key with RGB edge lights",
            "color_palette": "punchy primaries, high saturation",
            "set_dressing": "bold backdrop graphics, confetti cannons",
            "atmosphere": "spark bursts, floating emojis",
            "textures": "glossy jacket, matte backdrop"
         },
         "audio": {
            "ambience": "studio hush",
            "score": "trap beat drop",
            "foley": "zipper snap, confetti pops"
         },
         "interactive_moment": "Freeze-frame at 4s with arrow CTA pointing to caption link."
      },
      "effects": {
         "transitions": "whip-pan match cut",
         "speed_ramp": "micro ramp for reveal",
         "post": "add punchy LUT, sharpen text overlays"
      },
      "output": {
         "duration_seconds": 6,
         "aspect_ratio": "9:16",
         "resolution": "1080x1920",
         "frame_rate": 30,
         "delivery": "H.264",
         "render_style": "social_hook"
      },
      "negative_prompt": [
         "slow intro",
         "muted colors",
         "small typography",
         "low energy"
      ],
      "continuity": [
         "headline text remains uppercase",
         "confetti burst timed at 2s",
         "jacket color change triggered once"
      ],
      "notes": "If CTA unreadable, add 'increase outline stroke to 6px'."
   },
   {
      "title": "Side-by-Side Transformation",
      "id": "social_side_by_side_transformation_v2",
      "version": "2.1",
      "tags": ["social", "transformation", "before-after", "vertical"],
      "prompt": {
         "scene_opener": "Screen split 50/50 with bold labels 'BEFORE' and 'AFTER'.",
         "camera": {
            "shot": "static tripod with subtle push",
            "motion": "digital crop to create slow push",
            "lens": "35mm",
            "sensor": "full-frame, f/4",
            "movement_speed": "0.05 m/s",
            "motion_curve": "linear",
            "stabilization": "tripod"
         },
         "subjects": [
            {
               "id": "TransformationSubject",
               "description": "room makeover progressing from cluttered to styled",
               "action": "match cuts align with beats",
               "emotion": "satisfied reveal",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "consistent softbox light both halves",
            "color_palette": "neutral base with accent color in after",
            "set_dressing": "overlay progress labels, minimal UI",
            "atmosphere": "clean airy",
            "textures": "matte walls, plush textiles"
         },
         "audio": {
            "ambience": "room tone",
            "score": "upbeat clap track",
            "foley": "tool clicks, drawer slides"
         },
         "interactive_moment": "Mid-sequence time-lapse overlay highlights effort before final reveal."
      },
      "effects": {
         "transitions": "match cut with motion blur",
         "speed_ramp": "time-lapse at 200% mid clip",
         "post": "ensure label drop shadows, clean edges"
      },
      "output": {
         "duration_seconds": 12,
         "aspect_ratio": "9:16",
         "resolution": "HD",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "before_after_reel"
      },
      "negative_prompt": [
         "camera jitter",
         "cluttered labels",
         "uneven lighting",
         "off-beat cuts"
      ],
      "continuity": [
         "camera angle locked",
         "labels stay top corners",
         "color grading consistent between halves"
      ],
      "notes": "If halves drift, add 'lock frame alignment to grid overlays'."
   },
   {
      "title": "Captioned Mini-Doc",
      "id": "social_captioned_mini_doc_v2",
      "version": "2.1",
      "tags": ["social", "documentary", "captioned", "vertical"],
      "prompt": {
         "scene_opener": "Bold caption ribbon announces topic over opening b-roll of city skyline.",
         "camera": {
            "shot": "mix of handheld vlog and tripod b-roll",
            "motion": "alternating close-up talking head and cutaways",
            "lens": "24mm for b-roll, 35mm for talking head",
            "sensor": "APS-C, f/2.8",
            "movement_speed": "varied",
            "motion_curve": "documentary style",
            "stabilization": "IBIS"
         },
         "subjects": [
            {
               "id": "Narrator",
               "description": "subject delivering insight direct-to-camera",
               "action": "speaks to audience while interacting with overlays",
               "emotion": "confident warmth",
               "wardrobe": "casual smart"
            }
         ],
         "details": {
            "lighting": "soft key with window fill",
            "color_palette": "editorial neutrals with accent yellow",
            "set_dressing": "floating infographics, subtitle bar",
            "atmosphere": "clean professional",
            "textures": "matte background, crisp type"
         },
         "audio": {
            "ambience": "light city bed",
            "score": "subtle piano loop",
            "foley": "button presses, pen scribbles"
         },
         "interactive_moment": "End card offers question sticker space with call-to-action."
      },
      "effects": {
         "transitions": "L-cut audio between scenes",
         "speed_ramp": "none",
         "post": "ensure subtitles high contrast, animate infographics"
      },
      "output": {
         "duration_seconds": 30,
         "aspect_ratio": "9:16",
         "resolution": "UHD",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "social_doc"
      },
      "negative_prompt": [
         "low-contrast captions",
         "chaotic b-roll",
         "shaky handheld",
         "dead air"
      ],
      "continuity": [
         "caption color stays brand yellow",
         "talking head angle consistent",
         "infographics animate clockwise"
      ],
      "notes": "If captions flicker, add 'force subtitle background opacity to 70%'."
   },
   {
      "title": "Looping Food Boomerang",
      "id": "social_looping_food_boomerang_v2",
      "version": "2.1",
      "tags": ["social", "food", "loop", "boomerang"],
      "prompt": {
         "scene_opener": "Macro shot of caramel drizzle frozen mid-air over plated dessert.",
         "camera": {
            "shot": "high-speed capture looping action",
            "motion": "micro dolly arc synced to loop",
            "lens": "100mm macro",
            "sensor": "full-frame, f/4",
            "movement_speed": "0.1 m/s",
            "motion_curve": "palindromic for seamless loop",
            "stabilization": "macro rail"
         },
         "subjects": [
            {
               "id": "Dessert",
               "description": "artisan plated dish with sparkling toppings",
               "action": "glaze pours then rewinds cleanly",
               "emotion": "n/a",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "warm key with bounce card",
            "color_palette": "caramel gold, chocolate brown, cream",
            "set_dressing": "ceramic plate, linen napkin, sprig garnish",
            "atmosphere": "steam wisps, specular highlights",
            "textures": "glossy sauce, matte plate"
         },
         "audio": {
            "ambience": "subtle kitchen hush",
            "score": "lofi beat loop",
            "foley": "sizzle, spoon tap"
         },
         "interactive_moment": "Overlay 'REPLAY' text pulses on beat at loop point."
      },
      "effects": {
         "transitions": "seamless loop",
         "speed_ramp": "loop matches 120 FPS playback",
         "post": "enhance specular bloom, remove noise"
      },
      "output": {
         "duration_seconds": 8,
         "aspect_ratio": "1:1",
         "resolution": "UHD",
         "frame_rate": 60,
         "delivery": "H.264",
         "render_style": "food_loop"
      },
      "negative_prompt": [
         "visible loop seam",
         "messy backdrop",
         "overexposed highlights",
         "blurry macro"
      ],
      "continuity": [
         "drizzle height consistent",
         "overlay color stays warm white",
         "camera arc repeats flawlessly"
      ],
      "notes": "If loop stutters, add 'align first and last frames on identical motion pose'."
   },
   {
      "title": "Quick Tip Carousel",
      "id": "social_quick_tip_carousel_v2",
      "version": "2.1",
      "tags": ["social", "carousel", "tips", "vertical"],
      "prompt": {
         "scene_opener": "Card 1 slams forward with headline '3 TIPS TO [Goal]'.",
         "camera": {
            "shot": "simulated swipe across cards",
            "motion": "left-to-right parallax slides",
            "lens": "orthographic",
            "sensor": "virtual",
            "movement_speed": "card swap every 3 seconds",
            "motion_curve": "anticipation, snap, settle",
            "stabilization": "vector locked"
         },
         "subjects": [
            {
               "id": "CardSet",
               "description": "series of pastel cards with icons and mini b-roll",
               "action": "animate bullet points and pictograms",
               "emotion": "motivational clarity",
               "wardrobe": "n/a"
            }
         ],
         "details": {
            "lighting": "flat even",
            "color_palette": "clean pastels with navy accent",
            "set_dressing": "rounded corners, consistent padding",
            "atmosphere": "minimal graphic noise",
            "textures": "subtle grain overlay"
         },
         "audio": {
            "ambience": "soft swipes",
            "score": "bouncy mallet melody",
            "foley": "card flips, icon pops"
         },
         "interactive_moment": "Final card CTA 'SAVE FOR LATER' with downward arrow and bookmarking sound."
      },
      "effects": {
         "transitions": "swipe wipes",
         "speed_ramp": "micro acceleration during card entrance",
         "post": "ensure icon drop shadows at 12% opacity"
      },
      "output": {
         "duration_seconds": 15,
         "aspect_ratio": "4:5",
         "resolution": "HD",
         "frame_rate": 30,
         "delivery": "H.265",
         "render_style": "carousel_tips"
      },
      "negative_prompt": [
         "complex backgrounds",
         "tiny text",
         "inconsistent padding",
         "dark color grading"
      ],
      "continuity": [
         "iconography maintains stroke weight",
         "card numbering sequential",
         "headline font stays bold serif"
      ],
      "notes": "If cards feel flat, add 'introduce parallax background gradient at 5% depth'."
   }
]

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
