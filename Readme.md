---
jupyter:
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.9.6
  nbformat: 4
  nbformat_minor: 2
  orig_nbformat: 4
  vscode:
    interpreter:
      hash: 31f2aee4e71d21fbe5cf8b01ff0e069b9275f58929596ceb00d14d90e3e16cd6
---

::: {.cell .markdown}
## Exploratory Data Analysis with TED data
:::

::: {.cell .markdown}
### What is EDA?

EDA stands for Exploratory Data Analysis. This analysis is essential to
understand a given dataset. Usually to perform an EDA ,**we are
asking**:

-   What shape does the dataset have?
-   How does the data look like?
-   How many records?
-   How many columns?
-   What is the dataset about?
-   What columns represent?
-   What are the types for each column?

Once we understand the format, we can continue to **business questions
about the dataset**:

-   Is there any question given to answer over this dataset?
-   What information can this dataset provide that is crucial to
    business?
-   What dataset transformations will give us such information/answers?

**Iterate over:**

-   Once an answer is given: what other questions can be asked?
-   What visualization will help understand the dataset/answer this
    question? -Once the visualization is rendered, what is surprising
    about the result?
-   Did the visualization answer our question?
-   Did the visualization bring anything new? What can be inferred?
:::

::: {.cell .markdown}
Kaggle site (datasets) <https://www.kaggle.com/datasets> Recommended to
practice EDA and others Competitions, Models,Discussions, etc
:::

::: {.cell .markdown}
### Credit to the original creator

Credit to \@justmarkham
<https://github.com/justmarkham/pycon-2019-tutorial/blob/master/environment.yml>

I wanted to recreate the jupyter notebook step by step and make it
public as a learning exercise, also adding insight on some points
:::

::: {.cell .markdown}
Dataset <https://github.com/justmarkham/pycon-2019-tutorial>
:::

::: {.cell .markdown}
Pycon session reference <https://www.youtube.com/watch?v=dPwLlJkSHLo>
:::

::: {.cell .markdown}
## Retrieving the dataset to work with it

This one is a dataset containing info on several Ted Talks. Pandas has
built-in features to produce plots that we will be using throughout this
notebook.
:::

::: {.cell .code execution_count="5"}
``` python
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
ted = pd.read_csv('ted.csv')
```
:::

::: {.cell .markdown}
Using pandas features to plot number of comments on the ted dataset. The
ted.comments part makes reference to the column \"comments\" on the
\"ted\" dataframe.
:::

::: {.cell .code execution_count="6"}
``` python
ted.comments.plot()
```

::: {.output .execute_result execution_count="6"}
    <Axes: >
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/c91ece3ced7551ab627fea3a712157546a0e3619.png)
:::
:::

::: {.cell .markdown}
## Pandas version set up
:::

::: {.cell .code execution_count="7"}
``` python
pd.__version__
```

::: {.output .execute_result execution_count="7"}
    '2.0.1'
:::
:::

::: {.cell .markdown}
## TED talks dataset shape analysis
:::

::: {.cell .code execution_count="8"}
``` python
ted = pd.read_csv('ted.csv')
```
:::

::: {.cell .code execution_count="9"}
``` python
ted
```

::: {.output .execute_result execution_count="9"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4553</td>
      <td>Sir Ken Robinson makes an entertaining and pro...</td>
      <td>1164</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>60</td>
      <td>Ken Robinson</td>
      <td>Ken Robinson: Do schools kill creativity?</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 19645}, {...</td>
      <td>[{'id': 865, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Author/educator</td>
      <td>['children', 'creativity', 'culture', 'dance',...</td>
      <td>Do schools kill creativity?</td>
      <td>https://www.ted.com/talks/ken_robinson_says_sc...</td>
      <td>47227110</td>
    </tr>
    <tr>
      <th>1</th>
      <td>265</td>
      <td>With the same humor and humanity he exuded in ...</td>
      <td>977</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>43</td>
      <td>Al Gore</td>
      <td>Al Gore: Averting the climate crisis</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 544}, {'i...</td>
      <td>[{'id': 243, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Climate advocate</td>
      <td>['alternative energy', 'cars', 'climate change...</td>
      <td>Averting the climate crisis</td>
      <td>https://www.ted.com/talks/al_gore_on_averting_...</td>
      <td>3200520</td>
    </tr>
    <tr>
      <th>2</th>
      <td>124</td>
      <td>New York Times columnist David Pogue takes aim...</td>
      <td>1286</td>
      <td>TED2006</td>
      <td>1140739200</td>
      <td>26</td>
      <td>David Pogue</td>
      <td>David Pogue: Simplicity sells</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 964}, {'i...</td>
      <td>[{'id': 1725, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Technology columnist</td>
      <td>['computers', 'entertainment', 'interface desi...</td>
      <td>Simplicity sells</td>
      <td>https://www.ted.com/talks/david_pogue_says_sim...</td>
      <td>1636292</td>
    </tr>
    <tr>
      <th>3</th>
      <td>200</td>
      <td>In an emotionally charged talk, MacArthur-winn...</td>
      <td>1116</td>
      <td>TED2006</td>
      <td>1140912000</td>
      <td>35</td>
      <td>Majora Carter</td>
      <td>Majora Carter: Greening the ghetto</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 760}...</td>
      <td>[{'id': 1041, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Activist for environmental justice</td>
      <td>['MacArthur grant', 'activism', 'business', 'c...</td>
      <td>Greening the ghetto</td>
      <td>https://www.ted.com/talks/majora_carter_s_tale...</td>
      <td>1697550</td>
    </tr>
    <tr>
      <th>4</th>
      <td>593</td>
      <td>You've never seen data presented like this. Wi...</td>
      <td>1190</td>
      <td>TED2006</td>
      <td>1140566400</td>
      <td>48</td>
      <td>Hans Rosling</td>
      <td>Hans Rosling: The best stats you've ever seen</td>
      <td>1</td>
      <td>1151440680</td>
      <td>[{'id': 9, 'name': 'Ingenious', 'count': 3202}...</td>
      <td>[{'id': 2056, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Global health expert; data visionary</td>
      <td>['Africa', 'Asia', 'Google', 'demo', 'economic...</td>
      <td>The best stats you've ever seen</td>
      <td>https://www.ted.com/talks/hans_rosling_shows_t...</td>
      <td>12005869</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2545</th>
      <td>17</td>
      <td>Between 2008 and 2016, the United States depor...</td>
      <td>476</td>
      <td>TED2017</td>
      <td>1496707200</td>
      <td>4</td>
      <td>Duarte Geraldino</td>
      <td>Duarte Geraldino: What we're missing in the de...</td>
      <td>1</td>
      <td>1505851216</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 24},...</td>
      <td>[{'id': 2596, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Journalist</td>
      <td>['TED Residency', 'United States', 'community'...</td>
      <td>What we're missing in the debate about immigra...</td>
      <td>https://www.ted.com/talks/duarte_geraldino_wha...</td>
      <td>450430</td>
    </tr>
    <tr>
      <th>2546</th>
      <td>6</td>
      <td>How can you study Mars without a spaceship? He...</td>
      <td>290</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>3</td>
      <td>Armando Azua-Bustos</td>
      <td>Armando Azua-Bustos: The most Martian place on...</td>
      <td>1</td>
      <td>1505919737</td>
      <td>[{'id': 22, 'name': 'Fascinating', 'count': 32...</td>
      <td>[{'id': 2491, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Astrobiologist</td>
      <td>['Mars', 'South America', 'TED Fellows', 'astr...</td>
      <td>The most Martian place on Earth</td>
      <td>https://www.ted.com/talks/armando_azua_bustos_...</td>
      <td>417470</td>
    </tr>
    <tr>
      <th>2547</th>
      <td>10</td>
      <td>Science fiction visions of the future show us ...</td>
      <td>651</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>1</td>
      <td>Radhika Nagpal</td>
      <td>Radhika Nagpal: What intelligent machines can ...</td>
      <td>1</td>
      <td>1506006095</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 14}, ...</td>
      <td>[{'id': 2346, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Robotics engineer</td>
      <td>['AI', 'ants', 'fish', 'future', 'innovation',...</td>
      <td>What intelligent machines can learn from a sch...</td>
      <td>https://www.ted.com/talks/radhika_nagpal_what_...</td>
      <td>375647</td>
    </tr>
    <tr>
      <th>2548</th>
      <td>32</td>
      <td>In an unmissable talk about race and politics ...</td>
      <td>1100</td>
      <td>TEDxMileHigh</td>
      <td>1499472000</td>
      <td>1</td>
      <td>Theo E.J. Wilson</td>
      <td>Theo E.J. Wilson: A black man goes undercover ...</td>
      <td>1</td>
      <td>1506024042</td>
      <td>[{'id': 11, 'name': 'Longwinded', 'count': 3},...</td>
      <td>[{'id': 2512, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Public intellectual</td>
      <td>['Internet', 'TEDx', 'United States', 'communi...</td>
      <td>A black man goes undercover in the alt-right</td>
      <td>https://www.ted.com/talks/theo_e_j_wilson_a_bl...</td>
      <td>419309</td>
    </tr>
    <tr>
      <th>2549</th>
      <td>8</td>
      <td>With more than half of the world population li...</td>
      <td>519</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>1</td>
      <td>Karoliina Korppoo</td>
      <td>Karoliina Korppoo: How a video game might help...</td>
      <td>1</td>
      <td>1506092422</td>
      <td>[{'id': 21, 'name': 'Unconvincing', 'count': 2...</td>
      <td>[{'id': 2682, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Game designer</td>
      <td>['cities', 'design', 'future', 'infrastructure...</td>
      <td>How a video game might help us build better ci...</td>
      <td>https://www.ted.com/talks/karoliina_korppoo_ho...</td>
      <td>391721</td>
    </tr>
  </tbody>
</table>
<p>2550 rows × 17 columns</p>
</div>
```
:::
:::

::: {.cell .code execution_count="10"}
``` python
ted.head()
```

::: {.output .execute_result execution_count="10"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4553</td>
      <td>Sir Ken Robinson makes an entertaining and pro...</td>
      <td>1164</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>60</td>
      <td>Ken Robinson</td>
      <td>Ken Robinson: Do schools kill creativity?</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 19645}, {...</td>
      <td>[{'id': 865, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Author/educator</td>
      <td>['children', 'creativity', 'culture', 'dance',...</td>
      <td>Do schools kill creativity?</td>
      <td>https://www.ted.com/talks/ken_robinson_says_sc...</td>
      <td>47227110</td>
    </tr>
    <tr>
      <th>1</th>
      <td>265</td>
      <td>With the same humor and humanity he exuded in ...</td>
      <td>977</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>43</td>
      <td>Al Gore</td>
      <td>Al Gore: Averting the climate crisis</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 544}, {'i...</td>
      <td>[{'id': 243, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Climate advocate</td>
      <td>['alternative energy', 'cars', 'climate change...</td>
      <td>Averting the climate crisis</td>
      <td>https://www.ted.com/talks/al_gore_on_averting_...</td>
      <td>3200520</td>
    </tr>
    <tr>
      <th>2</th>
      <td>124</td>
      <td>New York Times columnist David Pogue takes aim...</td>
      <td>1286</td>
      <td>TED2006</td>
      <td>1140739200</td>
      <td>26</td>
      <td>David Pogue</td>
      <td>David Pogue: Simplicity sells</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 964}, {'i...</td>
      <td>[{'id': 1725, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Technology columnist</td>
      <td>['computers', 'entertainment', 'interface desi...</td>
      <td>Simplicity sells</td>
      <td>https://www.ted.com/talks/david_pogue_says_sim...</td>
      <td>1636292</td>
    </tr>
    <tr>
      <th>3</th>
      <td>200</td>
      <td>In an emotionally charged talk, MacArthur-winn...</td>
      <td>1116</td>
      <td>TED2006</td>
      <td>1140912000</td>
      <td>35</td>
      <td>Majora Carter</td>
      <td>Majora Carter: Greening the ghetto</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 760}...</td>
      <td>[{'id': 1041, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Activist for environmental justice</td>
      <td>['MacArthur grant', 'activism', 'business', 'c...</td>
      <td>Greening the ghetto</td>
      <td>https://www.ted.com/talks/majora_carter_s_tale...</td>
      <td>1697550</td>
    </tr>
    <tr>
      <th>4</th>
      <td>593</td>
      <td>You've never seen data presented like this. Wi...</td>
      <td>1190</td>
      <td>TED2006</td>
      <td>1140566400</td>
      <td>48</td>
      <td>Hans Rosling</td>
      <td>Hans Rosling: The best stats you've ever seen</td>
      <td>1</td>
      <td>1151440680</td>
      <td>[{'id': 9, 'name': 'Ingenious', 'count': 3202}...</td>
      <td>[{'id': 2056, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Global health expert; data visionary</td>
      <td>['Africa', 'Asia', 'Google', 'demo', 'economic...</td>
      <td>The best stats you've ever seen</td>
      <td>https://www.ted.com/talks/hans_rosling_shows_t...</td>
      <td>12005869</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="11"}
``` python
ted.shape
```

::: {.output .execute_result execution_count="11"}
    (2550, 17)
:::
:::

::: {.cell .code execution_count="12"}
``` python
ted.dtypes
```

::: {.output .execute_result execution_count="12"}
    comments               int64
    description           object
    duration               int64
    event                 object
    film_date              int64
    languages              int64
    main_speaker          object
    name                  object
    num_speaker            int64
    published_date         int64
    ratings               object
    related_talks         object
    speaker_occupation    object
    tags                  object
    title                 object
    url                   object
    views                  int64
    dtype: object
:::
:::

::: {.cell .markdown}
## Object columns can hold also dictionaries, lists and structures too ( additionally for strings) {#object-columns-can-hold-also-dictionaries-lists-and-structures-too--additionally-for-strings}
:::

::: {.cell .markdown}
1\) What part of this dataset contains useful info? Tell me the sum of
NA records on the dataset
:::

::: {.cell .code execution_count="13"}
``` python
ted.isna().sum()
```

::: {.output .execute_result execution_count="13"}
    comments              0
    description           0
    duration              0
    event                 0
    film_date             0
    languages             0
    main_speaker          0
    name                  0
    num_speaker           0
    published_date        0
    ratings               0
    related_talks         0
    speaker_occupation    6
    tags                  0
    title                 0
    url                   0
    views                 0
    dtype: int64
:::
:::

::: {.cell .markdown}
## Which talks provoke the most online discussion?
:::

::: {.cell .markdown}
In this case we start with a business question: \"*What are the talks
that are more provokative ( produce the most online discussion)*? So
creating a new column that can tell the amount of comments related to
the number of views. We are interested in talks that generate the max
number of comments per view.
:::

::: {.cell .code execution_count="14"}
``` python
ted['comments_per_view'] = ted.comments / ted.views
```
:::

::: {.cell .code execution_count="15"}
``` python
ted.sort_values('comments_per_view').tail()
```

::: {.output .execute_result execution_count="15"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
      <th>comments_per_view</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>954</th>
      <td>2492</td>
      <td>Janet Echelman found her true voice as an arti...</td>
      <td>566</td>
      <td>TED2011</td>
      <td>1299110400</td>
      <td>35</td>
      <td>Janet Echelman</td>
      <td>Janet Echelman: Taking imagination seriously</td>
      <td>1</td>
      <td>1307489760</td>
      <td>[{'id': 23, 'name': 'Jaw-dropping', 'count': 3...</td>
      <td>[{'id': 453, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Artist</td>
      <td>['art', 'cities', 'culture', 'data', 'design',...</td>
      <td>Taking imagination seriously</td>
      <td>https://www.ted.com/talks/janet_echelman</td>
      <td>1832930</td>
      <td>0.001360</td>
    </tr>
    <tr>
      <th>694</th>
      <td>1502</td>
      <td>Filmmaker Sharmeen Obaid-Chinoy takes on a ter...</td>
      <td>489</td>
      <td>TED2010</td>
      <td>1265760000</td>
      <td>32</td>
      <td>Sharmeen Obaid-Chinoy</td>
      <td>Sharmeen Obaid-Chinoy: Inside a school for sui...</td>
      <td>1</td>
      <td>1274865960</td>
      <td>[{'id': 23, 'name': 'Jaw-dropping', 'count': 3...</td>
      <td>[{'id': 171, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Filmmaker</td>
      <td>['TED Fellows', 'children', 'culture', 'film',...</td>
      <td>Inside a school for suicide bombers</td>
      <td>https://www.ted.com/talks/sharmeen_obaid_chino...</td>
      <td>1057238</td>
      <td>0.001421</td>
    </tr>
    <tr>
      <th>96</th>
      <td>6404</td>
      <td>Richard Dawkins urges all atheists to openly s...</td>
      <td>1750</td>
      <td>TED2002</td>
      <td>1012608000</td>
      <td>42</td>
      <td>Richard Dawkins</td>
      <td>Richard Dawkins: Militant atheism</td>
      <td>1</td>
      <td>1176689220</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 3236...</td>
      <td>[{'id': 86, 'hero': 'https://pe.tedcdn.com/ima...</td>
      <td>Evolutionary biologist</td>
      <td>['God', 'atheism', 'culture', 'religion', 'sci...</td>
      <td>Militant atheism</td>
      <td>https://www.ted.com/talks/richard_dawkins_on_m...</td>
      <td>4374792</td>
      <td>0.001464</td>
    </tr>
    <tr>
      <th>803</th>
      <td>834</td>
      <td>David Bismark demos a new system for voting th...</td>
      <td>422</td>
      <td>TEDGlobal 2010</td>
      <td>1279065600</td>
      <td>36</td>
      <td>David Bismark</td>
      <td>David Bismark: E-voting without fraud</td>
      <td>1</td>
      <td>1288685640</td>
      <td>[{'id': 25, 'name': 'OK', 'count': 111}, {'id'...</td>
      <td>[{'id': 803, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Voting system designer</td>
      <td>['culture', 'democracy', 'design', 'global iss...</td>
      <td>E-voting without fraud</td>
      <td>https://www.ted.com/talks/david_bismark_e_voti...</td>
      <td>543551</td>
      <td>0.001534</td>
    </tr>
    <tr>
      <th>744</th>
      <td>649</td>
      <td>Hours before New York lawmakers rejected a key...</td>
      <td>453</td>
      <td>New York State Senate</td>
      <td>1259712000</td>
      <td>0</td>
      <td>Diane J. Savino</td>
      <td>Diane J. Savino: The case for same-sex marriage</td>
      <td>1</td>
      <td>1282062180</td>
      <td>[{'id': 25, 'name': 'OK', 'count': 100}, {'id'...</td>
      <td>[{'id': 217, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Senator</td>
      <td>['God', 'LGBT', 'culture', 'government', 'law'...</td>
      <td>The case for same-sex marriage</td>
      <td>https://www.ted.com/talks/diane_j_savino_the_c...</td>
      <td>292395</td>
      <td>0.002220</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
Views per comment to make it more interpretable
:::

::: {.cell .code execution_count="16"}
``` python
ted.sort_values('comments_per_view').head()
```

::: {.output .execute_result execution_count="16"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
      <th>comments_per_view</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2534</th>
      <td>2</td>
      <td>What the astronauts felt when they saw Earth f...</td>
      <td>725</td>
      <td>TEDxSkoll</td>
      <td>1491523200</td>
      <td>1</td>
      <td>Benjamin Grant</td>
      <td>Benjamin Grant: What it feels like to see Eart...</td>
      <td>1</td>
      <td>1504814438</td>
      <td>[{'id': 10, 'name': 'Inspiring', 'count': 46},...</td>
      <td>[{'id': 2511, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Author</td>
      <td>['TEDx', 'art', 'climate change', 'environment...</td>
      <td>What it feels like to see Earth from space</td>
      <td>https://www.ted.com/talks/benjamin_grant_what_...</td>
      <td>646174</td>
      <td>0.000003</td>
    </tr>
    <tr>
      <th>2501</th>
      <td>3</td>
      <td>Meet Françoise Mouly, The New Yorker's art dir...</td>
      <td>509</td>
      <td>TEDNYC</td>
      <td>1488931200</td>
      <td>12</td>
      <td>Françoise Mouly</td>
      <td>Françoise Mouly: The stories behind The New Yo...</td>
      <td>1</td>
      <td>1501770244</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 10}, {'id...</td>
      <td>[{'id': 2479, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Art editor</td>
      <td>['TEDNYC', 'art', 'creativity', 'culture', 'de...</td>
      <td>The stories behind The New Yorker's iconic covers</td>
      <td>https://www.ted.com/talks/francoise_mouly_the_...</td>
      <td>839040</td>
      <td>0.000004</td>
    </tr>
    <tr>
      <th>2542</th>
      <td>3</td>
      <td>In the century-old statues that occupy Cape To...</td>
      <td>795</td>
      <td>TEDGlobal 2017</td>
      <td>1503792000</td>
      <td>1</td>
      <td>Sethembile Msezane</td>
      <td>Sethembile Msezane: Living sculptures that sta...</td>
      <td>1</td>
      <td>1505488093</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 41}, ...</td>
      <td>[{'id': 2873, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Artist</td>
      <td>['Africa', 'activism', 'art', 'community', 'hi...</td>
      <td>Living sculptures that stand for history's truths</td>
      <td>https://www.ted.com/talks/sethembile_msezane_l...</td>
      <td>542088</td>
      <td>0.000006</td>
    </tr>
    <tr>
      <th>2528</th>
      <td>3</td>
      <td>Digital archaeologist Chance Coughenour is usi...</td>
      <td>717</td>
      <td>TEDxHamburg</td>
      <td>1465344000</td>
      <td>5</td>
      <td>Chance Coughenour</td>
      <td>Chance Coughenour: How your pictures can help ...</td>
      <td>1</td>
      <td>1504209631</td>
      <td>[{'id': 9, 'name': 'Ingenious', 'count': 16}, ...</td>
      <td>[{'id': 2673, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Digital archaeologist</td>
      <td>['TEDx', 'ancient world', 'archaeology', 'cons...</td>
      <td>How your pictures can help reclaim lost history</td>
      <td>https://www.ted.com/talks/chance_coughenour_ho...</td>
      <td>539207</td>
      <td>0.000006</td>
    </tr>
    <tr>
      <th>2494</th>
      <td>7</td>
      <td>Jimmy Lin is developing technologies to catch ...</td>
      <td>730</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>10</td>
      <td>Jimmy Lin</td>
      <td>Jimmy Lin: A simple new blood test that can ca...</td>
      <td>1</td>
      <td>1500994384</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 7}, {...</td>
      <td>[{'id': 2498, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Geneticist</td>
      <td>['DNA', 'TED Fellows', 'biology', 'cancer', 'd...</td>
      <td>A simple new blood test that can catch cancer ...</td>
      <td>https://www.ted.com/talks/jimmy_lin_a_simple_n...</td>
      <td>1005506</td>
      <td>0.000007</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="17"}
``` python
ted['views_per_comment'] = ted.views/ted.comments
```
:::

::: {.cell .code execution_count="18"}
``` python
ted.sort_values('views_per_comment')
```

::: {.output .execute_result execution_count="18"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
      <th>comments_per_view</th>
      <th>views_per_comment</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>744</th>
      <td>649</td>
      <td>Hours before New York lawmakers rejected a key...</td>
      <td>453</td>
      <td>New York State Senate</td>
      <td>1259712000</td>
      <td>0</td>
      <td>Diane J. Savino</td>
      <td>Diane J. Savino: The case for same-sex marriage</td>
      <td>1</td>
      <td>1282062180</td>
      <td>[{'id': 25, 'name': 'OK', 'count': 100}, {'id'...</td>
      <td>[{'id': 217, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Senator</td>
      <td>['God', 'LGBT', 'culture', 'government', 'law'...</td>
      <td>The case for same-sex marriage</td>
      <td>https://www.ted.com/talks/diane_j_savino_the_c...</td>
      <td>292395</td>
      <td>0.002220</td>
      <td>450.531587</td>
    </tr>
    <tr>
      <th>803</th>
      <td>834</td>
      <td>David Bismark demos a new system for voting th...</td>
      <td>422</td>
      <td>TEDGlobal 2010</td>
      <td>1279065600</td>
      <td>36</td>
      <td>David Bismark</td>
      <td>David Bismark: E-voting without fraud</td>
      <td>1</td>
      <td>1288685640</td>
      <td>[{'id': 25, 'name': 'OK', 'count': 111}, {'id'...</td>
      <td>[{'id': 803, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Voting system designer</td>
      <td>['culture', 'democracy', 'design', 'global iss...</td>
      <td>E-voting without fraud</td>
      <td>https://www.ted.com/talks/david_bismark_e_voti...</td>
      <td>543551</td>
      <td>0.001534</td>
      <td>651.739808</td>
    </tr>
    <tr>
      <th>96</th>
      <td>6404</td>
      <td>Richard Dawkins urges all atheists to openly s...</td>
      <td>1750</td>
      <td>TED2002</td>
      <td>1012608000</td>
      <td>42</td>
      <td>Richard Dawkins</td>
      <td>Richard Dawkins: Militant atheism</td>
      <td>1</td>
      <td>1176689220</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 3236...</td>
      <td>[{'id': 86, 'hero': 'https://pe.tedcdn.com/ima...</td>
      <td>Evolutionary biologist</td>
      <td>['God', 'atheism', 'culture', 'religion', 'sci...</td>
      <td>Militant atheism</td>
      <td>https://www.ted.com/talks/richard_dawkins_on_m...</td>
      <td>4374792</td>
      <td>0.001464</td>
      <td>683.134291</td>
    </tr>
    <tr>
      <th>694</th>
      <td>1502</td>
      <td>Filmmaker Sharmeen Obaid-Chinoy takes on a ter...</td>
      <td>489</td>
      <td>TED2010</td>
      <td>1265760000</td>
      <td>32</td>
      <td>Sharmeen Obaid-Chinoy</td>
      <td>Sharmeen Obaid-Chinoy: Inside a school for sui...</td>
      <td>1</td>
      <td>1274865960</td>
      <td>[{'id': 23, 'name': 'Jaw-dropping', 'count': 3...</td>
      <td>[{'id': 171, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Filmmaker</td>
      <td>['TED Fellows', 'children', 'culture', 'film',...</td>
      <td>Inside a school for suicide bombers</td>
      <td>https://www.ted.com/talks/sharmeen_obaid_chino...</td>
      <td>1057238</td>
      <td>0.001421</td>
      <td>703.886818</td>
    </tr>
    <tr>
      <th>954</th>
      <td>2492</td>
      <td>Janet Echelman found her true voice as an arti...</td>
      <td>566</td>
      <td>TED2011</td>
      <td>1299110400</td>
      <td>35</td>
      <td>Janet Echelman</td>
      <td>Janet Echelman: Taking imagination seriously</td>
      <td>1</td>
      <td>1307489760</td>
      <td>[{'id': 23, 'name': 'Jaw-dropping', 'count': 3...</td>
      <td>[{'id': 453, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Artist</td>
      <td>['art', 'cities', 'culture', 'data', 'design',...</td>
      <td>Taking imagination seriously</td>
      <td>https://www.ted.com/talks/janet_echelman</td>
      <td>1832930</td>
      <td>0.001360</td>
      <td>735.525682</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2494</th>
      <td>7</td>
      <td>Jimmy Lin is developing technologies to catch ...</td>
      <td>730</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>10</td>
      <td>Jimmy Lin</td>
      <td>Jimmy Lin: A simple new blood test that can ca...</td>
      <td>1</td>
      <td>1500994384</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 7}, {...</td>
      <td>[{'id': 2498, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Geneticist</td>
      <td>['DNA', 'TED Fellows', 'biology', 'cancer', 'd...</td>
      <td>A simple new blood test that can catch cancer ...</td>
      <td>https://www.ted.com/talks/jimmy_lin_a_simple_n...</td>
      <td>1005506</td>
      <td>0.000007</td>
      <td>143643.714286</td>
    </tr>
    <tr>
      <th>2528</th>
      <td>3</td>
      <td>Digital archaeologist Chance Coughenour is usi...</td>
      <td>717</td>
      <td>TEDxHamburg</td>
      <td>1465344000</td>
      <td>5</td>
      <td>Chance Coughenour</td>
      <td>Chance Coughenour: How your pictures can help ...</td>
      <td>1</td>
      <td>1504209631</td>
      <td>[{'id': 9, 'name': 'Ingenious', 'count': 16}, ...</td>
      <td>[{'id': 2673, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Digital archaeologist</td>
      <td>['TEDx', 'ancient world', 'archaeology', 'cons...</td>
      <td>How your pictures can help reclaim lost history</td>
      <td>https://www.ted.com/talks/chance_coughenour_ho...</td>
      <td>539207</td>
      <td>0.000006</td>
      <td>179735.666667</td>
    </tr>
    <tr>
      <th>2542</th>
      <td>3</td>
      <td>In the century-old statues that occupy Cape To...</td>
      <td>795</td>
      <td>TEDGlobal 2017</td>
      <td>1503792000</td>
      <td>1</td>
      <td>Sethembile Msezane</td>
      <td>Sethembile Msezane: Living sculptures that sta...</td>
      <td>1</td>
      <td>1505488093</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 41}, ...</td>
      <td>[{'id': 2873, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Artist</td>
      <td>['Africa', 'activism', 'art', 'community', 'hi...</td>
      <td>Living sculptures that stand for history's truths</td>
      <td>https://www.ted.com/talks/sethembile_msezane_l...</td>
      <td>542088</td>
      <td>0.000006</td>
      <td>180696.000000</td>
    </tr>
    <tr>
      <th>2501</th>
      <td>3</td>
      <td>Meet Françoise Mouly, The New Yorker's art dir...</td>
      <td>509</td>
      <td>TEDNYC</td>
      <td>1488931200</td>
      <td>12</td>
      <td>Françoise Mouly</td>
      <td>Françoise Mouly: The stories behind The New Yo...</td>
      <td>1</td>
      <td>1501770244</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 10}, {'id...</td>
      <td>[{'id': 2479, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Art editor</td>
      <td>['TEDNYC', 'art', 'creativity', 'culture', 'de...</td>
      <td>The stories behind The New Yorker's iconic covers</td>
      <td>https://www.ted.com/talks/francoise_mouly_the_...</td>
      <td>839040</td>
      <td>0.000004</td>
      <td>279680.000000</td>
    </tr>
    <tr>
      <th>2534</th>
      <td>2</td>
      <td>What the astronauts felt when they saw Earth f...</td>
      <td>725</td>
      <td>TEDxSkoll</td>
      <td>1491523200</td>
      <td>1</td>
      <td>Benjamin Grant</td>
      <td>Benjamin Grant: What it feels like to see Eart...</td>
      <td>1</td>
      <td>1504814438</td>
      <td>[{'id': 10, 'name': 'Inspiring', 'count': 46},...</td>
      <td>[{'id': 2511, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Author</td>
      <td>['TEDx', 'art', 'climate change', 'environment...</td>
      <td>What it feels like to see Earth from space</td>
      <td>https://www.ted.com/talks/benjamin_grant_what_...</td>
      <td>646174</td>
      <td>0.000003</td>
      <td>323087.000000</td>
    </tr>
  </tbody>
</table>
<p>2550 rows × 19 columns</p>
</div>
```
:::
:::

::: {.cell .markdown}
Checking in graphical way the comments distribution. Line plot is the
first choice ( but no the best one) X= index Y= value of the comment
:::

::: {.cell .markdown}
This graph doesn\'t have a time component, line plot is not adequate.
:::

::: {.cell .markdown}
This plot is good, however it doesn\'t provide detail that we can use.
We just see that there are more TED talks that have between 0-1000
comments. We need more detail to make sure this intuition is true.
:::

::: {.cell .markdown}
## Visualization of the comment distribution
:::

::: {.cell .markdown}
A histogram plot is more adequate for frequency distribution
:::

::: {.cell .code execution_count="19"}
``` python
ted.comments.plot(kind='hist')
```

::: {.output .execute_result execution_count="19"}
    <Axes: ylabel='Frequency'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/cd0ebb7bf57429e91abe58ec55b8df94de966249.png)
:::
:::

::: {.cell .markdown}
Vast majority is on the left of 1000, so we would need to filter to
understand more
:::

::: {.cell .markdown}
So what does this look like in detail. Let\'s filter the dataframe by
the ones that have less than 1000
:::

::: {.cell .code execution_count="20"}
``` python
ted[ted.comments>=1000].shape
```

::: {.output .execute_result execution_count="20"}
    (32, 19)
:::
:::

::: {.cell .markdown}
By removing the ted talks with more than 1000 comments we cut out
information that is not relevant to the question asked. Just 32 records!
:::

::: {.cell .markdown}
This is the distribution of the ted talks within the ones with less than
1000 comments
:::

::: {.cell .code execution_count="21"}
``` python
ted[ted.comments<1000].comments.plot(kind='hist')
```

::: {.output .execute_result execution_count="21"}
    <Axes: ylabel='Frequency'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/26525c593f0fdf20b337cac4b3db29811c569c26.png)
:::
:::

::: {.cell .markdown}
Same result using query:
:::

::: {.cell .code execution_count="22"}
``` python
ted.query('comments<1000 ').comments.plot(kind='hist')
```

::: {.output .execute_result execution_count="22"}
    <Axes: ylabel='Frequency'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/26525c593f0fdf20b337cac4b3db29811c569c26.png)
:::
:::

::: {.cell .markdown}
Same result but using loc:
:::

::: {.cell .code execution_count="23"}
``` python
ted.loc[ ted.comments<1000,'comments' ].plot(kind='hist')
```

::: {.output .execute_result execution_count="23"}
    <Axes: ylabel='Frequency'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/26525c593f0fdf20b337cac4b3db29811c569c26.png)
:::
:::

::: {.cell .markdown}
Changing the number of bins:
:::

::: {.cell .markdown}
## Plot the number of talks that took place each year
:::

::: {.cell .code execution_count="24"}
``` python
ted.dtypes
```

::: {.output .execute_result execution_count="24"}
    comments                int64
    description            object
    duration                int64
    event                  object
    film_date               int64
    languages               int64
    main_speaker           object
    name                   object
    num_speaker             int64
    published_date          int64
    ratings                object
    related_talks          object
    speaker_occupation     object
    tags                   object
    title                  object
    url                    object
    views                   int64
    comments_per_view     float64
    views_per_comment     float64
    dtype: object
:::
:::

::: {.cell .code execution_count="25"}
``` python
ted
```

::: {.output .execute_result execution_count="25"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>description</th>
      <th>duration</th>
      <th>event</th>
      <th>film_date</th>
      <th>languages</th>
      <th>main_speaker</th>
      <th>name</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>ratings</th>
      <th>related_talks</th>
      <th>speaker_occupation</th>
      <th>tags</th>
      <th>title</th>
      <th>url</th>
      <th>views</th>
      <th>comments_per_view</th>
      <th>views_per_comment</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>4553</td>
      <td>Sir Ken Robinson makes an entertaining and pro...</td>
      <td>1164</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>60</td>
      <td>Ken Robinson</td>
      <td>Ken Robinson: Do schools kill creativity?</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 19645}, {...</td>
      <td>[{'id': 865, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Author/educator</td>
      <td>['children', 'creativity', 'culture', 'dance',...</td>
      <td>Do schools kill creativity?</td>
      <td>https://www.ted.com/talks/ken_robinson_says_sc...</td>
      <td>47227110</td>
      <td>0.000096</td>
      <td>10372.745443</td>
    </tr>
    <tr>
      <th>1</th>
      <td>265</td>
      <td>With the same humor and humanity he exuded in ...</td>
      <td>977</td>
      <td>TED2006</td>
      <td>1140825600</td>
      <td>43</td>
      <td>Al Gore</td>
      <td>Al Gore: Averting the climate crisis</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 544}, {'i...</td>
      <td>[{'id': 243, 'hero': 'https://pe.tedcdn.com/im...</td>
      <td>Climate advocate</td>
      <td>['alternative energy', 'cars', 'climate change...</td>
      <td>Averting the climate crisis</td>
      <td>https://www.ted.com/talks/al_gore_on_averting_...</td>
      <td>3200520</td>
      <td>0.000083</td>
      <td>12077.433962</td>
    </tr>
    <tr>
      <th>2</th>
      <td>124</td>
      <td>New York Times columnist David Pogue takes aim...</td>
      <td>1286</td>
      <td>TED2006</td>
      <td>1140739200</td>
      <td>26</td>
      <td>David Pogue</td>
      <td>David Pogue: Simplicity sells</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 7, 'name': 'Funny', 'count': 964}, {'i...</td>
      <td>[{'id': 1725, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Technology columnist</td>
      <td>['computers', 'entertainment', 'interface desi...</td>
      <td>Simplicity sells</td>
      <td>https://www.ted.com/talks/david_pogue_says_sim...</td>
      <td>1636292</td>
      <td>0.000076</td>
      <td>13195.903226</td>
    </tr>
    <tr>
      <th>3</th>
      <td>200</td>
      <td>In an emotionally charged talk, MacArthur-winn...</td>
      <td>1116</td>
      <td>TED2006</td>
      <td>1140912000</td>
      <td>35</td>
      <td>Majora Carter</td>
      <td>Majora Carter: Greening the ghetto</td>
      <td>1</td>
      <td>1151367060</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 760}...</td>
      <td>[{'id': 1041, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Activist for environmental justice</td>
      <td>['MacArthur grant', 'activism', 'business', 'c...</td>
      <td>Greening the ghetto</td>
      <td>https://www.ted.com/talks/majora_carter_s_tale...</td>
      <td>1697550</td>
      <td>0.000118</td>
      <td>8487.750000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>593</td>
      <td>You've never seen data presented like this. Wi...</td>
      <td>1190</td>
      <td>TED2006</td>
      <td>1140566400</td>
      <td>48</td>
      <td>Hans Rosling</td>
      <td>Hans Rosling: The best stats you've ever seen</td>
      <td>1</td>
      <td>1151440680</td>
      <td>[{'id': 9, 'name': 'Ingenious', 'count': 3202}...</td>
      <td>[{'id': 2056, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Global health expert; data visionary</td>
      <td>['Africa', 'Asia', 'Google', 'demo', 'economic...</td>
      <td>The best stats you've ever seen</td>
      <td>https://www.ted.com/talks/hans_rosling_shows_t...</td>
      <td>12005869</td>
      <td>0.000049</td>
      <td>20245.984823</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2545</th>
      <td>17</td>
      <td>Between 2008 and 2016, the United States depor...</td>
      <td>476</td>
      <td>TED2017</td>
      <td>1496707200</td>
      <td>4</td>
      <td>Duarte Geraldino</td>
      <td>Duarte Geraldino: What we're missing in the de...</td>
      <td>1</td>
      <td>1505851216</td>
      <td>[{'id': 3, 'name': 'Courageous', 'count': 24},...</td>
      <td>[{'id': 2596, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Journalist</td>
      <td>['TED Residency', 'United States', 'community'...</td>
      <td>What we're missing in the debate about immigra...</td>
      <td>https://www.ted.com/talks/duarte_geraldino_wha...</td>
      <td>450430</td>
      <td>0.000038</td>
      <td>26495.882353</td>
    </tr>
    <tr>
      <th>2546</th>
      <td>6</td>
      <td>How can you study Mars without a spaceship? He...</td>
      <td>290</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>3</td>
      <td>Armando Azua-Bustos</td>
      <td>Armando Azua-Bustos: The most Martian place on...</td>
      <td>1</td>
      <td>1505919737</td>
      <td>[{'id': 22, 'name': 'Fascinating', 'count': 32...</td>
      <td>[{'id': 2491, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Astrobiologist</td>
      <td>['Mars', 'South America', 'TED Fellows', 'astr...</td>
      <td>The most Martian place on Earth</td>
      <td>https://www.ted.com/talks/armando_azua_bustos_...</td>
      <td>417470</td>
      <td>0.000014</td>
      <td>69578.333333</td>
    </tr>
    <tr>
      <th>2547</th>
      <td>10</td>
      <td>Science fiction visions of the future show us ...</td>
      <td>651</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>1</td>
      <td>Radhika Nagpal</td>
      <td>Radhika Nagpal: What intelligent machines can ...</td>
      <td>1</td>
      <td>1506006095</td>
      <td>[{'id': 1, 'name': 'Beautiful', 'count': 14}, ...</td>
      <td>[{'id': 2346, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Robotics engineer</td>
      <td>['AI', 'ants', 'fish', 'future', 'innovation',...</td>
      <td>What intelligent machines can learn from a sch...</td>
      <td>https://www.ted.com/talks/radhika_nagpal_what_...</td>
      <td>375647</td>
      <td>0.000027</td>
      <td>37564.700000</td>
    </tr>
    <tr>
      <th>2548</th>
      <td>32</td>
      <td>In an unmissable talk about race and politics ...</td>
      <td>1100</td>
      <td>TEDxMileHigh</td>
      <td>1499472000</td>
      <td>1</td>
      <td>Theo E.J. Wilson</td>
      <td>Theo E.J. Wilson: A black man goes undercover ...</td>
      <td>1</td>
      <td>1506024042</td>
      <td>[{'id': 11, 'name': 'Longwinded', 'count': 3},...</td>
      <td>[{'id': 2512, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Public intellectual</td>
      <td>['Internet', 'TEDx', 'United States', 'communi...</td>
      <td>A black man goes undercover in the alt-right</td>
      <td>https://www.ted.com/talks/theo_e_j_wilson_a_bl...</td>
      <td>419309</td>
      <td>0.000076</td>
      <td>13103.406250</td>
    </tr>
    <tr>
      <th>2549</th>
      <td>8</td>
      <td>With more than half of the world population li...</td>
      <td>519</td>
      <td>TED2017</td>
      <td>1492992000</td>
      <td>1</td>
      <td>Karoliina Korppoo</td>
      <td>Karoliina Korppoo: How a video game might help...</td>
      <td>1</td>
      <td>1506092422</td>
      <td>[{'id': 21, 'name': 'Unconvincing', 'count': 2...</td>
      <td>[{'id': 2682, 'hero': 'https://pe.tedcdn.com/i...</td>
      <td>Game designer</td>
      <td>['cities', 'design', 'future', 'infrastructure...</td>
      <td>How a video game might help us build better ci...</td>
      <td>https://www.ted.com/talks/karoliina_korppoo_ho...</td>
      <td>391721</td>
      <td>0.000020</td>
      <td>48965.125000</td>
    </tr>
  </tbody>
</table>
<p>2550 rows × 19 columns</p>
</div>
```
:::
:::

::: {.cell .markdown}
## Displaying by column
:::

::: {.cell .code execution_count="26"}
``` python
ted.published_date
```

::: {.output .execute_result execution_count="26"}
    0       1151367060
    1       1151367060
    2       1151367060
    3       1151367060
    4       1151440680
               ...    
    2545    1505851216
    2546    1505919737
    2547    1506006095
    2548    1506024042
    2549    1506092422
    Name: published_date, Length: 2550, dtype: int64
:::
:::

::: {.cell .markdown}
1.  Showing a sample of 30 elements of the column \"event\" to check if
    it contains the year
:::

::: {.cell .code execution_count="27"}
``` python
ted.event.sample(30)
```

::: {.output .execute_result execution_count="27"}
    493                     TED2009
    1556             TEDGlobal 2013
    929                 TEDxCaltech
    292                     TED2002
    1150             TEDGlobal 2011
    2126       TEDxAmoskeagMillyard
    768                  TED@Cannes
    752         Mission Blue Voyage
    307                     TED2006
    510              TEDGlobal 2009
    2435             TEDxSanQuentin
    819                 TEDxMidwest
    2105              TEDWomen 2015
    84                      TED2005
    129              TEDGlobal 2007
    170                     TED2007
    218              TEDGlobal 2007
    912                     TED2011
    2022            TEDGlobalLondon
    1746             TEDActive 2014
    1818       TEDSalon Berlin 2014
    1309             TEDGlobal 2012
    1883           TEDxBeaconStreet
    1492                    TED2013
    1245                 TEDxSummit
    932                     TED2011
    2015                    TED2015
    911            TEDxToronto 2010
    1902    TED@State Street London
    1069           TEDxBoulder 2011
    Name: event, dtype: object
:::
:::

::: {.cell .markdown}
Unfortunately the date is not in date format, but as a timestamp, we
require converting to date.
:::

::: {.cell .code execution_count="28"}
``` python
ted.film_date
```

::: {.output .execute_result execution_count="28"}
    0       1140825600
    1       1140825600
    2       1140739200
    3       1140912000
    4       1140566400
               ...    
    2545    1496707200
    2546    1492992000
    2547    1492992000
    2548    1499472000
    2549    1492992000
    Name: film_date, Length: 2550, dtype: int64
:::
:::

::: {.cell .markdown}
## Using datetime transformations
:::

::: {.cell .code execution_count="29"}
``` python
pd.to_datetime(ted.published_date)
```

::: {.output .execute_result execution_count="29"}
    0      1970-01-01 00:00:01.151367060
    1      1970-01-01 00:00:01.151367060
    2      1970-01-01 00:00:01.151367060
    3      1970-01-01 00:00:01.151367060
    4      1970-01-01 00:00:01.151440680
                        ...             
    2545   1970-01-01 00:00:01.505851216
    2546   1970-01-01 00:00:01.505919737
    2547   1970-01-01 00:00:01.506006095
    2548   1970-01-01 00:00:01.506024042
    2549   1970-01-01 00:00:01.506092422
    Name: published_date, Length: 2550, dtype: datetime64[ns]
:::
:::

::: {.cell .code execution_count="30"}
``` python
pd.to_datetime(ted.published_date, unit='s')
```

::: {.output .execute_result execution_count="30"}
    0      2006-06-27 00:11:00
    1      2006-06-27 00:11:00
    2      2006-06-27 00:11:00
    3      2006-06-27 00:11:00
    4      2006-06-27 20:38:00
                   ...        
    2545   2017-09-19 20:00:16
    2546   2017-09-20 15:02:17
    2547   2017-09-21 15:01:35
    2548   2017-09-21 20:00:42
    2549   2017-09-22 15:00:22
    Name: published_date, Length: 2550, dtype: datetime64[ns]
:::
:::

::: {.cell .markdown}
The unit parameter is crucial for the conversion to be correct.
:::

::: {.cell .code execution_count="31"}
``` python
ted['film_datetime']= pd.to_datetime(ted.published_date, unit='s')
```
:::

::: {.cell .markdown}
Reviewing that the data makes sense comparing with event name
:::

::: {.cell .code execution_count="32"}
``` python
ted.film_datetime
```

::: {.output .execute_result execution_count="32"}
    0      2006-06-27 00:11:00
    1      2006-06-27 00:11:00
    2      2006-06-27 00:11:00
    3      2006-06-27 00:11:00
    4      2006-06-27 20:38:00
                   ...        
    2545   2017-09-19 20:00:16
    2546   2017-09-20 15:02:17
    2547   2017-09-21 15:01:35
    2548   2017-09-21 20:00:42
    2549   2017-09-22 15:00:22
    Name: film_datetime, Length: 2550, dtype: datetime64[ns]
:::
:::

::: {.cell .code execution_count="33"}
``` python
ted[['event','film_datetime']].sample(25)
```

::: {.output .execute_result execution_count="33"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>event</th>
      <th>film_datetime</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1693</th>
      <td>TED Fellows Retreat 2013</td>
      <td>2014-03-06 16:01:23</td>
    </tr>
    <tr>
      <th>1985</th>
      <td>TED2015</td>
      <td>2015-05-28 15:21:08</td>
    </tr>
    <tr>
      <th>1136</th>
      <td>TEDxCanberra</td>
      <td>2012-02-07 16:08:24</td>
    </tr>
    <tr>
      <th>283</th>
      <td>TED2008</td>
      <td>2008-09-02 01:00:00</td>
    </tr>
    <tr>
      <th>1784</th>
      <td>TEDGlobal 2013</td>
      <td>2014-07-09 14:51:35</td>
    </tr>
    <tr>
      <th>94</th>
      <td>TED2003</td>
      <td>2007-04-14 21:40:00</td>
    </tr>
    <tr>
      <th>1551</th>
      <td>TEDxCERN</td>
      <td>2013-07-22 15:12:18</td>
    </tr>
    <tr>
      <th>1314</th>
      <td>TEDxHousesOfParliament</td>
      <td>2012-08-12 15:13:23</td>
    </tr>
    <tr>
      <th>250</th>
      <td>TED2008</td>
      <td>2008-06-30 10:52:00</td>
    </tr>
    <tr>
      <th>2122</th>
      <td>TEDWomen 2015</td>
      <td>2016-01-21 15:49:36</td>
    </tr>
    <tr>
      <th>2246</th>
      <td>TEDSummit</td>
      <td>2016-07-13 15:00:19</td>
    </tr>
    <tr>
      <th>2182</th>
      <td>TED2015</td>
      <td>2016-04-12 14:41:40</td>
    </tr>
    <tr>
      <th>2036</th>
      <td>TEDGlobal 2014</td>
      <td>2015-08-31 14:57:59</td>
    </tr>
    <tr>
      <th>697</th>
      <td>TEDxNYED</td>
      <td>2010-05-31 11:13:00</td>
    </tr>
    <tr>
      <th>529</th>
      <td>TEDxUSC</td>
      <td>2009-10-06 01:00:00</td>
    </tr>
    <tr>
      <th>1994</th>
      <td>TED2015</td>
      <td>2015-06-11 15:37:45</td>
    </tr>
    <tr>
      <th>2044</th>
      <td>TED2015</td>
      <td>2015-09-14 15:32:00</td>
    </tr>
    <tr>
      <th>943</th>
      <td>TED2011</td>
      <td>2011-05-24 14:54:00</td>
    </tr>
    <tr>
      <th>1471</th>
      <td>TED2013</td>
      <td>2013-04-04 14:56:21</td>
    </tr>
    <tr>
      <th>2178</th>
      <td>TED2016</td>
      <td>2016-04-07 15:03:12</td>
    </tr>
    <tr>
      <th>1623</th>
      <td>TEDCity2.0</td>
      <td>2013-11-13 15:59:49</td>
    </tr>
    <tr>
      <th>2155</th>
      <td>TEDGlobal&gt;Geneva</td>
      <td>2016-03-08 16:05:54</td>
    </tr>
    <tr>
      <th>2543</th>
      <td>TED2017</td>
      <td>2017-09-18 15:14:47</td>
    </tr>
    <tr>
      <th>2506</th>
      <td>TEDxMileHigh</td>
      <td>2017-08-10 14:37:43</td>
    </tr>
    <tr>
      <th>2113</th>
      <td>TEDxMarin</td>
      <td>2016-01-07 16:40:18</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
Some of the records don\'t match exactly, however the most part do. We
take it as we have the right info for the film date.
:::

::: {.cell .code execution_count="34"}
``` python
ted.dtypes
```

::: {.output .execute_result execution_count="34"}
    comments                       int64
    description                   object
    duration                       int64
    event                         object
    film_date                      int64
    languages                      int64
    main_speaker                  object
    name                          object
    num_speaker                    int64
    published_date                 int64
    ratings                       object
    related_talks                 object
    speaker_occupation            object
    tags                          object
    title                         object
    url                           object
    views                          int64
    comments_per_view            float64
    views_per_comment            float64
    film_datetime         datetime64[ns]
    dtype: object
:::
:::

::: {.cell .markdown}
film_datetime has datetime64\[ns\] . This allows us to use a namespace
\"dt\" with Pandas. For example:
:::

::: {.cell .code execution_count="35"}
``` python
ted.film_datetime.dt.year
```

::: {.output .execute_result execution_count="35"}
    0       2006
    1       2006
    2       2006
    3       2006
    4       2006
            ... 
    2545    2017
    2546    2017
    2547    2017
    2548    2017
    2549    2017
    Name: film_datetime, Length: 2550, dtype: int32
:::
:::

::: {.cell .markdown}
From that point on, we can use agregations like \"value_counts()\".
Below a sentence that can bring the year and the number of values that
contain that year on the dataset.
:::

::: {.cell .code execution_count="36"}
``` python
ted.film_datetime.dt.year.value_counts()
```

::: {.output .execute_result execution_count="36"}
    film_datetime
    2012    306
    2011    261
    2010    257
    2013    244
    2016    243
    2014    240
    2009    222
    2015    220
    2017    197
    2008    188
    2007    122
    2006     50
    Name: count, dtype: int64
:::
:::

::: {.cell .markdown}
We can build a plot just calling it at the end of the sentence.
:::

::: {.cell .code execution_count="37"}
``` python
ted.film_datetime.dt.year.value_counts().plot()
```

::: {.output .execute_result execution_count="37"}
    <Axes: xlabel='film_datetime'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/4d20f2b009ba6862b7e3899018dac25f326bd7e9.png)
:::
:::

::: {.cell .markdown}
What can be concluded from the plot?
:::

::: {.cell .markdown}
Not much since the data is not ordered. Pandas will show them by default
in the order in which they appear.
:::

::: {.cell .code execution_count="38"}
``` python
ted.film_datetime.dt.year.value_counts().sort_index().plot()
```

::: {.output .execute_result execution_count="38"}
    <Axes: xlabel='film_datetime'>
:::

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/2d372d13a157fd3395e0e77fb56353c3eeac7be6.png)
:::
:::

::: {.cell .markdown}
It makes more sense.
:::

::: {.cell .code execution_count="39"}
``` python
ted.film_datetime.dt.day_of_year
```

::: {.output .execute_result execution_count="39"}
    0       178
    1       178
    2       178
    3       178
    4       178
           ... 
    2545    262
    2546    263
    2547    264
    2548    264
    2549    265
    Name: film_datetime, Length: 2550, dtype: int32
:::
:::

::: {.cell .markdown}
Other namespaces by the type of the column
:::

::: {.cell .code execution_count="40"}
``` python
ted.event.str.lower()
```

::: {.output .execute_result execution_count="40"}
    0            ted2006
    1            ted2006
    2            ted2006
    3            ted2006
    4            ted2006
                ...     
    2545         ted2017
    2546         ted2017
    2547         ted2017
    2548    tedxmilehigh
    2549         ted2017
    Name: event, Length: 2550, dtype: object
:::
:::

::: {.cell .markdown}
Is the number of talks in steep decline?
:::

::: {.cell .code execution_count="41"}
``` python
ted[ted.film_datetime.dt.year =='2017'].value_counts()
```

::: {.output .execute_result execution_count="41"}
    Series([], Name: count, dtype: int64)
:::
:::

::: {.cell .code execution_count="42"}
``` python
ted[ted.film_datetime.dt.year==2017].film_datetime.dt.year.value_counts()
```

::: {.output .execute_result execution_count="42"}
    film_datetime
    2017    197
    Name: count, dtype: int64
:::
:::

::: {.cell .code execution_count="43"}
``` python
ted[ted.film_datetime.dt.year==2016].film_datetime.dt.year.value_counts()
```

::: {.output .execute_result execution_count="43"}
    film_datetime
    2016    243
    Name: count, dtype: int64
:::
:::

::: {.cell .markdown}
Are TED talks on steep decline on 2017? No, maybe the dataset is missing
data from 2017 an onwards.

**Sometimes it is convenient to removing data from the dataset so the
conclusions are relevant**
:::

::: {.cell .markdown}
## What were the \"best\" events in TED history to attend?
:::

::: {.cell .markdown}
# Exercise 1. {#exercise-1}
:::

::: {.cell .markdown}
1.  How can we measure event/talk quality?

Let\'s use number of views for a talk as a measure of quality. The event
with the greatest number of views in its talks is the best event.

**We have to consider that an event is a aggregation of talks.**
:::

::: {.cell .markdown}
## Using aggregations with Pandas

-   groupby over a column
-   For each category you can call an aggregate function ( \'mean\' in
    this case)
-   You can later sort by value or sort by index
:::

::: {.cell .markdown}
The code shown below means to sort the events which talks have the least
amount of views (mean).
:::

::: {.cell .code execution_count="44"}
``` python
ted.groupby('event').views.mean().sort_values().head()
```

::: {.output .execute_result execution_count="44"}
    event
    The Do Lectures           112321.0
    TEDxIslay                 120274.0
    TEDxWaterloo              138812.0
    AORN Congress             149818.0
    TEDxNASA@SiliconValley    155895.0
    Name: views, dtype: float64
:::
:::

::: {.cell .markdown}
The code shown below means to sort the events which talks have the
highest amount views (mean).
:::

::: {.cell .markdown}
1.  Group by event 2.For each event 3.Aggregation = mean 4.Column =
    views
:::

::: {.cell .code execution_count="45"}
``` python
ted.groupby('event').views.mean().sort_values().tail()
```

::: {.output .execute_result execution_count="45"}
    event
    TEDxNorrkoping        6569493.0
    TEDxCreativeCoast     8444981.0
    TEDxBloomington       9484259.5
    TEDxHouston          16140250.5
    TEDxPuget Sound      34309432.0
    Name: views, dtype: float64
:::
:::

::: {.cell .markdown}
However we would like to detail more: maybe an event had a few
successful talks
:::

::: {.cell .markdown}
TEDExPugetSound looks like a great event, but let\'s break it down to
see the talks per event. We need to group by two columns:

1.  We need 2 different aggregations
:::

::: {.cell .markdown}
## Using multiple aggregation functions
:::

::: {.cell .code execution_count="46"}
``` python
ted.groupby('event').views.agg(['count','mean']).sort_values('mean').tail()
```

::: {.output .execute_result execution_count="46"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>count</th>
      <th>mean</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>TEDxNorrkoping</th>
      <td>1</td>
      <td>6569493.0</td>
    </tr>
    <tr>
      <th>TEDxCreativeCoast</th>
      <td>1</td>
      <td>8444981.0</td>
    </tr>
    <tr>
      <th>TEDxBloomington</th>
      <td>2</td>
      <td>9484259.5</td>
    </tr>
    <tr>
      <th>TEDxHouston</th>
      <td>2</td>
      <td>16140250.5</td>
    </tr>
    <tr>
      <th>TEDxPuget Sound</th>
      <td>1</td>
      <td>34309432.0</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
We see TEDxPuget Sound had just one talk (or at least one that was
published), and maybe that one was a really good one.

Adding \'sum\' to the agg functions, to see **what events had the most
total number of views**
:::

::: {.cell .code execution_count="47"}
``` python
ted.groupby('event').views.agg(['count','mean','sum']).sort_values('sum').tail()
```

::: {.output .execute_result execution_count="47"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>count</th>
      <th>mean</th>
      <th>sum</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>TED2006</th>
      <td>45</td>
      <td>3.274345e+06</td>
      <td>147345533</td>
    </tr>
    <tr>
      <th>TED2015</th>
      <td>75</td>
      <td>2.011017e+06</td>
      <td>150826305</td>
    </tr>
    <tr>
      <th>TEDGlobal 2013</th>
      <td>66</td>
      <td>2.584163e+06</td>
      <td>170554736</td>
    </tr>
    <tr>
      <th>TED2014</th>
      <td>84</td>
      <td>2.072874e+06</td>
      <td>174121423</td>
    </tr>
    <tr>
      <th>TED2013</th>
      <td>77</td>
      <td>2.302700e+06</td>
      <td>177307937</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
## Conclusions

1.  Think about how to use data creatively
2.  Think about the disavantages of your approach.
3.  Using small sample sizes
:::

::: {.cell .code}
``` python
```
:::

::: {.cell .markdown}
## Unpack ratings data
:::

::: {.cell .markdown}
Ratings data is in a stringified json format, so it needs \"unpacking\"
in a way that we can work with this data.
:::

::: {.cell .code execution_count="48"}
``` python
ted.ratings.head()
```

::: {.output .execute_result execution_count="48"}
    0    [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
    1    [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
    2    [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
    3    [{'id': 3, 'name': 'Courageous', 'count': 760}...
    4    [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
    Name: ratings, dtype: object
:::
:::

::: {.cell .markdown}
## Evaluate a string in a given object format and return as the object it is formatted like
:::

::: {.cell .code execution_count="49"}
``` python
import ast
```
:::

::: {.cell .markdown}
This library can be used to describe a stringified list and retrieve it
as a list object
:::

::: {.cell .code execution_count="50"}
``` python
ast.literal_eval('[1,2,3]')
```

::: {.output .execute_result execution_count="50"}
    [1, 2, 3]
:::
:::

::: {.cell .code execution_count="51"}
``` python
ted.ratings
```

::: {.output .execute_result execution_count="51"}
    0       [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
    1       [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
    2       [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
    3       [{'id': 3, 'name': 'Courageous', 'count': 760}...
    4       [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
                                  ...                        
    2545    [{'id': 3, 'name': 'Courageous', 'count': 24},...
    2546    [{'id': 22, 'name': 'Fascinating', 'count': 32...
    2547    [{'id': 1, 'name': 'Beautiful', 'count': 14}, ...
    2548    [{'id': 11, 'name': 'Longwinded', 'count': 3},...
    2549    [{'id': 21, 'name': 'Unconvincing', 'count': 2...
    Name: ratings, Length: 2550, dtype: object
:::
:::

::: {.cell .code execution_count="52"}
``` python
type(ted.ratings)
```

::: {.output .execute_result execution_count="52"}
    pandas.core.series.Series
:::
:::

::: {.cell .code execution_count="53"}
``` python
type(ted.ratings[0])
```

::: {.output .execute_result execution_count="53"}
    str
:::
:::

::: {.cell .code execution_count="54"}
``` python
ast.literal_eval(ted.ratings[0])
```

::: {.output .execute_result execution_count="54"}
    [{'id': 7, 'name': 'Funny', 'count': 19645},
     {'id': 1, 'name': 'Beautiful', 'count': 4573},
     {'id': 9, 'name': 'Ingenious', 'count': 6073},
     {'id': 3, 'name': 'Courageous', 'count': 3253},
     {'id': 11, 'name': 'Longwinded', 'count': 387},
     {'id': 2, 'name': 'Confusing', 'count': 242},
     {'id': 8, 'name': 'Informative', 'count': 7346},
     {'id': 22, 'name': 'Fascinating', 'count': 10581},
     {'id': 21, 'name': 'Unconvincing', 'count': 300},
     {'id': 24, 'name': 'Persuasive', 'count': 10704},
     {'id': 23, 'name': 'Jaw-dropping', 'count': 4439},
     {'id': 25, 'name': 'OK', 'count': 1174},
     {'id': 26, 'name': 'Obnoxious', 'count': 209},
     {'id': 10, 'name': 'Inspiring', 'count': 24924}]
:::
:::

::: {.cell .code execution_count="55"}
``` python
type(ast.literal_eval(ted.ratings[0]))
```

::: {.output .execute_result execution_count="55"}
    list
:::
:::

::: {.cell .markdown}
Creating a function to encapsulate this
:::

::: {.cell .code execution_count="56"}
``` python
def  str_to_list(ratings_list):
    return ast.literal_eval(ratings_list)
```
:::

::: {.cell .markdown}
So that we can apply this function to this field on the dataframe
:::

::: {.cell .code execution_count="57"}
``` python
ted ['ratings_list']=ted.ratings.apply( lambda x: ast.literal_eval(x))
```
:::

::: {.cell .code execution_count="58"}
``` python
ted.ratings_list
```

::: {.output .execute_result execution_count="58"}
    0       [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
    1       [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
    2       [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
    3       [{'id': 3, 'name': 'Courageous', 'count': 760}...
    4       [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
                                  ...                        
    2545    [{'id': 3, 'name': 'Courageous', 'count': 24},...
    2546    [{'id': 22, 'name': 'Fascinating', 'count': 32...
    2547    [{'id': 1, 'name': 'Beautiful', 'count': 14}, ...
    2548    [{'id': 11, 'name': 'Longwinded', 'count': 3},...
    2549    [{'id': 21, 'name': 'Unconvincing', 'count': 2...
    Name: ratings_list, Length: 2550, dtype: object
:::
:::

::: {.cell .code execution_count="59"}
``` python
type(ted.ratings_list)
```

::: {.output .execute_result execution_count="59"}
    pandas.core.series.Series
:::
:::

::: {.cell .code execution_count="60"}
``` python
type(ted.ratings_list[0])
```

::: {.output .execute_result execution_count="60"}
    list
:::
:::

::: {.cell .markdown}
## Map vs apply

1.  Map seems to have a subset of apply 2.Use apply anytime it\'s
    necessary
2.  Don\'t use apply when there is a built-in function that can do the
    same: usually built-in pandas functions are more reliable ,
    performant, documented and tested.
3.  Map is a better wrap for performance. However you don\'t always care
    about performance and sometimes they are equivalent (like for a
    small number of values). 5.Use apply last, rather than fast.
4.  Apply is confusing because:\

-   There is a series apply method
-   There is a dataframe apply method
-   There is a series map method
-   There is a dataframe applymap method

Use it with care!
:::

::: {.cell .markdown}
We added a column that is a series of lists, cotaining the ratings for
the talks ( instead of series of stringified lists)
:::

::: {.cell .markdown}
## Count the number of ratings received by each talk and store it in a column called num_ratings
:::

::: {.cell .markdown}
1.  For each talk, calculate the percentage of ratings that were
    negative
2.  For each talk, calculate the average number of ratings it received
    per day since it was published.
:::

::: {.cell .code execution_count="61"}
``` python
ted.ratings_list[1]
```

::: {.output .execute_result execution_count="61"}
    [{'id': 7, 'name': 'Funny', 'count': 544},
     {'id': 3, 'name': 'Courageous', 'count': 139},
     {'id': 2, 'name': 'Confusing', 'count': 62},
     {'id': 1, 'name': 'Beautiful', 'count': 58},
     {'id': 21, 'name': 'Unconvincing', 'count': 258},
     {'id': 11, 'name': 'Longwinded', 'count': 113},
     {'id': 8, 'name': 'Informative', 'count': 443},
     {'id': 10, 'name': 'Inspiring', 'count': 413},
     {'id': 22, 'name': 'Fascinating', 'count': 132},
     {'id': 9, 'name': 'Ingenious', 'count': 56},
     {'id': 24, 'name': 'Persuasive', 'count': 268},
     {'id': 23, 'name': 'Jaw-dropping', 'count': 116},
     {'id': 26, 'name': 'Obnoxious', 'count': 131},
     {'id': 25, 'name': 'OK', 'count': 203}]
:::
:::

::: {.cell .code execution_count="62"}
``` python
def get_num_ratings(list_of_dicts):
    num = 0
    for d in list_of_dicts:
        num = num + d['count']
    return num
```
:::

::: {.cell .code execution_count="63"}
``` python
get_num_ratings(ted.ratings_list[1])
```

::: {.output .execute_result execution_count="63"}
    2936
:::
:::

::: {.cell .code execution_count="64"}
``` python
ted['num_ratings'] = ted.ratings_list.apply(get_num_ratings)
```
:::

::: {.cell .code execution_count="65"}
``` python
ted.num_ratings
```

::: {.output .execute_result execution_count="65"}
    0       93850
    1        2936
    2        2824
    3        3728
    4       25620
            ...  
    2545      192
    2546      151
    2547      136
    2548      583
    2549      142
    Name: num_ratings, Length: 2550, dtype: int64
:::
:::

::: {.cell .code execution_count="66"}
``` python
ted.num_ratings.describe()
```

::: {.output .execute_result execution_count="66"}
    count     2550.000000
    mean      2436.408235
    std       4226.795631
    min         68.000000
    25%        870.750000
    50%       1452.500000
    75%       2506.750000
    max      93850.000000
    Name: num_ratings, dtype: float64
:::
:::

::: {.cell .markdown}
Another way to do this ( Using lambdas in one go!)
:::

::: {.cell .code execution_count="67"}
``` python
pd.DataFrame(ted.ratings_list[0])['count'].sum()
```

::: {.output .execute_result execution_count="67"}
    93850
:::
:::

::: {.cell .code execution_count="68"}
``` python
ted['another_num_ratings'] = ted.ratings_list.apply( lambda x: pd.DataFrame(x)['count'].sum())
```
:::

::: {.cell .code execution_count="69"}
``` python
ted.another_num_ratings
```

::: {.output .execute_result execution_count="69"}
    0       93850
    1        2936
    2        2824
    3        3728
    4       25620
            ...  
    2545      192
    2546      151
    2547      136
    2548      583
    2549      142
    Name: another_num_ratings, Length: 2550, dtype: int64
:::
:::

::: {.cell .code execution_count="70"}
``` python
ted.another_num_ratings.describe()
```

::: {.output .execute_result execution_count="70"}
    count     2550.000000
    mean      2436.408235
    std       4226.795631
    min         68.000000
    25%        870.750000
    50%       1452.500000
    75%       2506.750000
    max      93850.000000
    Name: another_num_ratings, dtype: float64
:::
:::

::: {.cell .markdown}
## Conclusions {#conclusions}

1.  Write one-liners as much as you can and check your work as you go
2.  Lambda is best for simple functions
:::

::: {.cell .markdown}
## Which occupations deliver the funniest TED talks on average?
:::

::: {.cell .markdown}
## Step 1: Count the number of funny ratings
:::

::: {.cell .code execution_count="71"}
``` python
ted.ratings_list.head()
```

::: {.output .execute_result execution_count="71"}
    0    [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
    1    [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
    2    [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
    3    [{'id': 3, 'name': 'Courageous', 'count': 760}...
    4    [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
    Name: ratings_list, dtype: object
:::
:::

::: {.cell .markdown}
1.  Does every rating contain a \"Funny\" score?
:::

::: {.cell .code execution_count="72"}
``` python
ted.ratings.str.contains('Funny').value_counts()
```

::: {.output .execute_result execution_count="72"}
    ratings
    True    2550
    Name: count, dtype: int64
:::
:::

::: {.cell .code execution_count="73"}
``` python
def get_funny_ratings(list_of_dicts):
    for d in list_of_dicts:
        if d['name']=='Funny':
            return d['count']
        
        
```
:::

::: {.cell .code execution_count="74"}
``` python
ted['funny_ratings'] = ted.ratings_list.apply(get_funny_ratings)
```
:::

::: {.cell .code execution_count="75"}
``` python
ted.funny_ratings
```

::: {.output .execute_result execution_count="75"}
    0       19645
    1         544
    2         964
    3          59
    4        1390
            ...  
    2545        1
    2546       20
    2547        1
    2548       63
    2549        0
    Name: funny_ratings, Length: 2550, dtype: int64
:::
:::

::: {.cell .code execution_count="76"}
``` python
ted.funny_ratings.describe()
```

::: {.output .execute_result execution_count="76"}
    count     2550.000000
    mean       154.468627
    std        589.137728
    min          0.000000
    25%          8.000000
    50%         21.000000
    75%         92.000000
    max      19645.000000
    Name: funny_ratings, dtype: float64
:::
:::

::: {.cell .code execution_count="77"}
``` python
ted['funny_rate'] = ted.funny_ratings / ted.num_ratings
```
:::

::: {.cell .code execution_count="78"}
``` python
ted.funny_rate
```

::: {.output .execute_result execution_count="78"}
    0       0.209323
    1       0.185286
    2       0.341360
    3       0.015826
    4       0.054254
              ...   
    2545    0.005208
    2546    0.132450
    2547    0.007353
    2548    0.108062
    2549    0.000000
    Name: funny_rate, Length: 2550, dtype: float64
:::
:::

::: {.cell .code execution_count="79"}
``` python
ted.funny_rate.describe()
```

::: {.output .execute_result execution_count="79"}
    count    2550.000000
    mean        0.050361
    std         0.087779
    min         0.000000
    25%         0.005922
    50%         0.014981
    75%         0.047736
    max         0.702076
    Name: funny_rate, dtype: float64
:::
:::

::: {.cell .markdown}
How to verify that this measure makes sense? Sorting about the \"Funny\"
rating for each talk in the listings would make sense.
:::

::: {.cell .code execution_count="80"}
``` python
ted.sort_values('funny_rate').speaker_occupation.tail(20)
```

::: {.output .execute_result execution_count="80"}
    1849                       Science humorist
    337                                Comedian
    124     Performance poet, multimedia artist
    315                                  Expert
    1168             Social energy entrepreneur
    1468                          Ornithologist
    595                  Comedian, voice artist
    1534                         Cartoon editor
    97                                 Satirist
    2297                          Actor, writer
    568                                Comedian
    675                          Data scientist
    21                     Humorist, web artist
    194                                Jugglers
    2273                    Comedian and writer
    2114                    Comedian and writer
    173                                Investor
    747                                Comedian
    1398                               Comedian
    685             Actor, comedian, playwright
    Name: speaker_occupation, dtype: object
:::
:::

::: {.cell .code execution_count="81"}
``` python
ted.sort_values('funny_rate').speaker_occupation.head(20)
```

::: {.output .execute_result execution_count="81"}
    2549               Game designer
    1612                   Biologist
    612                     Sculptor
    998               Penguin expert
    593                     Engineer
    284               Space activist
    1041         Biomedical engineer
    1618      Spinal cord researcher
    2132    Computational geneticist
    442                     Sculptor
    426              Author, thinker
    458                     Educator
    2437      Environmental engineer
    1491             Photojournalist
    1893     Forensic anthropologist
    783             Marine biologist
    195                    Kenyan MP
    772             HIV/AIDS fighter
    788            Building activist
    936                Neuroengineer
    Name: speaker_occupation, dtype: object
:::
:::

::: {.cell .markdown}
## Step 3: Analyze the funny rate by occupation
:::

::: {.cell .markdown}
Using group by , used by speaker would give us the funny rate by
occupation
:::

::: {.cell .code execution_count="82"}
``` python
ted.groupby('speaker_occupation').funny_rate.mean().sort_values().tail(20)
```

::: {.output .execute_result execution_count="82"}
    speaker_occupation
    Cartoonist                       0.369335
    YouTube trends manager           0.404886
    Entrepreneur, Lego enthusiast    0.409814
    First aid instructor             0.413043
    Expert                           0.415295
    Philosopher-comic                0.415871
    Marketing expert                 0.434353
    Pranksters                       0.437240
    African grey parrot              0.441525
    Comedian + Designer              0.463068
    Science humorist                 0.468405
    Social energy entrepreneur       0.502117
    Comedian, voice artist           0.503542
    Cartoon editor                   0.511628
    Satirist                         0.512383
    Comedian                         0.512457
    Actor, writer                    0.515152
    Actor, comedian, playwright      0.558107
    Jugglers                         0.566828
    Comedian and writer              0.602085
    Name: funny_rate, dtype: float64
:::
:::

::: {.cell .code execution_count="83"}
``` python
ted.speaker_occupation.describe()
```

::: {.output .execute_result execution_count="83"}
    count       2544
    unique      1458
    top       Writer
    freq          45
    Name: speaker_occupation, dtype: object
:::
:::

::: {.cell .markdown}
The problem with this calculation is that these occupations have a small
sample size. 1458 are unique values, so there is a lot of occupations
that are unique
:::

::: {.cell .markdown}
## Focus on occupations that are well-represented in the data
:::

::: {.cell .markdown}
1.  Generate a list of the most represented occupations
:::

::: {.cell .code execution_count="84"}
``` python
occupation_counts = ted.speaker_occupation.value_counts()
```
:::

::: {.cell .code execution_count="85"}
``` python
top_occupations = occupation_counts [occupation_counts>= 5].index
```
:::

::: {.cell .code execution_count="86"}
``` python
top_occupations
```

::: {.output .execute_result execution_count="86"}
    Index(['Writer', 'Artist', 'Designer', 'Journalist', 'Entrepreneur',
           'Architect', 'Inventor', 'Psychologist', 'Photographer', 'Filmmaker',
           'Economist', 'Author', 'Neuroscientist', 'Educator', 'Roboticist',
           'Philosopher', 'Biologist', 'Physicist', 'Musician', 'Marine biologist',
           'Activist', 'Global health expert; data visionary', 'Technologist',
           'Graphic designer', 'Historian', 'Philanthropist', 'Astronomer',
           'Behavioral economist', 'Oceanographer', 'Singer/songwriter', 'Poet',
           'Futurist', 'Engineer', 'Computer scientist', 'Social psychologist',
           'Novelist', 'Mathematician', 'Astrophysicist', 'Social entrepreneur',
           'Photojournalist', 'Writer, activist', 'Evolutionary biologist',
           'Legal activist', 'Climate advocate', 'Techno-illusionist',
           'Singer-songwriter', 'Comedian', 'Performance poet, multimedia artist',
           'Reporter', 'Paleontologist', 'Chemist', 'Cartoonist',
           'Investor and advocate for moral leadership', 'Violinist',
           'Tech visionary', 'Producer', 'Sound consultant', 'Game designer',
           'Physician', 'Surgeon', 'Sculptor', 'Researcher', 'Science writer',
           'Data scientist', 'Musician, activist', 'Social Media Theorist',
           'Environmentalist, futurist', 'Chef'],
          dtype='object', name='speaker_occupation')
:::
:::

::: {.cell .code execution_count="87"}
``` python
type(top_occupations)
```

::: {.output .execute_result execution_count="87"}
    pandas.core.indexes.base.Index
:::
:::

::: {.cell .code execution_count="88"}
``` python
ted_top_occupations = ted[ted['speaker_occupation'].isin(top_occupations)]
```
:::

::: {.cell .code execution_count="89"}
``` python
ted_top_occupations.shape
```

::: {.output .execute_result execution_count="89"}
    (786, 25)
:::
:::

::: {.cell .code execution_count="90"}
``` python
ted_top_occupations.describe()
```

::: {.output .execute_result execution_count="90"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>comments</th>
      <th>duration</th>
      <th>film_date</th>
      <th>languages</th>
      <th>num_speaker</th>
      <th>published_date</th>
      <th>views</th>
      <th>comments_per_view</th>
      <th>views_per_comment</th>
      <th>film_datetime</th>
      <th>num_ratings</th>
      <th>another_num_ratings</th>
      <th>funny_ratings</th>
      <th>funny_rate</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>786.000000</td>
      <td>786.000000</td>
      <td>7.860000e+02</td>
      <td>786.000000</td>
      <td>786.000000</td>
      <td>7.860000e+02</td>
      <td>7.860000e+02</td>
      <td>786.000000</td>
      <td>786.000000</td>
      <td>786</td>
      <td>786.000000</td>
      <td>786.000000</td>
      <td>786.000000</td>
      <td>786.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>205.409669</td>
      <td>826.286260</td>
      <td>1.301029e+09</td>
      <td>27.815522</td>
      <td>1.034351</td>
      <td>1.326715e+09</td>
      <td>1.712339e+06</td>
      <td>0.000154</td>
      <td>14206.494098</td>
      <td>2012-01-16 11:49:37.044529152</td>
      <td>2525.507634</td>
      <td>2525.507634</td>
      <td>165.482188</td>
      <td>0.053808</td>
    </tr>
    <tr>
      <th>min</th>
      <td>2.000000</td>
      <td>135.000000</td>
      <td>4.265316e+08</td>
      <td>0.000000</td>
      <td>1.000000</td>
      <td>1.151367e+09</td>
      <td>5.044300e+04</td>
      <td>0.000003</td>
      <td>683.134291</td>
      <td>2006-06-27 00:11:00</td>
      <td>142.000000</td>
      <td>142.000000</td>
      <td>0.000000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>63.000000</td>
      <td>541.500000</td>
      <td>1.233965e+09</td>
      <td>23.000000</td>
      <td>1.000000</td>
      <td>1.251356e+09</td>
      <td>7.192218e+05</td>
      <td>0.000059</td>
      <td>5540.287089</td>
      <td>2009-08-27 07:00:00</td>
      <td>918.000000</td>
      <td>918.000000</td>
      <td>8.000000</td>
      <td>0.006463</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>124.000000</td>
      <td>848.000000</td>
      <td>1.310558e+09</td>
      <td>28.000000</td>
      <td>1.000000</td>
      <td>1.323102e+09</td>
      <td>1.123634e+06</td>
      <td>0.000106</td>
      <td>9473.250007</td>
      <td>2011-12-05 16:19:41</td>
      <td>1490.000000</td>
      <td>1490.000000</td>
      <td>26.000000</td>
      <td>0.017125</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>224.750000</td>
      <td>1063.000000</td>
      <td>1.394950e+09</td>
      <td>34.000000</td>
      <td>1.000000</td>
      <td>1.401073e+09</td>
      <td>1.759730e+06</td>
      <td>0.000180</td>
      <td>16808.135662</td>
      <td>2014-05-26 02:54:11.500000</td>
      <td>2640.000000</td>
      <td>2640.000000</td>
      <td>110.000000</td>
      <td>0.055667</td>
    </tr>
    <tr>
      <th>max</th>
      <td>6404.000000</td>
      <td>3955.000000</td>
      <td>1.503792e+09</td>
      <td>72.000000</td>
      <td>4.000000</td>
      <td>1.506092e+09</td>
      <td>4.315540e+07</td>
      <td>0.001464</td>
      <td>323087.000000</td>
      <td>2017-09-22 15:00:22</td>
      <td>65968.000000</td>
      <td>65968.000000</td>
      <td>7315.000000</td>
      <td>0.669927</td>
    </tr>
    <tr>
      <th>std</th>
      <td>339.003617</td>
      <td>404.903481</td>
      <td>1.274605e+08</td>
      <td>10.260198</td>
      <td>0.202130</td>
      <td>9.433474e+07</td>
      <td>2.509243e+06</td>
      <td>0.000170</td>
      <td>18131.368966</td>
      <td>NaN</td>
      <td>3904.029024</td>
      <td>3904.029024</td>
      <td>482.137463</td>
      <td>0.089033</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .code execution_count="91"}
``` python
ted_top_occupations.groupby('speaker_occupation').funny_rate.mean().sort_values().tail(20)
```

::: {.output .execute_result execution_count="91"}
    speaker_occupation
    Science writer                          0.055993
    Designer                                0.059287
    Writer                                  0.060745
    Game designer                           0.062317
    Reporter                                0.066250
    Evolutionary biologist                  0.069157
    Novelist                                0.070876
    Entrepreneur                            0.073295
    Author                                  0.075508
    Artist                                  0.078939
    Global health expert; data visionary    0.090306
    Poet                                    0.107398
    Graphic designer                        0.135718
    Techno-illusionist                      0.152171
    Cartoonist                              0.162120
    Data scientist                          0.184076
    Producer                                0.202531
    Singer/songwriter                       0.252205
    Performance poet, multimedia artist     0.306468
    Comedian                                0.512457
    Name: funny_rate, dtype: float64
:::
:::

::: {.cell .markdown}
:::

::: {.cell .markdown}
## Conclusions {#conclusions}

1.  Check your assumptions about your data
2.  Check whether your results make sense.
3.  Check the type of pandas operations: they are usually DataFrame or
    Series.
4.  Watch out for small sample sizes.
5.  Consider the impact of missing data: this is NOT showing any errors
    :)
:::

::: {.cell .markdown}
# Pandas Tips and Tricks
:::

::: {.cell .markdown}
**Credits**: From the video of same author
<https://youtu.be/RlIiVeig3hc>
:::

::: {.cell .markdown}
1.  Show Pandas Versions (and from its dependencies)
:::

::: {.cell .code execution_count="92"}
``` python
pd.show_versions()
```

::: {.output .stream .stdout}

    INSTALLED VERSIONS
    ------------------
    commit           : 37ea63d540fd27274cad6585082c91b1283f963d
    python           : 3.9.6.final.0
    python-bits      : 64
    OS               : Darwin
    OS-release       : 22.4.0
    Version          : Darwin Kernel Version 22.4.0: Mon Mar  6 20:59:28 PST 2023; root:xnu-8796.101.5~3/RELEASE_ARM64_T6000
    machine          : arm64
    processor        : arm
    byteorder        : little
    LC_ALL           : None
    LANG             : None
    LOCALE           : None.UTF-8

    pandas           : 2.0.1
    numpy            : 1.23.3
    pytz             : 2022.2.1
    dateutil         : 2.8.2
    setuptools       : 58.0.4
    pip              : 21.2.4
    Cython           : None
    pytest           : None
    hypothesis       : None
    sphinx           : None
    blosc            : None
    feather          : None
    xlsxwriter       : None
    lxml.etree       : 4.9.1
    html5lib         : None
    pymysql          : None
    psycopg2         : None
    jinja2           : 3.1.2
    IPython          : 8.13.2
    pandas_datareader: None
    bs4              : 4.11.1
    bottleneck       : None
    brotli           : None
    fastparquet      : None
    fsspec           : None
    gcsfs            : None
    matplotlib       : 3.7.1
    numba            : None
    numexpr          : None
    odfpy            : None
    openpyxl         : None
    pandas_gbq       : None
    pyarrow          : None
    pyreadstat       : None
    pyxlsb           : None
    s3fs             : None
    scipy            : None
    snappy           : None
    sqlalchemy       : None
    tables           : None
    tabulate         : None
    xarray           : None
    xlrd             : None
    zstandard        : None
    tzdata           : 2023.3
    qtpy             : 2.2.0
    pyqt5            : None
:::
:::

::: {.cell .markdown}
1.  Generate a sample Data Frame
:::

::: {.cell .markdown}
What we do manually:
:::

::: {.cell .code execution_count="93"}
``` python
df = pd.DataFrame({'col one':[100,200],'col two':[300,400]})
```
:::

::: {.cell .code execution_count="94"}
``` python
df
```

::: {.output .execute_result execution_count="94"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>col one</th>
      <th>col two</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100</td>
      <td>300</td>
    </tr>
    <tr>
      <th>1</th>
      <td>200</td>
      <td>400</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
Easier, using numpy:
:::

::: {.cell .code execution_count="95"}
``` python
import numpy as np
```
:::

::: {.cell .markdown}
Parameters are: rows,columns
:::

::: {.cell .code execution_count="96"}
``` python
pd.DataFrame(np.random.rand(4,8))
```

::: {.output .execute_result execution_count="96"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
      <th>5</th>
      <th>6</th>
      <th>7</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0.570378</td>
      <td>0.367411</td>
      <td>0.865880</td>
      <td>0.437038</td>
      <td>0.354206</td>
      <td>0.412463</td>
      <td>0.330390</td>
      <td>0.722543</td>
    </tr>
    <tr>
      <th>1</th>
      <td>0.167644</td>
      <td>0.677556</td>
      <td>0.615086</td>
      <td>0.454293</td>
      <td>0.614237</td>
      <td>0.409272</td>
      <td>0.704607</td>
      <td>0.045908</td>
    </tr>
    <tr>
      <th>2</th>
      <td>0.285340</td>
      <td>0.438551</td>
      <td>0.402809</td>
      <td>0.296770</td>
      <td>0.996599</td>
      <td>0.989184</td>
      <td>0.386614</td>
      <td>0.050287</td>
    </tr>
    <tr>
      <th>3</th>
      <td>0.283214</td>
      <td>0.040261</td>
      <td>0.310578</td>
      <td>0.272318</td>
      <td>0.544209</td>
      <td>0.575619</td>
      <td>0.861728</td>
      <td>0.279068</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
Giving it the header for each column (as a list)
:::

::: {.cell .code execution_count="97"}
``` python
pd.DataFrame(np.random.rand(4,8), columns=list('abcdefgh'))
```

::: {.output .execute_result execution_count="97"}
```{=html}
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>a</th>
      <th>b</th>
      <th>c</th>
      <th>d</th>
      <th>e</th>
      <th>f</th>
      <th>g</th>
      <th>h</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0.034104</td>
      <td>0.075956</td>
      <td>0.334785</td>
      <td>0.442860</td>
      <td>0.179954</td>
      <td>0.607041</td>
      <td>0.558778</td>
      <td>0.288265</td>
    </tr>
    <tr>
      <th>1</th>
      <td>0.650791</td>
      <td>0.718474</td>
      <td>0.694375</td>
      <td>0.901698</td>
      <td>0.437911</td>
      <td>0.848726</td>
      <td>0.272597</td>
      <td>0.982334</td>
    </tr>
    <tr>
      <th>2</th>
      <td>0.344147</td>
      <td>0.791109</td>
      <td>0.560324</td>
      <td>0.882701</td>
      <td>0.282536</td>
      <td>0.992830</td>
      <td>0.900864</td>
      <td>0.334858</td>
    </tr>
    <tr>
      <th>3</th>
      <td>0.645883</td>
      <td>0.584075</td>
      <td>0.442720</td>
      <td>0.289285</td>
      <td>0.273389</td>
      <td>0.024719</td>
      <td>0.316358</td>
      <td>0.203573</td>
    </tr>
  </tbody>
</table>
</div>
```
:::
:::

::: {.cell .markdown}
1.  Renaming columns
:::

::: {.cell .markdown}
# Pandas AI
:::

::: {.cell .code execution_count="98" vscode="{\"languageId\":\"powershell\"}"}
``` python
pip install pandasai
```

::: {.output .stream .stdout}
    Defaulting to user installation because normal site-packages is not writeable
    Requirement already satisfied: pandasai in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (0.2.11)
    Requirement already satisfied: openai<0.28.0,>=0.27.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (0.27.6)
    Requirement already satisfied: ipython<9.0.0,>=8.13.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (8.13.2)
    Requirement already satisfied: astor<0.9.0,>=0.8.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (0.8.1)
    Requirement already satisfied: python-dotenv<2.0.0,>=1.0.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (1.0.0)
    Requirement already satisfied: pandas<3.0.0,>=2.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (2.0.1)
    Requirement already satisfied: matplotlib<4.0.0,>=3.7.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (3.7.1)
    Requirement already satisfied: prompt-toolkit!=3.0.37,<3.1.0,>=3.0.30 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (3.0.31)
    Requirement already satisfied: pexpect>4.3 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (4.8.0)
    Requirement already satisfied: matplotlib-inline in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.1.6)
    Requirement already satisfied: appnope in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.1.3)
    Requirement already satisfied: stack-data in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.5.1)
    Requirement already satisfied: backcall in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.2.0)
    Requirement already satisfied: decorator in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (5.1.1)
    Requirement already satisfied: traitlets>=5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (5.4.0)
    Requirement already satisfied: pickleshare in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.7.5)
    Requirement already satisfied: typing-extensions in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (4.5.0)
    Requirement already satisfied: pygments>=2.4.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (2.13.0)
    Requirement already satisfied: jedi>=0.16 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.18.1)
    Requirement already satisfied: parso<0.9.0,>=0.8.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from jedi>=0.16->ipython<9.0.0,>=8.13.1->pandasai) (0.8.3)
    Requirement already satisfied: pyparsing>=2.3.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (3.0.9)
    Requirement already satisfied: packaging>=20.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (21.3)
    Requirement already satisfied: kiwisolver>=1.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.4.4)
    Requirement already satisfied: python-dateutil>=2.7 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (2.8.2)
    Requirement already satisfied: pillow>=6.2.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (9.2.0)
    Requirement already satisfied: contourpy>=1.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.0.5)
    Requirement already satisfied: numpy>=1.20 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.23.3)
    Requirement already satisfied: cycler>=0.10 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (0.11.0)
    Requirement already satisfied: fonttools>=4.22.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (4.37.3)
    Requirement already satisfied: importlib-resources>=3.2.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (5.12.0)
    Requirement already satisfied: zipp>=3.1.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from importlib-resources>=3.2.0->matplotlib<4.0.0,>=3.7.1->pandasai) (3.8.1)
    Requirement already satisfied: aiohttp in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (3.8.4)
    Requirement already satisfied: tqdm in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (4.64.1)
    Requirement already satisfied: requests>=2.20 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (2.28.1)
    Requirement already satisfied: tzdata>=2022.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandas<3.0.0,>=2.0.1->pandasai) (2023.3)
    Requirement already satisfied: pytz>=2020.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandas<3.0.0,>=2.0.1->pandasai) (2022.2.1)
    Requirement already satisfied: ptyprocess>=0.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pexpect>4.3->ipython<9.0.0,>=8.13.1->pandasai) (0.7.0)
    Requirement already satisfied: wcwidth in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from prompt-toolkit!=3.0.37,<3.1.0,>=3.0.30->ipython<9.0.0,>=8.13.1->pandasai) (0.2.5)
    Requirement already satisfied: six>=1.5 in /Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.9/lib/python3.9/site-packages (from python-dateutil>=2.7->matplotlib<4.0.0,>=3.7.1->pandasai) (1.15.0)
    Requirement already satisfied: idna<4,>=2.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (3.4)
    Requirement already satisfied: certifi>=2017.4.17 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (2022.9.24)
    Requirement already satisfied: charset-normalizer<3,>=2 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (2.1.1)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (1.26.12)
    Requirement already satisfied: multidict<7.0,>=4.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (6.0.4)
    Requirement already satisfied: aiosignal>=1.1.2 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.3.1)
    Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (4.0.2)
    Requirement already satisfied: yarl<2.0,>=1.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.9.2)
    Requirement already satisfied: attrs>=17.3.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (22.1.0)
    Requirement already satisfied: frozenlist>=1.1.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.3.3)
    Requirement already satisfied: executing in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (1.1.0)
    Requirement already satisfied: pure-eval in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (0.2.2)
    Requirement already satisfied: asttokens in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (2.0.8)
    WARNING: You are using pip version 21.2.4; however, version 23.1.2 is available.
    You should consider upgrading via the '/Library/Developer/CommandLineTools/usr/bin/python3 -m pip install --upgrade pip' command.
    Note: you may need to restart the kernel to use updated packages.
:::
:::

::: {.cell .code execution_count="99" vscode="{\"languageId\":\"powershell\"}"}
``` python
from pandasai import PandasAI
```
:::

::: {.cell .code vscode="{\"languageId\":\"powershell\"}"}
``` python
```
:::

::: {.cell .code execution_count="120" vscode="{\"languageId\":\"powershell\"}"}
``` python
{
    "tags": [
        "hide-cell"
    ]
}
```

::: {.output .execute_result execution_count="120"}
    {'tags': ['hide-cell']}
:::
:::

::: {.cell .code execution_count="122" tags="[\"remove-input\"]"}
``` python
# Instantiate a LLM
from pandasai.llm.openai import OpenAI
llm = OpenAI(api_token="API_KEY")
```
:::

::: {.cell .code execution_count="123"}
``` python
df = pd.DataFrame({
    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
})
```
:::

::: {.cell .code execution_count="128"}
``` python
pandas_ai = PandasAI(llm, conversational=False)
pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
```

::: {.output .execute_result execution_count="128"}
    '6            Canada\n7         Australia\n1    United Kingdom\n3           Germany\n0     United States\nName: country, dtype: object\n'
:::
:::

::: {.cell .code execution_count="129"}
``` python
pandas_ai.run(
    df,
    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
)
```

::: {.output .display_data}
![](vertopal_b065e047d75a40e4a5a83d795a81d805/b770eee5b8044fbad42fa843ac6e5ddd785f8f42.png)
:::

::: {.output .execute_result execution_count="129"}
    ''
:::
:::
