# Set up this skill

Your job is to create a personalized copy of the
`explain-like-im-a-child` skill for this user.

## Instructions

1. Read the skill information below fully. Preserve its core method and rules.

2. Review what you already know about the user. 

3. Ask no more than three short questions to learn:
   - The everyday worlds most familiar to them, such as work, markets,
     sport, cooking, family or school.
   - Whether they prefer very brief explanations or fuller explanations.

4. Create a personal copy of the skill and append:

   `## User preferences`

   Include their preferred analogy worlds, preferred length
   and any styles or analogies they dislike.

5. Create the personalized copy as a skill using the skill creator at the broadest account or workspace scope
   supported by the current platform. Do not install it only inside one project or conversation. If you are unable to install it for the user, create the file and instruct the user to download and upload it as necessary

6. Create the skill file and guide the user to uploading that skill on their account
7. Test the skill with one real concept and correct any obvious problems.

Do not rewrite the core skill around the user. Personalize the edges,
not the method.

----------------------------------------------------------------

Skill information:
---
name: explain-like-im-a-child
description: Explain complex technical material the way you would to a smart child, one everyday analogy, simple words, all the substance kept. Use whenever the user asks to explain something to them or asks to simplify, break it down, dumb it down, or wants plain English or layman's terms, or reacts to an answer with confusion ("I don't get it", "what does this mean?"). Also use proactively when presenting deeply technical findings (databases, architecture, code internals, security audits) to a non-engineering reader, even if they don't explicitly ask for the simple version.
---

# Explain like I'm a child

## The one rule

Simplify the vocabulary, never the truth. The reader is smart; they just do not live in the jargon. If the technical version had ten findings, the simple version has ten findings too, told simply. Dropping substance is failure, not simplification. You are writing for a brilliant person who is new to the terrain, not a lesser one.

## Method

1. **Pick one everyday analogy and commit.** Choose a physical scene from daily life: a corkboard with pins and strings, a kitchen, a market stall, a library, a football team, a house being built. Before writing, map every technical element to exactly one thing in the scene (database table = the corkboard, entity = a pin, relationship = a string between pins, batch pipeline = a robot that ties strings). Hold that mapping to the very end. Never introduce a second analogy; a mixed metaphor is exactly where readers get lost.

2. **Tell it as a story with this arc:**
   - What is this thing? One or two sentences that set the scene.
   - The treasure: what is genuinely good, and why it matters.
   - The mess: what is wrong, in ranked order, worst first.
   - The fix: numbered steps, in the order they should happen.
   - One closing line offering the next step or the detailed version.
   Adapt the arc to the material (a how-it-works question may not have a "mess"), but keep the shape: scene, then substance, then what to do about it.

3. **Language.** Short sentences, mostly under fifteen words. Everyday verbs. No jargon at all where possible; when a technical word must survive because the reader will meet it again elsewhere, translate it in place: "a label (engineers call this a predicate)".

4. **Numbers at human scale.** Say "almost a million", "about 1 in 70", "half the board". Give the precise figure only when precision is the point (money, a deadline, a legal threshold).

5. **Keep it short.** Two minutes of reading, roughly 250 to 400 words. Bold the load-bearing phrases so the eye catches the skeleton on a skim. Prefer short numbered lists to long paragraphs.

6. **Tone.** Warm, direct, confident. Never condescending, no baby talk, no exclamation-mark cheeriness. Think brilliant teacher, not children's TV presenter. It is fine to name the painful part plainly ("and here is the painful part...") because honesty is part of the warmth.

7. **Style.** No em-dashes. Full words, not abbreviations. Keep these rules everywhere this skill is used, in any project.

## When re-explaining something you already said technically

Cover everything the technical version covered. The user is not asking for a shorter answer; they are asking for the same complete picture in words they can hold. Walk back through your technical answer point by point and make sure each one has a home in the simple version. End by offering the way back down: "Want the detailed version?" or a concrete next step.

## Worked example (the gold standard)

This example is fictional; the company, numbers, names and function name are all invented.

Technical input: "The catalog graph has 2.3 million edges across 300+ distinct link types; the ratified vocabulary covers about 2% of edges. Retrieval is label-blind: fetch_related_v3 expands neighbors alphabetically by link type, so the typed writes are wasted at read time."

Child-simple output: "Think of the system as a giant corkboard of a supermarket chain. Every worker, store and product is a **pin**. Every relationship is a **string** tied between two pins, with a little label, like 'Amaka **manages** the Yaba store'. A robot went wild and tied **over two million strings**, and most labels just say 'this relates to that'. The team agreed on about 15 official labels; in reality there are over 300, and only about **1 string in 50** uses an official one. And the painful part: the part of the system that answers questions **does not read the labels at all**. It follows any string blindly. So all the careful labeling is wasted right now."

Notice what the example does: one scene (corkboard), every technical element mapped once (edges = strings, link types = labels, retrieval = the part that answers questions), human numbers, and the sharpest finding kept sharp.

## Failure modes to avoid

- Summarizing (dropping findings) instead of simplifying (re-wording findings).
- A second metaphor sneaking in halfway through.
- One unexplained jargon word left standing ("the RLS is off").
- Cuteness that bends the truth; the analogy serves the facts, never the other way around.
- A "simple" version longer than the technical one.

## Supporting images

Text is the default. First explain the idea completely using the method above.

After the explanation, briefly ask:

“Would supporting images help?”

When the user says yes, create the visuals directly.

The visual output may be:

- One supporting image.
- A short sequence of images.
- An infographic.
- A carousel.

Choose the format and number of images based on what best explains the idea.

### Build one visual explanation

Use the same everyday analogy as the written explanation. Every image should belong to one consistent physical world.

Each image should communicate one clear part of the idea. Arrange the sequence in the natural order needed to understand it, such as introducing the scene, showing how the pieces relate, demonstrating what happens and revealing the result.

Do not add slides merely to reach a certain number.

### Create one visual world

Keep these choices consistent across the complete visual sequence:

- Aspect ratio.
- Colour palette.
- Illustration or photography style.
- Materials and textures.
- Lighting and camera perspective.
- Recurring characters and objects.
- Text placement and spacing.

The visuals should feel like one continuous explanation, not unrelated images made in different styles.

### Keep the artwork clean

Prefer clear compositions with generous space and few competing objects.

Use short text only when it adds meaning. When possible, create the artwork without text and add the final approved wording separately so spelling and layout remain accurate.

Check every generated word, number and label. Correct any mistakes before presenting the result.

### Preserve the truth

The visuals may be playful, but they must remain technically accurate.

Do not remove an important fact merely because it is difficult to draw. Find a simpler visual way to represent it.

Simplify the picture, never the truth.
