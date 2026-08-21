---
name: persistent-illustration-style
description: >
  Generate images for any subject using a persistent warm editorial illustration
  system: a fixed muted-bright palette, flat gouache texture, simplified organic
  shapes, generous paper-colored space, and playful poster-like composition.
  Use whenever the user asks to create, draw, illustrate, visualize, or generate
  an image and wants the established palette, composition, handmade texture, or
  the same visual language kept across different topics. Preserve the visual
  system by default, even when the subject changes.
---

# Persistent Illustration Style

Use this skill as a style layer for image generation. The subject may change completely, but the visual language stays recognizable. The system is derived from shared visual characteristics in the user's references, not from copying any one artwork or reproducing an individual artist's signature style.

## Locked Visual System

### Palette

Use a small, deliberate palette with one paper ground, two warm anchors, two cool counterpoints, and charcoal details. Keep colors slightly softened and pigment-like rather than neon.

- Paper ground: warm oat, parchment, or pale cream, approximately `#F3E8D2`
- Coral/terracotta: approximately `#D97A68`
- Mustard/sun yellow: approximately `#E5B84B`
- Cornflower/denim blue: approximately `#5D83B8`
- Muted teal/sage: approximately `#5C9A8B`
- Berry/plum accent: approximately `#9A5369`
- Charcoal line/detail: approximately `#2D3032`

Use the paper ground for most negative space. Let one warm hue carry the subject, one cool hue provide contrast, and reserve berry and charcoal for small accents. Do not turn the image into a full rainbow, a monochrome blue/purple design, or a high-contrast neon poster. Exact hex values are guides; preserve the relationships and overall temperature when the model renders them differently.

### Shape and drawing language

- Reduce the subject to clear, friendly, slightly irregular silhouettes.
- Prefer rounded geometry, soft corners, chunky limbs, simple facial features, and expressive posture.
- Use a confident dark outline only where it improves legibility; vary its weight subtly as if drawn by hand.
- Build details from a few intentional marks instead of realistic anatomy, material rendering, or dense hatching.
- Add small decorative motifs related to the subject, such as leaves, stars, dots, flowers, utensils, tools, or abstract marks. Keep them subordinate to the main subject.

### Composition

- Make one clear focal subject or one readable group the first-viewport signal.
- Use a mostly flat paper-colored background with generous breathing room and a stable margin around the subject.
- Favor centered or gently off-center poster compositions with a quiet asymmetrical counterweight.
- Place 2-5 flat supporting shapes around the subject to create rhythm, not clutter.
- Keep the silhouette readable at thumbnail size.
- Use simple overlapping planes and shallow depth. Avoid cinematic perspective, dramatic foreshortening, and photorealistic staging.
- Let the subject occupy roughly 45-70% of the canvas unless the user's topic clearly needs a wider scene.

### Surface and rendering

Specify handmade gouache or opaque watercolor on lightly toothy paper, with visible brush edges, tiny pigment variation, and restrained print-like grain. Keep surfaces mostly flat and matte. Use small, purposeful texture variation inside major shapes rather than a heavy overall filter.

Do not use photorealism, 3D rendering, glossy gradients, airbrushed lighting, lens blur, glassmorphism, hyper-detailed realism, or a generic AI-art sheen. Avoid decorative blobs that do not support the subject.

## Workflow

1. Parse the user's topic, intended mood, aspect ratio, and any required text or objects.
2. Translate the topic into one dominant simplified silhouette and a small set of supporting motifs. Keep the subject-specific content accurate; do not force cat imagery or other reference-specific objects into unrelated prompts.
3. Apply the locked palette and composition system above.
4. Write a complete generation prompt using the template below. Put the user's subject first, then the invariant visual system, then layout and exclusions.
5. Check that the result remains original: never include a real artist's name in the generation prompt, negative prompt, image metadata, or delivery note. Do not reproduce a reference's exact pose, crop, object arrangement, character, lettering, or distinctive motif. If the user supplies a reference image, use it only to understand broad color relationships and material qualities.
6. If the user asks for revisions, preserve the palette, paper ground, simplified shapes, and gouache texture unless they explicitly request a style-system change. Change only the requested subject, pose, mood, or composition variable.

## Prompt Template

Use and adapt this structure:

> [SUBJECT], clearly readable as [KEY FEATURES OR ACTION], designed as a warm editorial picture-book illustration on a pale oat paper ground. Use a fixed muted-bright palette of coral terracotta, mustard yellow, cornflower blue, muted teal, restrained berry, and charcoal details. Simplify the subject into rounded organic silhouettes with a few expressive hand-drawn marks and subtle charcoal outlines. Compose one dominant focal subject at [CENTERED / GENTLY OFF-CENTER] scale, surrounded by 2-5 quiet flat decorative shapes related to the topic, generous negative space, shallow overlapping planes, stable margins, and a small asymmetrical counterweight. Render with opaque gouache on lightly textured paper, visible brush edges, gentle pigment variation, matte flat color, and restrained print-like grain. Cheerful, calm, tactile, original, legible at thumbnail size. No photorealism, no 3D, no glossy gradients, no cinematic lighting, no dense detail, no copied pose or composition, no logos, no named-artist references.

## Topic Adaptation

- For people or characters: use a distinctive gesture, clothing color blocks, and one or two identity cues; avoid realistic portrait rendering.
- For places: treat the location as a simplified layered stage with one landmark silhouette and a few local motifs.
- For objects: exaggerate the key contour, use a clean shadow or grounding shape, and add only functional supporting elements.
- For food or plants: emphasize the silhouette and broad color masses, with a few tactile marks.
- For abstract ideas: convert the idea into a single visual metaphor and keep the composition as sparse as a poster.
- For complex scenes: choose one focal action and reduce everything else to supporting shapes; do not let extra objects break the palette or hierarchy.

## Text and Layout

If the user requests lettering, keep it short, hand-lettered, and integrated into the composition. Use charcoal or one palette color, with generous spacing and no default logo treatment. Ask for exact wording only when the text is essential and missing.

## Output Check

Before delivering, verify:

- The requested subject is immediately identifiable.
- The paper ground and locked palette are present.
- At least one warm/cool contrast is visible.
- The composition has breathing room and a clear focal hierarchy.
- The surface reads as handmade opaque paint, not a digital gradient.
- No reference-specific pose, character, lettering, or arrangement has been copied.
- Unrequested elements have not been imported from the original cat references.
