# __Religious Attendance__

### CSS 610 Agent-Based Modeling

#### _Kelby Mace 4/7/2025_

Hardware Platform: Lenovo ThinkPad with AMD Ryzen 7 4700U processor, Radeon Graphics, and 16GB RAM (x64-based architecture).

Operating System: 64-bit Windows OS

Software Development Environment: VS Code Jupyter Notebook extension, Python version 3.10.6

#### __Assumptions:__

1. Social network does not change as a result of an agent's religious participation (or lack thereof).

2. Agents initialized as "religious" have historically attended institution every tick, while agents initialized as secular historically have never attended.

3. Whether someone is considered religious or secular is simply whether they attended that religious institution the previous tick.

4. Agents attend at most one service per tick (they can only be affiliated with one religious institution at a time).

5. Secular agents have a random network with a specifiable number of connections.

#### __Parameters to Analyze:__

1. Strategy distribution:
- 3 Scenarios:
    - Even mix of strategies.
    - No contrarian strategies.
    - Global strategies versus local (concerned with neighbors only).

2. Scale-free vs. small-world (and parameters of each)

3. Initial Conditions (how many are religious / secular at the start)
- 3 Scenarios:
    - 1 Religion, low secular.
    - 1 Religion, no secular.
    - 1 Religion, 50/50.
    - 1 Religion, high secular.

4. Number of inter-faith connections, number of secular connections.

#### __Questions to Ask:__

1. What percent of the population must be "independent fixed" to maintain religious attendance above some level (and under what combination of other conditions)?

2. What percent of the population do you need to have contrarian strategies to maintain oscillation?

3. What conditions sustain some sort of steady state?

4. What conditions lead to (almost) 100% secularization or religiosity?

5. What are the impacts of multiple institutions?

#### __Future Investigation:__

1. Calibrate strategy parameters and probabilities of having a certain strategy (decision-making criteria).

2. Look at the effect of number of religious / secular connections (if one is religious, their network will have more religious people)

3. Look at the effects of weighted decision-making (popular people with high centrality have more of an influence in an agent's decision than others). But they already have a higher influence based on their position in the network...

4. Agent social networks are dynamic (if they go to church, they meet people there)

5. People who make decisions independently

6. Generate agent roles / attributes, such as father, with familial relations...
