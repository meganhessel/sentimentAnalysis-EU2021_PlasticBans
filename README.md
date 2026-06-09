---
editor_options: 
  markdown: 
    wrap: 72
---

# EU Single-Use Plastic Bans

## Text Analysis

Use sentiment analysts to monitor and gauge the public's response to the
actions of the EU Single Use plastic (SUP) direction after July of 2021.
This project applies sentiment analysis to news media coverage in order
to monitor and gauge public response to the EU Single-Use Plastics (SUP)
Directive (2019/904) following its enforcement date of July 3, 2021. The
directive banned single-use plastic plates, cutlery, straws, balloon
sticks, cotton buds, and expanded polystyrene food containers across EU
member states.

The analysis tracks how media sentiment toward the directive shifted
over time using Bing, AFINN, sentimentr, and VADAR.

## Research Question:

How has media sentiment toward the EU Single-Use Plastics Directive
changed following its implementation in July 2021?

## Data Sources

Data source are not located within this repository.

**Nexis Uni** (Primary):

News articles were retrieved from Nexis Uni using the following search
terms:

-   single-use plastic

-   SUP directive

-   EU plastic ban

-   single use plastics directive

Articles were downloaded as .docx files and parsed using the
LexisNexisTools R package.

**Reddit (Supplementary)**

Historical Reddit comments were sourced from the Pushshift dataset via
Academic Torrents, covering the following subreddits:

-   r/environment

-   r/ZeroWaste

-   r/european

Files were filtered using grep before loading into R to reduce memory
overhead.

## File Structure

```         
├── README.md
├── load_data.qmd
├── Nexis-analysis
│   ├── sentiment-analysis-Nexis.qmd
│   └── topic-analysis-Nexis.qmd
└── reddit-analysis
    ├── sentiment-analysis-reddit.qmd
    └── topic-analysis-reddit.qmd
```

## References

European Commission. (n.d.). Single-use plastics.
<https://environment.ec.europa.eu/topics/plastics/single-use-plastics_en>

Jonny Auping. (2024). European Union Adopts Rules Banning Single-Use
Plastics By 2030. Promotional Products Association International.
<https://www.ppai.org/media-hub/european-union-adopts-rules-banning-single-use-plastics-by-2030/>

Paloniitty, T., & Ala-Lahti, T. (2024). The European Union and plastics.
In *Research Handbook on Plastics Regulation* (pp. 187-207). Edward
Elgar Publishing.
