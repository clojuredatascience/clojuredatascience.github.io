{:title "Expressive Parallel Analytics with Clojure"
 :layout :post
 :tags  ["clojure" "data science" "statistics" "transducers" "reducers" "talks"]}

[Henry](https://twitter.com/henrygarner) spoke at [Clojure eXchange 2015](https://skillsmatter.com/conferences/6861-clojure-exchange-2015#program) on the subject of parallel folds using Clojure's transducers.

From the programme:

<blockquote><p>
Sharing experience gained from his work on a mission-critical data product earlier this year, Henry will speak about some newer features of Clojure that enable data scientists to write concise, expressive and performant data processing code. He’ll explore transducers and reducing functions, and show how simple functional combinators can make even sophisticated analytical code both faster and easier to comprehend.
</p></blockquote>

The key takeaway is that with transducers, reducing functions must now provide an arity-1 **completer** implementation which provides them with the opportunity to convert an accumulated value into a final output. Together with the (optional) arity-0 **initializer** this provides reducing functions the ability to wrap arbitrarily intricate state. The natural composability of transducers can be mirrored with similarly composable reducing functions to build up sophisticated parallel computations.

You can see a [video of the talk](https://skillsmatter.com/skillscasts/7243-expressive-parallel-analytics-with-clojure) on Skills Matter's website, the [org-mode slides](https://github.com/henrygarner/cljx-december-2015), or a PDF of the presentation below.

<script async class="speakerdeck-embed" data-id="9945344f8783426d8e5fdffc90d5d818" data-ratio="1.37081659973226" src="//speakerdeck.com/assets/embed.js"></script>
