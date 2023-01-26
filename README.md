# assignment2Gollapalli


### my favourite sport is Cricket and team is Indian Cricket team.

**Cricket is not just a sport in india, it is believed to be a religion**. and the most important reason i like is because of the thrill that we get from it. I have my idol **Mr. M.S.Dhoni** sir who plays for indian cricket team, that boosts my interest towards watching or playing cricket.



## Best Indian and Newzealand crciket players, I love watching them playing.
1. Indian cricket team
    1. Sachin tendulkar
    2. M.S.Dhoni
    3. Virat Kohli


* Newzealand Cricket team
    * Devon conway
    * Kane williamson
    * Trent Boult



[Click here to get the details about me](AboutMe.md)


***

# Table for *Contries to visit once in their life time*!

| country | Reasons | Days to spend |
| --- | --- | ---: |
| India | Amazing street food, Temples, breathtaking landscapes and rich history | Life time if possible |
| Thailand | wild nightlife,scrumptious food, winding rivers and canals | 150 Days |
| United states | exciting opportunities to have fun, vibrant cities, innovative gastronomy | 360 Days |
| Italy | glorious landscapes, italian divine food, vibrant culture| 120 days |

***

## Quotes for life.

> “Never underestimate the power of stupid people in large groups.” - *Dwight D. Eisenhower*

> “Only one man in a thousand is a leader of men — the other 999 follow women.” - *Isaac Asimov*


# Code to Get Latest Twitter Status using PHP.

```
<?php

function getTwitterStatus($userid){
$url = "https://api.twitter.com/1/statuses/user_timeline/$userid.xml?count=1&include_rts=1callback=?";

$xml = simplexml_load_file($url) or die("could not connect");

       foreach($xml->status as $status){
       $text = $status->text;
       }
       echo $text;
 }

// USAGE
getTwitterStatus("chriscoyier");

?>

```

[Source code](https://css-tricks.com/snippets/php/get-latest-twitter-status/)