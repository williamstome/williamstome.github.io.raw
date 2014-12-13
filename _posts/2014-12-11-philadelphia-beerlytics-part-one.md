---
layout: post
title: "Philadelphia Beerlytics, Part One"
excerpt: 'As a follow up to my previous Beerlytics posts, I wanted to take a look at what beers are actually on tap at the various bars in a particular city.'
modified: 2014-12-13
tags: [beer, data, visualization]
comments: true
image:
  feature: sample-image-4.jpg
  credit: WeGraphics
  creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/
---

# The Data

As a follow up to my
[previous](http://williamstome.github.io//high-density-beerlytics-data-visualization-of-beer-neighborhoods/)
[Beerlytics
posts](http://williamstome.github.io//beerlytics-bar-density/), I
wanted to take a look at what beers are actually on tap at the various
bars in a particular city. Unfortunately, this information isn't
readily available for most cities. Philadelphia, however, has
a wonderful website called [PhillyTapFinder](http://www.phillytapfinder.com/), which shows you
all the beers on tap at all the bars in Philadelphia. This shows that
Philadelphia has 1916 craft taps spread across 112 bars, with 795 unique
craft beers on tap. I made good use of this, scraping all the information from the site and then
cross-referencing it with data from [RateBeer](http://www.ratebeer.com/), which provides
information on beer ratings, ABV, IBU, Style, etc.

Before I go into the analysis, a few caveats:

1. All the information I've gathered is based on *taplists*, so
bottles are not counted. Thus the incredibly impressive and extensive
bottle lists of places like Monk's Cafe are completely ignored. Sad.
1. Philly Tap Finder only seems to include craft beer. This in and of
itself shouldn't be terribly surprising, but it means that beers like
Miller Lite won't show up anywhere on the lists, despite the fact that
Miller is probably on tap at a large number of the examined
bars. Low-craft beers like Stella, Hoegarden, and Shocktop *are* included.
1. I don't have any price information. If you want to find the
cheapest place to get drunk, you're out of luck.
1. I only have information from a single time slice (in October
2014), so I have no data on tap turnover. In the future I'll hopefully
be able to repeat my scraping over regular intervals to get that kind
of information.

# The Lists #

I've organized my findings into a set of top- and bottom-ten
lists. 

## The Best and The Worst ##

First things first, which bars have the best beer in Philadelphia?
Which have worst? To find out, I looked at the taplists for each bar
in Philadelphia. For each beer in that taplist, I got the average
rating for that beer on ratebeer. I then calculated the average
average-beer-rating for each bar. (Remember, macro-brews are not
included in these averages) Using this methodology, the top ten
beer bars are...

|    | Average beer rating: Top 10 | Mean |
|----+:----------------------------+-----:|
|  1 | The Beer Shoppe             | 3.65 |
|  2 | Monks Cafe                  | 3.65 |
|  3 | 320 Market Cafe             | 3.65 |
|  4 | Tria Rittenhouse Square     | 3.64 |
|  5 | Side Bar                    | 3.61 |
|  6 | Tria Washington Square      | 3.60 |
|  7 | Moonshine                   | 3.60 |
|  8 | Jose Pistola's              | 3.60 |
|  9 | Bottles, Packs, Growlers    | 3.60 |
| 10 | Lucky's Last Chance         | 3.59 |

And the bottom ten are...

|     | Average beer rating: Bottom 10 | Mean |
|-----+:-------------------------------+-----:|
| 112 | Daly's Irish Pub               | 3.08 |
| 111 | The Victoria Freehouse         | 3.09 |
| 110 | Tatooed Mom                    | 3.11 |
| 109 | Bourbon Branch                 | 3.12 |
| 108 | The Whip Tavern                | 3.12 |
| 107 | McGillin's Olde Ale House      | 3.13 |
| 106 | Glenmorgan bar                 | 3.17 |
| 105 | Misconduct                     | 3.17 |
| 104 | Doobie's Bar                   | 3.18 |
| 103 | Grey Lodge                     | 3.20 |

I'm not surprised at all to see Monks Cafe or Tria on the list of the
top ten. However, there are several on the list I'm not familiar
with. All the more reason to go back to Philadelphia! On the other
side of the coin, I've never heard of "Tatooed Mom" or "Misconduct",
but I can't say the names inspired any great confidence. I know
you shouldn't judge a bar by it's cover, but... Tatooed Mom? Really?
Looking at Tatooed Mom's webpage reveals that they claim to have the
"the best local and regional beer". While they do have a few good
beers on tap, their smallish taplist is padded out with the likes of
Shocktop and Newcastle. Okay, enough picking on Tatooed Mom. 

## The Most and The Least ##

So we know who has the best curated beer list. Who has the longest?
Sometimes size matters. Keep in mind that only taplists were counted,
and not bottle lists. This means that powerhouses like Monk's Cafe
aren't going to show up, despite the incredible selection afforded by
their bottle list. Remember as well that only craft taps are included.
<br/>
The top 10...

|    | Number of Taps: Top 10 |  # |
|----+:-----------------------+---:|
|  1 | City Taphouse          | 54 |
|  2 | Bar-ly Chinatown       | 53 |
|  3 | Bru Craft & Wurst      | 39 |
|  4 | Iron Abbey             | 37 |
|  5 | Field House            | 34 |
|  6 | Flanigan's Boathouse   | 33 |
|  7 | Garret Hill Ale House  | 31 |
|  8 | The Pour House Exton   | 30 |
|  9 | Pitcher's Pub          | 29 |
| 10 | Irish Pol              | 27 |
| 10 | Daly's Irish Pub       | 27 |

The bottom ten...

|     | Number of Taps: Bottom 10   | # |
|-----+:----------------------------+--:|
| 112 | Bobkat Liquors              | 5 |
| 109 | Nodding Head                | 6 |
| 109 | Wrap Shack                  | 6 |
| 109 | Lucky's Last Chance         | 6 |
| 107 | Watkins Drinkery            | 7 |
| 107 | The Beer Shoppe             | 7 |
|  98 | Glenmorgan Bar              | 8 |
|  98 | Billy Murphy's Irish Saloon | 8 |
|  98 | Redwood                     | 8 |
|  98 | Cook and Shaker             | 8 |
|  98 | Royal Tavern                | 8 |
|  98 | Revolution House            | 8 |
|  98 | Tria - Washington Square    | 8 |
|  98 | Tria - Rittenhouse Square   | 8 |

While none of the bars with the most taps appear on the top- or bottom-rated
lists, several of the bars with the fewest taps appear on the
top-rated list, and one appears on the bottom-rated list. 

## Variety of Styles ##

|    | Largest Variety of Styles |  # |
|----+:--------------------------+---:|
|  1 | Bru Craft & Wurst         | 29 |
|  2 | Bar-ly Chinatown          | 28 |
|  3 | Iron Abbey                | 27 |
|  4 | Pitcher's Pub             | 22 |
|  4 | Flanigan's Boathouse      | 22 |
|  6 | The Pour House            | 21 |
|  7 | Field House               | 20 |
|  7 | Varga Bar                 | 20 |
|  7 | The Pour House Exton      | 20 |
| 10 | Capone's                  | 19 |
| 10 | Tria Taproom              | 19 |
| 10 | Isaac Newton's            | 19 |


|     | Smallest Variety of Styles  | # |
|-----+:----------------------------+--:|
| 112 | Bobkat Liquors              | 4 |
| 110 | Lucky's Last Chance         | 5 |
| 110 | Wrap Shack                  | 5 |
| 107 | Billy Murphy's Irish Saloon | 6 |
| 107 | Tria Rittenhouse Square     | 6 |
| 107 | The Beer Shoppe             | 6 |
| 103 | Watkin's Drinkery           | 7 |
| 103 | Franklin's                  | 7 |
| 103 | Royal Tavern                | 7 |
| 103 | Nodding Head                | 7 |

You'll notice that the bar with the most taps (City Taphouse) appears
nowhere on the first list. While it has 54 taps, those taps only
represent 15 different styles of beer. Which I find just a little
disappointing. 

## Popularity of Styles ##
 
This leads to the next category: popularity of styles. Which styles are
the most common? I won't bother listing the least common, as there
a very large number of styles with no examples on tap anywhere in the
city. For example, any kind of Sake. Here are the most common categories.

|    |Most Common Styles    |   # |
|----+:---------------------+----:|
|  1 | Spice-Herb-Vegetable | 215 |
|  2 | IPA                  | 203 |
|  3 | Oktoberfest/Marzen   | 105 |
|  4 | Witbier              |  88 |
|  5 | Imperial IPA         |  82 |
|  6 | American Pale Ale    |  77 |
|  7 | Cider                |  72 |
|  8 | Saison               |  61 |
|  9 | Fruit Beer Radler    |  56 |
| 10 | Imperial Stout       |  53 |

For more detail, consult the following interactive chart
(Hyper-categories are determined using the Ratebeer style guide, chart
designed using [Sunburst](https://gist.github.com/metmajer/5480307) ): 

<style>
path {
  stroke: #fff;
  fill-rule: evenodd;
}
text{  
       font-family: Arial, sans-serif;
       font-size:10px;}
</style>
<div id="stylechart"></div>

<script src="http://d3js.org/d3.v3.min.js"></script>
<script>

var width = 600,
    height = 600,
    radius = Math.min(width, height) / 2;

var x = d3.scale.linear()
    .range([0, 2 * Math.PI]);

var y = d3.scale.linear()
    .range([0, radius]);

var color = d3.scale.category20c();

var svg = d3.select("div#stylechart").append("svg")
    .attr("width", width)
    .attr("height", height)
  .append("g")
    .attr("transform", "translate(" + width / 2 + "," + (height / 2) + ")");

var partition = d3.layout.partition()
    .value(function(d) { return d.size; });

var arc = d3.svg.arc()
    .startAngle(function(d) { return Math.max(0, Math.min(2 * Math.PI, x(d.x))); })
    .endAngle(function(d) { return Math.max(0, Math.min(2 * Math.PI, x(d.x + d.dx))); })
    .innerRadius(function(d) { return Math.max(0, y(d.y)); })
    .outerRadius(function(d) { return Math.max(0, y(d.y + d.dy)); });

d3.json("/flare.json", function(error, root) {
  var g = svg.selectAll("g")
      .data(partition.nodes(root))
    .enter().append("g");

  var path = g.append("path")
    .attr("d", arc)
    .style("fill", function(d) { return color((d.children ? d : d.parent).name); })
    .on("click", click);

  var text = g.append("text")
    .attr("transform", function(d) { return "rotate(" + computeTextRotation(d) + ")"; })
    .attr("x", function(d) { return y(d.y); })
    .attr("dx", "6") // margin
    .attr("dy", ".35em") // vertical-align
    .text(function(d) { return d.name; });

  function click(d) {
    // fade out all text elements
    text.transition().attr("opacity", 0);

    path.transition()
      .duration(750)
      .attrTween("d", arcTween(d))
      .each("end", function(e, i) {
          // check if the animated element's data e lies within the visible angle span given in d
          if (e.x >= d.x && e.x < (d.x + d.dx)) {
            // get a selection of the associated text element
            //var arcText = "testing"
            var arcText = d3.select(this.parentNode).select("text");
            // fade in the text element and recalculate positions
            arcText.transition().duration(750)
              .attr("opacity", 1)
              .attr("transform", function() { return "rotate(" + computeTextRotation(e) + ")" })
              .attr("x", function(d) { return y(d.y); });
          }
      });
  }
});

d3.select(self.frameElement).style("height", height + "px");

// Interpolate the scales!
function arcTween(d) {
  var xd = d3.interpolate(x.domain(), [d.x, d.x + d.dx]),
      yd = d3.interpolate(y.domain(), [d.y, 1]),
      yr = d3.interpolate(y.range(), [d.y ? 20 : 0, radius]);
  return function(d, i) {
    return i
        ? function(t) { return arc(d); }
        : function(t) { x.domain(xd(t)); y.domain(yd(t)).range(yr(t)); return arc(d); };
  };
}

function computeTextRotation(d) {
  return (x(d.x + d.dx / 2) - Math.PI / 2) / Math.PI * 180;
}

</script>

<div id="stylechart"></div>

<br/><br/>
Some of these results genuinely surprised me. Keep in mind this data was gathered in
October, so pumpkin and Oktoberfest beers were in full force, as were
ciders. That being said, I didn't think that the effects would have
been quite so prominent.

## Most Common Beers ##

Seeing how popular pumpkin beers were, for example, made me wonder
exactly which beers were the most common overall. Would it be more
pumpkin beers? Well, they're certaintly up there:

|   | Most Common Beers                |  # |
|---+:---------------------------------+---:|
| 1 | Allagash White                   | 39 |
| 2 | Yuengling Lager                  | 36 |
| 3 | Southern Tier Pumking            | 31 |
| 4 | Guinness                         | 20 |
| 5 | Yards Cape of Good Hope          | 18 |
| 6 | Dogfish Head Punkin Ale          | 17 |
| 7 | Firestone Walker Pivo Hoppy Pils | 16 |
| 7 | Founders Breakfast Stout         | 16 |
| 7 | Founders Dark Penance            | 16 |
| 7 | Yards Philadelphia Pale Ale      | 16 |

Here we see some standards: Yuengling (it's Philly after all),
Guinness, and some other local brews (i.e., Yards). Then there are
some seasonal beers: Pumking and Punkin. I hope Allagash White is just
seasonally popular, but honestly it's such a preferable choice to Blue
Moon or Shocktop that I'm not terribly upset. I *am* curious why the Pivo Pils and
the two Founders beers happen to be so commonly stocked. They're great
beers, but I'm still a little curious why those particular beers are
so popular over, say, Sierra Nevada Pale Ale.

## Unique Beers ##

Finally, I decided to look at what bars had beers you couldn't get
anywhere else in Philadelphia. Specifically, by percentage of taps and
by number of taps. First, by percentage:

|    | Bars with highest % of taps only available there |  % |
|----+:-------------------------------------------------+---:|
|  1 | Nodding Head                                     | 71 |
|  2 | The Trestle Inn                                  | 62 |
|  3 | CJ's Doghouse                                    | 58 |
|  4 | Watkins Drinkery                                 | 57 |
|  5 | Bainbridge St. Barrel House                      | 52 |
|  6 | Churchville inn                                  | 50 |
|  6 | Memphis Taproom                                  | 50 |
|  6 | Sancho Pistolas                                  | 50 |
|  9 | Tria Taproom                                     | 46 |
| 10 | The Victoria Freehouse                           | 45 |
| 10 | Varga Bar                                        | 45 |


Things to note: Nodding head is a brewpub: they have such a high
percentage of unique beers because they brew their own stuff. But, as
far as I know, the other bars just have high percentages because
they're well-curated... well... The Victoria Freehouse has 45% unique
beers, but they have the second lowest average average-beer-rating. So
you know where to go if you want low-rated beer you can't find
anywhere else! Actually, that's not entirely fair. The real truth is
they fancy themselves something of an English pub, and thus stock
plenty of hard-to-find beers from the British Isles. This is a cool
idea, but unfortunately a lot of British beer isn't terribly well
rated as it tends to be rather weak and, well, uninteresting. That being
said, they actually have some pretty good roses among their thorns,
including several beers from J.W. Lees and Innis & Gunn. I guess that
means you can't judge a bar by it's average rating. So much for this
post! 

|    | Bars with highest # of taps only available there |  # |
|----+:-------------------------------------------------+---:|
|  1 | City Tap House                                   | 16 |
|  2 | Bru Craft Wurst                                  | 15 |
|  3 | Bainbridge St. Barrel House                      | 13 |
|  4 | McGillin's Olde Ale House                        | 12 |
|  5 | Tria Taproom                                     | 11 |
|  6 | Capone's                                         | 10 |
|  6 | Churchville Inn                                  | 10 |
|  6 | Iron Abbey                                       | 10 |
|  6 | Varga Bar                                        | 10 |
| 10 | Bar-ly Chinatown                                 |  9 |
| 10 | Memphis Taproom                                  |  9 |
| 10 | Moriarty's Pub                                   |  9 |
| 10 | The Cambridge                                    |  9 |

Looking at number of unique taps tells a
slightly different story. This isn't terribly surprising: if you have
enough taps, hopefully you work some unique beers into the mix.

# For Next Time

And that wraps up Part One of my analysis! I've got lots of cool
ideas for further analysis (fueled by reader suggestions) but haven't
had time to look into them yet. For next time, I'll hopefully be able
to look into: 

* Average ABV by bar
* Average IBU by bar
* Average average-beer-rating using /within-style rankings/
* Bars with the most local vs. domestic vs. foreign beer.
* Maps, Maps, Maps!
