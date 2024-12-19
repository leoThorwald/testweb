---
layout: default
title: Welcome to our Data Story
---

<div class="homepage">
    <div class="content">
        <h1>Welcome to our Data Story!</h1>
        <h2>DO YOU BELIEVE IMDB RANKING REFLECT BOX OFFICE?</h2>
        <a href="#about" class="btn btn1">Tell Me More</a>
    </div>
</div>

<div id="introduction" class="section">
    <h1>Introduction</h1>
    <p>
        Michael Bay’s Transformers movie franchise once reigned in the box office for four movies in a row while barely having gotten more than 60% in Rotten Tomatoes before finally being struck down in the form of a flop. Still, its sheer staying power for an entire decade practically redefined what Hollywood juggernauts, even those that were never particularly critic darlings, can do. Fast forward 7 years later, and Transformers One, despite enjoying a rave 89% Rotten Tomatoes, made barely enough to break even production and marketing wise.
    </p>
    <p>
        The sheer disparity between various films in what amounts to the same cinematic arena presents a curious paradox: which factors decide such things? How can a series that critics gleefully dismantle—often with the precision of a Decepticon going after a power grid—still rake in billions at the box office; while films showered with praise, poetic dialogue, and teary-eyed festival audiences sometimes limp away from theaters with barely enough profit to buy popcorn? This baffling divide between critical acclaim and financial success in cinema isn't just a case of art versus commerce—it’s a fascinating puzzle of audience expectations, marketing muscle, and the ever-mysterious “X factor” that drives people to theaters (or keeps them away).

    </p>
    <p>
        With this data analysis story, we aim to explore – and hopefully reveal – the hidden mechanics behind why some films soar financially despite scathing, or at least middling, reviews, while others praised as modern masterpieces fade into relative box office oblivion. It can be hidden in the overall way the plot shifts, the degree it fluctuates, the way the plot might’ve leaned too much or little into one emotion, or the blessing (or curse) of certain star power. This is the story about the outliers, the films that refuse to conform to the average data analyst’ neat linear regression models. Let’s untangle the reels and find out.
    </p>
</div>


<!-- Portfolio Section -->
<div id="portfolio" class="section">
    <h1>First Data Insights</h1>
    <p>
        However, the primary factor we need to consider is that movie ticket prices have been rising each year due to `inflation`. This leads to an increase in total box office revenue, even if the number of moviegoers remains steady or slightly declines. Therefore, we need to adjust for inflation's effect on box office revenue and introduce the `US-CPI` index as a measure of inflation. Below is a look on how adjusting for inflation puts into perspective how well movies in certain years might *actually* have performed by the standards of the time.
    </p>
    <img src="{{ '/assets/images/fig_1.jpg' | relative_url }}" alt="Portfolio Image" class="section-image">
    <p>
        We take a small look at the language makeup of our dataset, for a better idea that our use of the US-CPI index hopefully don’t overwhelmingly misrepresent movies from other countries:
    </p>
    <p>
        Meanwhile, we take a detour in trying to (tentatively) see if movie runtime might’ve correlated with either the runtime or revenue a bit. As we can see, the relationship for either is not entirely straightforward. 
    </p>
    <p>
        An even closer look, where we take a look at the distribution of runtime and revenue across runtime (in blue), and the distribution of movie counts in pink, might give us better insight.
    </p>
    <p>
        Interestingly, longer runtimes also show a very subtle correlation with higher ratings (and a less subtle but still notable correlation with adjusted revenue). However, this trend is far from definitive and doesn’t necessarily imply that runtime directly influences either revenue or ratings. Instead, it may hint at a preference for films with enough time to develop compelling narratives, though other factors undoubtedly play a more significant role in a film’s success. 
        We finally plot the adjusted revenue against movie ratings directly, with the color of each movie based on how well it performs comparatively both in critics ratings and box office performance. We can get a faint sense that whenever one increases, the other follows - but, of course, far from everything follows a neat linear regression line.
    </p>
    <p>
        Feel free to explore below the timeline of movies being plotted on box office vs ratings, colored by each country of origin, throughout all the years included in the IMDb dataset
    </p>
</div>

<!-- About Section -->
<div id="about" class="section">
    <h1>Discovering the Overperformers and Underperformers</h1>
    <p>
        Now that we’ve waded through all the data, it’s time to draw the line between the glittering overperformers and the tragically underperformers. To spot the outliers, we first need to define what’s “normal.” After all, one film’s blockbuster is another’s underwhelming flop, depending on context.
        When we apply a log transformation to the dataset, the box office revenue becomes more evenly distributed, smoothing out extremes and bringing the data closer to resembling a linear relationship. This adjustment provides a clearer lens through which to identify the standouts—both those that defy expectations and those that fall short.
    </p>
</div>

<!-- Timeline Section -->
<div id="timeline" class="section">
    <h1>Timeline</h1>
    <p>
        A chronological overview of key milestones in our journey.
    </p>
</div>

<!-- Team Section -->
<div id="team" class="section">
    <h1>Team</h1>
    <p>
        Meet the amazing people behind this project.
    </p>
</div>

<!-- Contact Section -->
<div id="contact" class="section">
    <h1>Contact</h1>
    <p>
        Get in touch with us for more information or collaboration opportunities.
    </p>
</div>
