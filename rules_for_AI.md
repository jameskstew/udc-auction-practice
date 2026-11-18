# The UDC group project market: complete rules

Understanding Digital Capitalism (University of Edinburgh), group project, Weeks 3 to 5.

This file describes the whole market so that you, or an AI chatbot you paste it into, can work out bidding strategies and operator strategies. The points are only for choosing firms. They do not count towards marks.

## 1. The setting

- About 27 students rank 7 firms each from a list of 30 firms, favourite first.
- Project teams of about 4 people are formed (7 teams). Some teams choose each other; the rest are placed with people who chose similar firms.
- Each team must end up with exactly one firm to study, and each firm goes to at most one team.
- The course organiser runs the market and is called the **operator**. Everything teams pay goes to the operator.

## 2. Firms on offer

- Only some firms are up for auction. By default these are the **10 most popular firms** from the survey (popularity: a 1st choice scores 7 points, a 2nd choice 6, down to 1 for a 7th choice).
- The operator can change this: the most popular N firms, every firm at least one student chose, or all 30.
- A team **cannot bid for a firm that any of its members studied in the Week 3 case study**. Such bids are ignored.
- The list of firms on offer is fixed when round 1 opens.

## 3. Points

- Every team starts with **100 points**. All teams start equal; points have nothing to do with marks or team make-up.
- Points are spent in three ways, all paid to the operator:
  1. the **price** of the firm a team wins;
  2. **rent**, paid by every team that wins nothing in a round;
  3. a **secret boost**, if the team chooses to pay one.
- Points left at the end are worth nothing.

## 4. A round, step by step

1. **Bids.** Each team still without a firm submits one sealed bid: up to **3 firms** (default), with a number of points for each. Bids plus boost must not add up to more than the team's points. Each bid must be at least the **minimum bid** (default 1). Teams cannot see each other's bids.
2. **Secret boost (optional).** A team may also pay the operator up to **25 points** (default). The boost makes all of that team's bids rank as if they were bigger: the multiplier is **1 + boost ÷ 50**. So a 10-point boost gives ×1.2, a 25-point boost gives ×1.5. The boost is paid whether or not the team wins anything. It does not add points to any bid, and the team still pays for a firm in real points.
3. **Ranking.** All bids from all teams are put in one list, ordered by their **weighted size** (bid × the team's multiplier), largest first. Ties are broken at random.
4. **Awarding.** Go down the list. For each bid:
   - if that team has already won a firm, skip it;
   - if that firm has already gone to another team, skip it;
   - otherwise the team **wins** that firm.
5. **Price (second price, the default).** The winner pays only what it needed to beat the best rival bid for that firm, plus 1 point, and never more than its own bid:
   - price = min( own bid, (best rival's weighted bid ÷ winner's multiplier) + 1 )
   - If nobody else bid for that firm, the price is the minimum, 1 point.
   - Alternative rule the operator can choose: **pay your own bid** (first price).
6. **Rent.** Every team that won nothing this round pays **20 points** of rent (default; or all its remaining points if it has fewer), then bids again next round for the firms still free, with the points it has left.
7. **Last round.** After **3 rounds** (default), any team still without a firm is given a free firm by lot.

After each round, every team's bids and boosts are shown to everyone.

## 5. Worked examples

**Example A: boost wins and saves points.** Your team bids 40 for Anthropic with an 11-point boost (multiplier 1.22), so it ranks as 48.8. Team 6 bids 39 with no boost. You win. To beat 39 you needed a real bid of 39 ÷ 1.22 = 32, so you pay 32 + 1 = 33. Without the boost you would have paid 39 + 1 = 40. The boost saved 7 on the price but cost 11.

**Example B: boost turns a loss into a win.** Team 6 bids 39 with a 10-point boost (×1.2), ranking 46.8. You bid 40 with no boost. Team 6 wins and pays 40 ÷ 1.2 + 1 = 34.3. Without its boost it would have lost.

**Example C: rent.** Your team bids 50 for TSMC but Team 2 bids 60 and wins it; your other bids lose too. You pay 20 rent and start round 2 with 80 points, choosing from fewer firms.

**Example D: uncontested firm.** You bid 30 for Kiva and nobody else bids for it. You win and pay 1.

## 6. What the rules imply (for thinking about strategy)

- With the second-price rule, what you pay depends on the **rival's** bid, not yours, so bidding what a firm is really worth to you is safer than shading your bid down.
- A big bid on one firm makes you likely to win it, but if it loses you pay rent and have fewer firms left.
- Spreading points over 3 firms gives you more chances, but each bid is smaller.
- Only one bid per team can win, and the largest weighted bids are settled first. Your **largest** bid is the one most likely to be decided first.
- Popular firms attract more rival bids. Less popular firms on offer may be won cheaply.
- A boost helps most when you expect a close contest; it is wasted if your firm was uncontested or if you lose anyway.
- Rent makes waiting expensive: 3 lost rounds cost 60 points.

## 7. The simulated rival teams (practice page only)

The practice page runs six rival teams, each with one fixed strategy:

| Strategy | What it does |
|---|---|
| Spreader | Spreads its points evenly over five liked firms (cut to the bid limit) |
| All-in | Puts everything on its favourite firm |
| Booster | Pays a 20-point boost in round 1, then bids on two firms (2:1) |
| Bargain hunter | Bids evenly on firms that are less popular |
| Top-heavy | 60% on its favourite, the rest spread |
| Random | Random firms and amounts |

Rivals choose firms in proportion to popularity. **They do not adapt to the rules or to your behaviour.** Real teams will.

## 8. Being the operator

On the practice page you can set the rules and run 1,000 simulated auctions to see how much the operator collects. The rules you can change:

| Rule | Default | Range on the page |
|---|---|---|
| Price rule | Second-highest bid + 1 | or pay your own bid |
| Rent per round | 20 | 0 to 60 |
| Minimum bid (reserve price) | 1 | 1 to 60 |
| Firms on offer | 10 most popular | 8 to 30 |
| Bids per round | 3 | 1 to 5 |
| Maximum secret boost | 25 | 0 to 50 |
| Boost strength | 5 points per +0.1 (÷50) | 2.5 or 10 points per +0.1 |
| Rounds before firms go by lot | 3 | 1 to 5 |

Total points in the market: 7 teams × 100 = 700.

## 9. Questions to ask an AI chatbot

Paste this whole file into the chatbot first, then ask, for example:

- "Our team ranks firms A, B and C as worth 60, 30 and 10 to us. Five other teams are likely to want A. Suggest a bid and boost for round 1, and explain the risk."
- "When is a secret boost worth paying? Work out the break-even for a 10-point boost."
- "Is it better to bid on 1 firm or 3? Compare the expected outcomes."
- "Which operator rules would maximise revenue if the teams did not adapt? Which if the teams learned the rules?"
- "How does this market compare with Google's ad auction, or with app store rankings that sellers can pay to boost?"
- "Who benefits from the secret boost: the teams, or the operator?"

Then test the chatbot's suggestions on the practice page. Do they work against the simulated teams? Would they work against your classmates?

## 10. Playing with your own bot

You can prime a chatbot to play for your team on the practice page.

1. Paste this whole file into the chatbot. Tell it your team's goal and how much risk you will take. For example:
   - "We want firm 2 (Anthropic) and no other. If we lose it, we do not care what we get."
   - "We don't mind which of firms 8, 19 and 27 we get, but we want to pay as little as possible."
   - "Get us any firm in the top 5, and never pay rent."
   - "We want to win cheaply, even if it is a less popular firm."
   - "Spend nothing on boosts: we think they mainly benefit the operator."
   You can also type the goal into the box on the practice page, so it is sent with every round.
2. On the practice page, press **Copy this round for the chatbot** and paste the result in. It gives your points, the firms still free, the bid limits and every bid from earlier rounds.
3. Ask the chatbot for this round's bid. **It must end its reply with one line in exactly this format:**

   `BID: 12=40, 2=30, 26=20; BOOST=10`

   The numbers before `=` are the firm numbers from the list (1 to 30). The numbers after are points. Use at most the number of bids allowed. Bids plus boost must not exceed your points left. `BOOST=0` means no boost.
4. Paste the chatbot's whole reply into **Paste the chatbot's bid** and press **Use this bid**. The page reads the `BID:` line and fills in the form. Check it, then submit the round.
5. Repeat each round. Afterwards, compare: how did your bot do against the simulated teams? How did other students prime their bots, and whose did best?

## 11. Betting on the outcome (practice page)

On top of the auction there is a prediction market. It uses separate **betting tokens** (100 to start), which never affect who gets a firm.

- Before each round, markets open on: who wins each of the three most popular free firms this round (each team still without a firm, or "nobody this round"); whether every team will have a firm after the round; and whether any team will pay a secret boost.
- The six simulated teams bet too, each from its own rough view of the odds (worked out by simulating the round).
- **Self-staking is allowed.** You can bet on your own team. You know your own bid and the others do not, so you are an insider.
- **Pooled betting:** everyone stakes tokens on an outcome. After the round the operator takes its cut (default 5%) and the rest of the pot is shared among those who backed the result, in proportion to their stakes. If nobody backed the result, all stakes are returned.
- **Live prices (like Polymarket):** the operator runs an automated market maker (a logarithmic market scoring rule, liquidity 25). Each outcome has a price from 0 to 100, read as a probability, and the prices always add up to 100. Buying an outcome raises its price. Each share pays 1 token if that outcome happens. The operator takes its cut from each purchase, and can lose money if bettors know better than its prices.

Questions to ask: When is betting on your own team worth more than winning the firm? Could a team bid low on purpose and bet against itself? Who earns more from betting, the operator or the insiders? How is this like insider trading on Polymarket or Kalshi, or match-fixing in sports betting?
