## TBC Analystics Test (Beer Advocate)

**From [How to Hire and Test for Data Skills: a One-Size-Fits-All Interview Kit](https://tcbanalytics.com/2016/01/29/how-to-hire-and-test-for-data-skills-a-one-size-fits-all-interview-kit/)**

"In an effort to make the interviewing experience a bit more fun, we use a dataset that involves beer. This dataset consists of 1.5 million beer reviews from Beer Advocate. It is an ideal dataset for testing candidates since it is too large to fit into Excel, but small enough to process on a single laptop in Python or R. We prefer that candidates complete the test in either Python or R, and generally if they are hesitant about using or trying to learn either of these languages, that should signal a red flag.

- Which brewery produces the strongest beers by ABV%?
  Schorschbräu with a beauty at 57.7%. This brewery also has highest average strength (19.2%), followd by Shoes Brewery at 15.2%.
  
- If you had to pick 3 beers to recommend using only this data, which would you pick?
  Doing this my the maximum average overall score and the averaged maximum of the specific factors and ranking by the lower range of the confidence 
  interval (to wight by mumber of reviews), for all beers:

  | beer_id   | beer_name  | beer_style | beer_abv  |rewery_id  | rewery_name | review_overall | +/- | review_others |+/-| No. reviews|
  | :---       | :---      | :---        | :---     | :---       | :---        | :---          | :--- | :---         | :--- | :---    |
  |63649|Rare D.O.S. | American Double/Imperial Stout| NaN |22147| Peg's Cantina & Brewpub/Cycle Brewing|4.848485 |0.091719 |4.719697 |0.073459|33|  
  44910|Dirty Horse|Lambic - Unblended|7.0|15237|De Struise Brouwers|4.820513|0.092892|0.589744|0.081014|39|
  8626| Southampton Berliner Weisse|Berliner Weissbier|2.0|1628|Southampton Publick House|4.768293|0.092306|4.371951 |0.100824 |41|  

  This is for all beers at 95% confidence. Both the beer style and confidence level can be altered via the dropdown and the slider.

- Which of the factors (aroma, taste, appearance, palette) are most important in determining the overall quality of a beer?

  Taste and palate
  ![](https://raw.githubusercontent.com/steviecurran/beer-reviews/refs/heads/main/heatmap.png) ![]

- Lastly, if I typically enjoy a beer due to its aroma and appearance, which beer style should I try?"

  | beer_id   | beer_name  | beer_style | beer_abv  |rewery_id  | rewery_name | review_overall | +/- | review_others |+/-| No. reviews|
  | :---       | :---      | :---        | :---     | :---       | :---        | :---          | :--- | :---         | :--- | :---    |
  |21690 |Pliny The Younger|American Double/Imperial IPA|17536|11.0|63 |Russian River Brewing Company |4.723770|0.028002|4.482787|0.032832|610|  
  |42349|Vanilla Bean Aged Dark Lord|Russian Imperial Stout|13.0|26|Three Floyds Brewing Co. & Brewpub| 4.717105|0.064031|4.450658|0.066032|152|  
  |63649|Rare D.O.S.  American Double/ mperial Stout|NaN|22147|Peg's Cantina & Brewpub/ ycle Brewing|4.757576|0.107152|4.469697|0.096254|33|  

  Again for all, although style can be selected from a drop down menus, as well as the characeristics.

Here's my attempt. 

If the remote data are taking too long to load, try the notebook at [Kaggle](https://www.kaggle.com/code/steviemooncat/beer-reviews)
