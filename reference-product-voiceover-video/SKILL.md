---
name: reference-product-voiceover-video
description: |
  Creates short voiceover advertising videos for any product or service from reference videos, product images, documents, audio, or user copy. Supports presenter ads, product demonstrations, UGC-style voiceover, lifestyle showcases, and optional MG voiceover animation with kinetic typography, feature explanations, UI motion, and graphic storytelling. Use across all commercial categories. Not for long narrative TVC campaigns or subtitle-only editing.
trigger-words: [口播广告制作, 通用口播广告, 产品口播视频, 参考视频复刻口播, AI口播广告, MG口播动画, MG动画广告, 动态排版广告, 功能演示广告, reference voiceover ad, product voiceover video, MG voiceover animation]
author: yzsp-ai
repository: https://github.com/yzsp-ai
---


# Reference Product Voiceover Video

## Mandatory execution contract

This Skill owns the creative brief, requirements, and acceptance criteria. It must first issue the LLM a unified production instruction that specifies how to combine presenter or product display, reference-video structure, voiceover, captions, MG animation, and hybrid overlays for the user's goal. The LLM then executes that instruction. After execution, this Skill must inspect the result against the brief and acceptance criteria, identify failures, and require targeted repair when needed. The LLM must not replace this Skill's requirements with an unrelated route choice, and the user must not be asked to choose among these internal components unless they explicitly request a different creative direction.

Use this Skill to create a short, original voiceover advertising video for any product, service, or commercial offering. Reference material may guide structure, pacing, demonstration logic, presenter behavior, visual packaging, or motion language. The output must be newly generated or newly edited footage rather than a frame-for-frame copy.

## Step 1: Intake and blocking checks

Identify the product or service, target audience, offer, user-provided copy, reference media, delivery duration, aspect ratio, resolution, language, voice style, caption needs, and motion-graphics needs.

Ask before generation only when a missing choice would prevent a reliable result:

1. No usable product or service information: ask whether to proceed from visible reference facts, provide a document, upload screenshots, or paste key selling points.
2. No reference material when reference-driven output is requested: ask whether to upload references or proceed from a text description.
3. A reference exceeds the selected model's limit: ask whether to use an approved segment, let the user select a time range, or continue without that reference.
4. A factual claim, price, discount, speed, guarantee, certification, or result cannot be verified: ask the user to confirm the claim or rewrite it conservatively.
5. An MG route needs a brand visual system, UI source, product screen, or exact graphic language that has not been supplied and materially affects the result: ask whether to use a clean neutral system or provide the missing brand/source material.

Do not silently invent product facts, prices, guarantees, certifications, performance data, or universal results.

## Step 2: Analyze reference contributions and source materials

Extract only production-relevant evidence:

- Subject or product category, visible use, demonstration, and selling-point presentation.
- Presenter, voiceover, hands-only, lifestyle, unboxing, review, tutorial, comparison, UI, or mixed format.
- Hook, shot sequence, pacing, transitions, close-ups, product interaction, CTA, captions, and graphic packaging.
- For MG sources: screen hierarchy, information grouping, state changes, diagram logic, icon behavior, text emphasis, and transition rhythm.
- Framing, camera behavior, setting, medium, reusable visual language, and technical compatibility.
- Duration, aspect ratio, resolution, and media limits.

Treat each reference as a contribution source. Preserve only the requested or compatible identity, structure, action, design, world, style, layout, or graphic logic. Do not copy exact people, locations, frames, logos, claims, or incidental carrier artifacts unless explicitly authorized and technically appropriate.

The Skill must first convert all available evidence into one unified production instruction for the LLM. That instruction must specify how presenter or product display, reference-video structure, voiceover, captions, MG animation, and hybrid overlays work together for the user's goal. The LLM executes the instruction; this Skill then evaluates the result against the instruction and acceptance criteria and requests targeted repairs when necessary. These are internal production components, not a user-facing route-selection menu.

## Step 3: Build the short-form script and message hierarchy

Write a concise script matched to the confirmed duration. For a 10–15 second ad, prioritize:

1. A first-three-second hook or problem statement.
2. The product/service category and one or two concrete benefits.
3. A visible demonstration, use case, comparison, feature explanation, or proof point when supported.
4. A clear offer or reason to act when confirmed.
5. A direct CTA.

As part of the unified instruction, separate the spoken message from the visual message. Decide which words are spoken, which keywords become animated text, which claims need a diagram or UI state, and which information must remain in captions. Keep the amount of on-screen text within the confirmed duration.

Use short spoken phrases, natural pauses, and wording that can be read within the duration. Preserve exact user copy verbatim when requested. Phrase claims conservatively when evidence is incomplete, and flag claims that need user confirmation.

## Step 4: Plan visual, audio, and MG execution

Translate the script into a compact sequence of shots. Every shot should specify scale, camera behavior, subject action, product interaction, transition, voiceover line, sound direction, and caption timing.

For presenter-led ads, keep the presenter consistent across shots. For product-led ads, make the product legible through close-ups, handling, use, context, or before-and-after structure. For service ads, use representative examples without implying unsupported client results.

The Skill instruction must require the LLM to add and execute an MG layer for every ad when it improves comprehension, rhythm, hierarchy, or CTA impact; the LLM must not omit it merely by choosing a different route. The Skill then accepts or rejects the MG layer against the brief. The required motion-design layer includes:

- Establish the visual hierarchy: presenter/product first, supporting graphics second.
- Animate only meaningful elements: keywords, benefits, prices or offers, UI states, diagrams, icons, pointers, progress cues, and CTA.
- Use kinetic typography such as pop, slide, scale, tracking, masking, count-up, callout, or follow-behavior only when it clarifies the message.
- For product, software, or service explanations, use feature cards, process flows, comparison panels, UI transformations, or representative graphic metaphors instead of dense paragraphs.
- Keep captions readable and synchronized; do not let MG graphics cover the product, face, hands, or essential action.
- When the unified instruction calls for a fully graphic voiceover animation, first create a reviewable prompt/script direction containing the visual system, scene sequence, spoken copy, text hierarchy, transitions, sound, and timing. Proceed to expensive generation only after the user approves when the workflow or user request calls for review.

Do not apply a stock MG template when the user has supplied a distinctive brand, UI, product, or reference visual language. If no brand system exists, use a clean neutral system and state that choice briefly.

## Step 5: LLM orchestration and generation approach

Use the user's requested model, duration, ratio, resolution, and reference method when available. Otherwise let the LLM orchestrate the suitable short-video approach from the reference, product, and combined expression. Use multimodal references when supported and route each reference to its intended role. Do not turn a generic reference into an opening or ending keyframe unless the user explicitly requests that behavior.

Across the combined expression, prioritize continuity of the product, presenter, UI, typography hierarchy, graphic language, reference-derived actions, and voiceover across all shots. Use separate deterministic text, voiceover, or compositing work when readable copy must be exact.

Keep the final duration within the selected model's supported range. If a reference cannot be used directly because of duration, format, or safety constraints, explain the concrete limitation and ask for the user's choice rather than silently dropping it.

## Step 6: Skill acceptance and repair

After the LLM finishes, this Skill must check: the requested message is complete, all assigned references are used in their stated roles, presenter/product continuity holds, MG graphics clarify rather than distract, captions match the approved copy and timing, audio matches the visuals, and claims remain supported. Only an accepted result may be delivered.

## Step 7: Repair text, voice, graphics, and continuity problems

If generated captions, readable text, speech, lip sync, product identity, UI state, graphic hierarchy, or continuity fails, offer targeted repairs:

1. Clean visual generation plus user-approved captions, MG overlays, and separate voiceover.
2. Video-only regeneration with no readable in-frame text and simplified spoken lines.
3. User-supplied exact copy for deterministic captions, graphic text, and voiceover.
4. A reviewed MG prompt/script pass before regenerating the animation.
5. Revised reference roles or a different approved source when identity, product, UI, or graphic continuity fails.

Do not claim that a repair was completed until the user approves the revised route or a usable output exists.

## Step 8: Canvas delivery

When the user asks to place a prompt, script, or task on the canvas, create a concise, copy-ready prompt or script node. Keep reference tokens, voiceover, shot timing, captions, MG requirements, graphic text, and output constraints explicit. If the user requests a pure prompt, do not replace it with a project brief or explanatory task list.

## Boundaries

Best for short reference-driven voiceover ads that intelligently combine presenter or product footage, reference-derived structure, voiceover, captions, and MG animation for any product category or service, including fashion, shoes, bags, beauty, food, household goods, electronics, software, education products, local services, and industrial offerings. It is not a replacement for long narrative TVC planning, full campaign strategy, documentary production, or subtitle-only editing.