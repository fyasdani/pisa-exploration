# PISA 2012 Data Exploration
#### by fyasdani

## [Dataset](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip&sa=D&ust=1581581520574000)\*

PISA stands for the Programme for International Student Assessment. Every few
years, since 1997, PISA has compared 15-year-old students from different
countries based on their reading, math and science acumen. PISA is funded by
the Organization for Economic Co-operation and Development. Their goal is to
improve education policy internationally—for OECD and non-OECD countries alike.
All are welcome to participate. This report explores the data from 2012—
when 485,490 students from 65 countries participated. There are 635 features,
of which 120 pertain to math.

\*325 MB (2.6 GB uncompressed)

## Summary of [Findings](https://raw.githack.com/fyasdani/pisa-exploration/main/exploration.html)

This exploration's purpose is twofold: 1) to discover why the US underperforms
at math, while its neighbor Canada excels—when the two countries are otherwise
quite similar; and 2) to discover what the US can do to excel as well.

-   American STEM students prioritize math over science at a rate greater than
    that of their Canadian counterparts (+9%).
-   10% of math-oriented, US high-school students have no intention of going to
    college for math, or of pursuing a career in it, whereas Canada's numbers
    hold steady.
    -   Nationwide, that amounts to *millions* of students forsaking math.
-   The average Canadian student is more math-focused than the average American
    one.
    -   Yet a greater percentage of American students focus *fully* on math.
-   In both countries, most students come from home-life cultures that are
    largely ambivalent towards math, and it falls on the teachers to encourage
    them towards the topic.
-   Fully-focused US students have high self-efficacy and self-concept.
-   Compared to Canadian students, fewer American students have strongly
    negative feelings about math (10% vs 13%).
-   Students strongly encouraged to do math tend to do so.
-   Some students have the confidence but lack the desire.
-   Subjective norms, self-concept, and self-efficacy are all positively
    correlated with math intention, as well as with each other.
-   Math intention and self-concept are moderately correlated (0.39), as are
    self-concept and self-efficacy (0.53).
-   The theory of reasoned action (TRA) elegantly explains why some American
    students intend to do math, and others do not.

## Key Insights for [Presentation](https://raw.githack.com/fyasdani/pisa-exploration/main/explanation.slides.html#/)

-   10% of math-oriented, US high-school students have no intention of going to
    college for math, or of pursuing a career in it, whereas Canada's numbers
    hold steady.
    -   Nationwide, that amounts to *millions* of students forsaking math.
-   The average Canadian student is more math-focused than the average American
    one.
    -   Yet a greater percentage of American students focus *fully* on math.
-   The theory of reasoned action (TRA) elegantly explains why some American
    students intend to do math, and others do not.

### Changes in Design

1)  The redundant y-axes were removed from the subplotted figures using the following bit of code:

```python
ax2.set_yticks([])
ax2.set_ylabel('')
```

2)  Additionally, an annotation and a title were added to the histograms plot like so:

```python
fig.suptitle('Distribution of Students by Intentions towards Math')
fig.text(0, 0, 'Note: Math Intention is an score reflecting students\'' 
               ' orientation towards or away from doing math.')
```

3)  A similar note was added to the multivariate scatterplot, this time using `plt`.
