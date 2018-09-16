{:title "Data Science Screencasts from Lambda Island"
 :layout :post
 :author "Henry Garner"
 :tags  ["clojure" "data science" "screencast" "kixi.stats" "xforms" "transduce"]}

[Lambda Island](https://lambdaisland.com/) has produced a high-quality Clojure-focused screencast every few weeks over the past couple of years. [Arne Brasseur](https://twitter.com/plexus) is the author and producer of these videos. To date he's generated diverse walk-throughs on language fundamentals, library APIs, architectural considerations, and development tooling. The most recent two screencasts, numbers 43 & 44, have signalled a move into the realm of data science. Both screencasts make heavy use of [kixi.stats](https://github.com/mastodonC/kixi.stats): a library of statistical reducing functions. As the author of kixi.stats, I'm relieved to say that I think that the topics are dealt with really well.

The screencasts are intended for a broad audience, and the material covered is beginner-friendly. The [first video](https://lambdaisland.com/episodes/clojure-data-science-kixi-stats) could more accurately be titled _"Exploratory data analysis with Clojure's Transducers"_, but in any case this is worthy material for a video of this length. If you want to understand how Clojure's transducers can be used to create summary statistics in a single pass over the data, and how to render empirical distributions to histograms and interpret them, this is a great place to start.

The [second video](https://lambdaisland.com/episodes/clojure-data-science-kixi-stats-2) builds towards the creation of a simple linear model. Along the way, standard data science concerns regarding data scrubbing, feature selection and model evaluation are covered. The screencast also demonstrates how to make use of transducers and composite reducing functions to achieve non-trivial results. For example, at one point we are shown how to create a reducing function which returns a linear model expressed as a function of _x_ and _y_. Chaining a post-complete function to a reducing function to  return a function?! It's functions all the way down!

* [Data Science with Kixi.stats, part 1](https://lambdaisland.com/episodes/clojure-data-science-kixi-stats)
* [Data Science with Kixi.stats, part 2](https://lambdaisland.com/episodes/clojure-data-science-kixi-stats-2)

A free trial is available, and discounts are available for those unable to cover the full fee. Whether or not you decide to subscribe, the code for each episode is freely accessible on GitHub. For example, [here's the code for episode 43](https://github.com/lambdaisland/ep43-data-science-kixi-stats). For me, the graphs namespace is particularly noteworthy because Clojure currently lacks a flexible high-level charting library. As a complete tangent to the main content of his screencasts, Arne has done an excellent job of spiking out a set of functions which could form the basis of such a library. Watch this space...

_Disclosure: Henry was granted free access to Lambda Island in exchange for advising on the content of the episodes linked above._
