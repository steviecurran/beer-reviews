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
  |63649  | Rare D.O.S.  | American Double / Imperial Stout |  NaN   22147   
  44910                  Dirty Horse                Lambic - Unblended       7.0       15237   
  8626  Southampton Berliner Weisse                Berliner Weissbier       2.0        1628   

                                  b \
53419  Peg's Cantina & Brewpub / Cycle Brewing        4.848485            0.091719       4.719697   
37035                      De Struise Brouwers        4.820513            0.092892       4.589744   
7188                 Southampton Publick House        4.768293            0.092306       4.371951   

       +/- review_others  No. reviews  
53419           0.073459           33  
37035           0.081014           39  
7188            0.100824           41  

This is for all beers at 95% confidence. Both the beer style and confidence level can be altered via the dropdown and the slider.

- Which of the factors (aroma, taste, appearance, palette) are most important in determining the overall quality of a beer?

- Lastly, if I typically enjoy a beer due to its aroma and appearance, which beer style should I try?"

Here's my attempt. 

If the remote data are taking too long to load, try the notebook at [Kaggle](https://www.kaggle.com/code/steviemooncat/beer-reviews)

![](https://raw.githubusercontent.com/steviecurran/beer-reviews/refs/heads/main/heatmap.png) ![](https://raw.githubusercontent.com/steviecurran/beer-reviews/refs/heads/main/IMG_1809%20copy.JPG)
