# Marketing-Insight-FMCG

[Question](https://codebasics.io/challenge/codebasics-resume-project-challenge/9)
![Capture](https://github.com/dzvlhakimi/Marketing-Insight-FMCG/assets/156594044/b1a1e8f0-f726-40ad-bb18-fc1c817d6522)


```SQL
select fr.Ingredients_expected, count(*) as IngredientCount
from survey.fact_survey_responses fr
join respondents.dim_respondents on dim_respondents.Respondent_ID = fr.Respondent_ID
-- where dim_respondents.gender in ('Female')
-- where dim_respondents.gender in ('Male')
-- where dim_respondents.gender in ('Non-binary')
group by fr.Ingredients_expected;
```
