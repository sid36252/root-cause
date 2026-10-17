# Reddit — r/Cricket (posted)

**Title:**
Spent way too long building a WAR (Wins Above Replacement) model for Test cricket, turns out Root's #1 since 2001. Tell me where I'm wrong.

**Body:**

Been messing around with Cricsheet's ball-by-ball data (2001 onwards, so about 1.76m deliveries) and ended up building a proper WAR model for Test cricket, the kind basketball and baseball have had forever but cricket never really has. Adjusts for opposition quality, pitch conditions, country, and how much each moment mattered.

Would like some pushback on this rather than just posting it and running. Quick rundown of where it landed on the debates people actually argue about:

Root's #1, no asterisk. Best value of anyone, bat or ball, across the whole 25 years.

Lyon over Ashwin, which surprised me too. Turns out Lyon's done almost all his bowling in Australia (worst country in the dataset for a spinner) and Ashwin gets a lot of his in India (the easiest), so once that's priced in it's not close.

Root beats Smith on career value but Smith's ahead per Test.

Stokes edges Jadeja on total career value, Jadeja's clearly ahead per Test. Close either way.

Anderson over Steyn, and not for the reason I expected. Not conditions. Anderson's best season came at 39, Steyn's body never got that long.

Anderson vs Broad is basically a coin flip, closest gap in the whole thing.

Full writeup's here if you want the numbers: https://sid36252.github.io/root-cause/

Curious what people who've watched this era closely think I've got wrong.

---

# LinkedIn — Root Cause (posted)

Spent the last while building a Wins Above Replacement model for Test cricket, from scratch, off 1.76 million ball-by-ball deliveries.

It's the metric basketball and baseball have used for years and cricket's never really had. Adjusted for opposition quality, pitch conditions, and how much each moment mattered to the result, not just raw runs and wickets.

Joe Root comes out on top, worth roughly 16 extra wins to England across his career, more than anyone else since 2001.

A few of the other findings surprised me too, including a spinner who rates as the second most valuable player of the last 25 years despite never being mentioned in the same breath as the sport's greats, once you account for exactly where he's bowled most of his career.

Full piece here: https://sid36252.github.io/root-cause/

---

# LinkedIn — Measure Twice (post later, a few days after Root Cause)

Ten rebuilds. Three real bugs that changed the leaderboard. Twelve ideas that looked promising, got built, got tested against held-out data, and got correctly thrown out.

Wrote up the full build log behind the Test cricket WAR model I posted about last week, including the one that stung the most: a model that beat every validation check I had, passed random-split AND time-based testing, and still turned out to be invalid because two players were quietly grading their own homework.

If you're interested in how a small modeling project actually gets stress-tested rather than just shipped the first time it "works": https://sid36252.github.io/measure-twice/
