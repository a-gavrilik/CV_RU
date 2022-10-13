# **A/B testing**

### Stack:
- Python
  - Pandas
  - Numpy
  - scipy.stats
    - ttest_ind
    - chi2_contingency

### Task Description:

One of the main tasks of analytics in our team is correct conduct of experiments. For this we use the A/B-testing method. In the course of testing one hypothesis, the task force was proposed a new mechanism of payment for services on the site, the control group remained basic mechanics. As a task you need to analyze the results of the experiment and make a conclusion whether to run the new payment mechanism on all users.

As input you have 4 csv files:
- [groups.csv](https://disk.yandex.ru/d/58Us0DWOzuWAjg) - file with information about the user belonging to a control or experimental group (**A** - control, **B** - experimental group)
- [groups_add.csv](https://disk.yandex.ru/d/3aARY-P9pfaksg) - an additional file with users which was sent to you 2 days after the data transfer
- [active_studs.csv](https://disk.yandex.ru/d/prbgU-rZpiXVYg) - file with information about users who logged on to the platform on the days of the experiment
- [checks.csv](https://disk.yandex.ru/d/84hTmELphW2sqQ) - file with user payments on the days of the experiment

The following questions must be answered:
- What metrics do you look at during the analysis and why?
- Are there differences in indicators and what might they be related to?
- Are these differences statistically significant?
- Is it worth running the new mechanic on all users?