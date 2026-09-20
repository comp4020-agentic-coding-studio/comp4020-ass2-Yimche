# Process overview

## What I built

Linux Ricing is a full course website for an invented course at Slop
University, built on the course-site Astro template and deployed to GitHub
Pages. It teaches the Unix desktop as a craft: twelve weeks of lectures and
labs, a five-part assessment scheme, a setup guide, and a teaching team, all
wrapped in a Catppuccin terminal aesthetic that argues a course about ricing
should look like the thing it teaches. The harness behind it, my `CLAUDE.md`
and the checks under `spec/`, carried forward from the week 6 crit
([`b6f52dd`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/b6f52dd)).

## How I got here

I first started by listing out 10 ideas. Some niche, some eccentric, such as
"Demonic Egyptology", "How to make a personalised ergonomic mech suit",
"Sailing the high seas, why piracy is protecting media", etc.
I made it generate a bunch of mockups to get an idea, a skeleton of the course
outlines. 
Once I settled I in one pass I set the course record and homepage, wrote the
teaching team and policies, laid out the twelve-week lecture programme and the
studio schedule, replaced the sample assessments with a five-part scheme,
and added the setup guide
([`7b6dbce...ac3cafb`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/compare/7b6dbce...ac3cafb)).
That gave me a complete site to react to rather than a blank one to imagine.

The visuals came next, and it drove most of the decisions after it. I recoloured
everything to Catppuccin so a single palette carries both light and dark
through one `light-dark()` token set
([`999e391`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/999e391)),
set the type in JetBrains Mono and removed all border radius 
([`9e285fd`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/9e285fd)),
then pushed further: cards and the home hero became terminal windows with
titlebars and traffic-light dots
([`f6ac00e`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/f6ac00e)),
and the page receded to Mantle so the reading column lifts off it, such that it
didn't feel so flat.
([`33a3aa9`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/33a3aa9)).
A slide deck for every week followed
([`64a3518`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/64a3518)),
and the assessment scheme grew until its weights reached 100 percent
([`34cd21e`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/34cd21e)).

One issue I had was trying to get more visually appealing elements.
Unfortunately the ability to add images was very vague and I didn't want to
potentially violate copy right laws, so I removed a lot of the text as without
visual cues it is a bit difficult to follow a wall of text.

Most of the work was the long tail of reacting to the built site. I brought the
People page back after cutting it, and had some fun with the people,
([`6e00cdf`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/6e00cdf)),
added a Readings section
([`21511b3`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/21511b3)),
reworked the teaching team, and dropped the placeholder portraits rather than
fake them
([`a7e528e`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/a7e528e)).
A recurring problem was the page grid: it insets the reading column on the left
only, so content ran flush against the right edge. I fixed it at the panel
level, so prose, figures, and cards all get symmetric breathing room
([`2dee162`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/2dee162)),
and embedded each week's deck directly in its lecture page
([`ad37e2d`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/commit/ad37e2d)).

The clearest example of how the loop actually goes is the lead paragraphs.
Asked to replace the lead on People and Readings with a header, I first removed
the wrong thing, a body paragraph, and left the real lead standing. The lead
turned out to be the frontmatter description, rendered by the layout, so the fix
was to thread the theme's opt-out through the wrapper and switch it off, then
restore the paragraph I had wrongly cut. The prompt that caught it was blunt:

> what happened to removing the p.leads for readings and people?

I kept both commits rather than squashing them, because the misstep is part of
the record
([`0957600...420c592`](https://github.com/comp4020-agentic-coding-studio/comp4020-ass2-Yimche/compare/0957600...420c592)).

Throughout, `pnpm check` (build, axe accessibility, the base-path and
broken-link checks, the deck check, and the course-data test) was the gate I
ran before every commit.
