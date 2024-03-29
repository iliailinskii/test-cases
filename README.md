# Data analyst tech tasks

I have faced many tech tasks for data analysis during my career. You can find my solutions and some recommendations for analysts in this repository. 
## Repository structure
* Real tech tasks solutions
* Best practice
* How to introduce yourself 

## To be done in the future
* Create a universal testing case for marketing/growth analyst
* Create documentation for a team lead
* Make better versions of my case solutions

## Real tech tasks solutions
All cases in this repository are actual interview tech tasks for a senior data analyst position, primarily in marketing or growth teams.
I rename companies to protect their anonymity. 
I chose only successful tech tasks. Thus, you can see an acceptable work level for successful data analyst tech interview completion. 
There are 3 types of tech interviews for data analysts:
* Online test. Usually, test SQL skills. 
* Home task. The company provides a dataset and tech task description and gives 1 week for its solution.
* Tech interview. Candidates are asked to write some scripts in SQL / Python during the interview. 

However, some companies use various combinations of these types. 
### Company A
This company is specialized in call-center automatization with their AI bots. Their tech task tests analyst ability to find insights in data, prepare visualization and provide recommendations to the business.

Case content:
* [Task description](https://github.com/iliailinskii/test-cases/blob/main/company%20a/Company%20A%20tech%20task.pdf)
* [Presentation to managers](https://github.com/iliailinskii/test-cases/blob/main/company%20a/Company%20A%20result%20slides.pdf)
* [Solution scripts](https://github.com/iliailinskii/test-cases/blob/main/company%20a/Company_A%20scripts.ipynb)

### Company B
This is a fintech company. The task challenges the analyst's ability to analyze cohorts and work as a growth hacker.

Case content:
* [Task description](https://github.com/iliailinskii/test-cases/blob/main/company%20b/Company%20b%20tech%20task.pdf)
* [Solution scripts](https://github.com/iliailinskii/test-cases/blob/main/company%20b/Company_B_scripts.ipynb)

### Company C
This is a dating app company. The task challenges analysts' ability to work with unstructured data and find anomalies.

Case content:
* [Task description](https://github.com/iliailinskii/test-cases/blob/main/company%20c/Company%20C%20tech%20task.pdf)
* [Presentation to managers](https://github.com/iliailinskii/test-cases/blob/main/company%20c/Company%20C%20result%20slides.pdf)
* [Solution scripts](https://github.com/iliailinskii/test-cases/blob/main/company%20c/Company_C_scripts.ipynb)

### Company D
This is a fintech company that distributes digital subscription products. The task is focused on marketing analysis and testing the ability of channel evaluation.

Case content:
* [Task description](https://github.com/iliailinskii/test-cases/blob/main/company%20d/Company%20%20D%20tech%20task.pdf)
* [Solution scripts](https://github.com/iliailinskii/test-cases/blob/main/company%20d/Company%20D%20scripts.ipynb)

## Best practice
Here I collected the main points of how to complete analyst tech tasks and some small tips for it.

### Choose instrument 
Nowadays, there are lots of instruments that allow you to demonstrate your analyst skills. 
I suppose [Jupyter Notebooks](https://jupyter.org/install) to be one of the most widespread ones. There are some pros to using it:
- Use python for working with data
- Ability to organize research structure
- Convenient markdowns system, so you can follow your scripts with comments and conclusions
- Standard format 

So you can write scripts and presentations for research all in one. 
By the way, I conduct all my studies in [Colab](https://colab.research.google.com/notebooks/basic_features_overview.ipynb). I chose it because I had only the old-fashioned laptop with 2 cores processor and sometimes worked on public library computers. Thus, Colab let me not be limited by laptop resources and be flexible in working on the project from different devices. Among other pros, Colab is much easier to set up. You just need to open the link. Also, it is easy to share by link. 
> Small tip. You can use the Colab Pro version with GPU and additional RAM for 10 euros per month. And still, all these things are highly affordable because you can have lots of calculation resources even on super cheap devices (in extremal cases, even on tablets or smartphones)

### Instrument to demonstrate SQL skills
Initially, I highly recommend trying this [site](https://sqliteonline.com/). Here you can import CSV files and work with them on SQL lite. Also, you can deploy MariaDB, Postgres, or MS SQL locally and use this site as an interface. 

However, sqliteinline has limits for table size, and you can not make a dashboard in it to share your results by link. That's why I suggest using [pandasql](https://pypi.org/project/pandasql/) in combination with Jupyter Notebook. In such an approach, you can demonstrate all your skills in one document.
> Small tip. If you use pandasql, you must format your values to the 8-bit datatype. It is SQL lite limit. 

### How to organize the process
Tech task usually is quite stressful processes. That is why a plan allows you to focus and worry less. 
Surprisingly, most of the tasks are structured the same. You have a dataset, its description (hopefully), and a task list. 
>  It is critical to understand what the company wants to test to make a good solution. 
From my managerial expirience, most companies follow the aim to test candidates for the next skills.
- Work process organization
- Ability to work with the new dataset
- Understand metric trees in the company field (funnels, unit economy, statistics, etc.)
- Python / SQL level
- Data Visualisation 
- Make conclusions and insights based on data

Based on this information, we can tune our approach to task solutions.
I suggest following the following checklist for every solution.

1. Read the task  and the dataset description mindfully
2. If there is no dataset description, have a look at it (how to do it in the next parts)
3. Create a research plan.
>  I know that research is a creative process, and most analysts create a plan during working with data. However, in a test task, you do not have enough time to spend in such a way.
4. Describe your plan in Notebook
5. Read the data
6. Clear data
7. Create an analytical platform for yourself. It includes all your scripts to complete the task.
8. Reassume scripts and reorganize them to save only the working hypothesis to make it more straightforward for the examinator
9. Tune visualizations
10. Write down conclusions and markdown comments on scripts
11. Make a presentation to the manager
12. Create a solution pack, describe it and send it to the company

Doing our best at each of these points will increase our chances of passing the test.
You can see that most of them are very universal for any task. Thus, my advice will work for most analyst tech tasks.

### Tips to improve the solution
**No dataset description**

Okay, sometimes either company wants to test your ability to work with undocumented data, or they are just lazy to make descriptions. In that case, you need to define data nature by yourself. How to do it. 
Usually follow the next plan:
- Have a look at the data. Select head 5-10 rows and visually see their values. 
> Using the pandas library in python, you can use the function df.head(number_rows) 
- Try to connect column name, value, and business meaning. 
- Classify the values and select a data type. Is it categorical, rank, number, DateTime, bool, or something else?
- Based on the data type, I tried to learn what this data looks like. How many categories? What are the minimum and maximum dates? How number value is distributed. Do data include NaN, and how are they logged?
> First, change a data format to the correct one for DateTime. Use DateTime library and pandas function pandas.datetime for other types. You can use .astype. Then to see general information simplest way is to use the pandas function .describe(). It returns max, min, average, unique, count, and other essential metrics. For number value distribution you can build a box splot in any convenient library (in the next part, I will share my favorite one).

This analysis usually is enough to go to the planning stage.

**How to create a plan**

Honestly, there is no precisely one way to do it. It highly depends on the tech task.
However, to save time, you can use a common research pattern.
Which patterns do I often use?
Based on tech task:
- From up to down approach. Select the primary metric, decompose this metric into sub-metrics and build all possible distributions of these metrics based on available slices. 
> For example, you need to define marketing channel efficiency, and the high metric is ROI. You can decompose it to LTV and CAC, LTV decomposes to ARPU and LT, ARPU decays to APPP and APPU. Then you can see time dynamics, structure by market channels and their companies, structure by segment, country, device, etc.
Based on the data description:
- If I have time series in the data frame, I research dynamics with one or several spans, daily, weekly, or monthly.
- If I have categorical values, I use them for slices.
- If I have numerical values, I research their distribution. 
- If I have event timestamps, I build funnels.
- If I have the first action date I built cohorts.

I form a plan as a result of a combination of business and technical parts. In my practice, these patterns cover almost all cases.

**Read data**

Nothing special. I used pandas.read_csv / pandas.read_excel. In the case of CSV, sometimes you need to update the separation parameter to ";" using sep = ";" condition. 
Also, if you work in Colab you can read files from your google disk.
```
from google.colab import drive
drive.mount('/content/gdrive', force_remount=True) # set default location as main disc direction
```
**Clear data**

Anomalies in data may spoil all your further analysis. That is why always complete this step, even in test tasks.
The basic steps for these processes are the next:

Cope with missings.

- First, define them. It might be empty/space/NaN/na/nan/NA or called something else. To detect missing values, use isnull() and isna(). However, to double-check it I recommend calculating the count by unique values.
-  Secondly, decide what to do drop it (.dropna()) / to set default value (.fillna())/ reconstruct it.
> Usually, you can drop data if it's an extremely rare event. You should fill in the default value if it is a good part of the data. And in rare cases, there is a way to reconstruct data from other fields. For instance, you do not have a device brand, but you have device OS, so you can reconstruct apple devices by ios value. 
-  Finally, conduct the proper action.

Check anomalies. 

The most common one:
- Negative values for real numbers value
- Wrong DateTime ( dates in the future or far in the past)
- Wrong time sequence. For example, first, purchase earlier than the first visit.
- Sometimes, there is a need to exclude extremal values like first or 99 percentile

Check doubles

In the case of a unique id that should be unique in this table, it makes sense to check it.
In categorical values, you may have the same category meaning with different labels (with various literature, upper or lower, with close words, etc).
To find out it, you can count values by unique ones in the column. 

**Create an analytical platform**

That is an exciting part. I really believe that the best way to research data is to make a convenient interactive dashboard for yourself. 
A good analyst is getting used to exploring data by writing scripts and visually seeing that data tables might be essential.
But, the ability to operate with data using UI makes the exploration process much faster, and it may be critical in the creative process. 
When you can navigate over the data by clicking, it allows you to follow your mind immediately without thinking about how to construct the query. 

As an example, you want to research the conversion rate to purchase to see study user base quality. You have two ways to build funnels one by one or create master data and build an interactive dashboard, where you can select segment, cohort, country, span, device, etc. When you can choose slices, grouping, and define periods, it allows you to test many hypotheses and generate new ones just on the go.

I hope I prove a need for such a platform. Then how can it be created?
In a company, you usually have a BI system. In a test task you have two ways:
1. Use the BI system on your own:) But it may be time overkill to set up it locally for each task
2. Use Notebook interactive abilities.

I personally vote for the second one. In my case, I use [plotly](https://plotly.com/python/).
Why I have chosen it?
1. Simplicity, less code, more functions. You need to write a couple of code lines and as a result, get an animated, interactive graph.
2. Beauty. It looks clear, modern, and pretty, so you will have nice graphs even if you are not a professional visualizer. In addition, you may use these graphs not just for your platform but also for your case solution visualizations. 
3. Big graph assortment from bars to maps. 

In cases when you need to build a lot of graphs, I highly recommend writing the graph generator method and automating this process to make your script even more concise.

**Reassume scripts**

I do recommend not sending your "analytical platform" as a solution to the hiring managers. It might work clearly for you as soon as you have constructed it, but it can be too complicated for a manager. You should understand that an examinator manager usually only has a little free time. The best practice is to provide a shorter decision and either hide your "analytical platform" or add it at the end of the solution. 

In the shorter version, place all your analysis in the logic sequence and leave only the parts which lead to the result skipping analysis without outcomes. 

**Tune visualisations**

As I said before, I highly recommend [plotly](https://plotly.com/python/). However, you are free to choose any instrument. 

The thing you should keep in mind is that every graph must have:
* Head title
* Legend
* Axis names
* Description of how to read it

Also, data have to be:
* Visually separated
* Not overloaded with the content
* Not be misinterpreted 

Use the correct graphs:
* Barchart or piecharts for structure 
* Line charts for time series 
* Box plot, scatter plot, bars for distributions
* Maps for geo-data
* Tables for the multimetric comparisons

etc

**Make presentation**
You are not expected to be a designer. Still, presentation quality is a massive plus for you, especially for presentations to non-analyst managers.
Your presentation should be simple and clear.

1. Add a research plan to the first slide.
2. Follow each task with visualization and conclusion (better on one slide but not overload slide)

A good idea is to use company corporate colors from their website.
The presentation should be business style but not boring.

I suggest using [canva](https://www.canva.com/) as a presentation constructor. It has nice fonts, presets, and an easy UI. 
1. [Presentation example 1](https://github.com/iliailinskii/test-cases/blob/main/company%20a/Company%20A%20result%20slides.pdf)
2. [Presentation example 2](https://github.com/iliailinskii/test-cases/blob/main/company%20c/Company%20C%20result%20slides.pdf)

**Create a solution pack**

Write a letter to the company with your decision. 

In the letter list all files and describe what they contain.

In the case of collab, you can send an invitation to your file, but I still recommend sending HTML version in addition. 
If you use Plotly you might face the problem that graphs are not rendered in HTML.
To fix this problem, use the next code.

```
fig.show("png") # in such case graph becomes not interactive, but it will be showed by default in HTML

```
## Self-presentation

Still, you should remember that you are evaluated not just based on your tech task, your interview sometimes is even more critical.
Almost all interviews do have the same script. On the one hand, it is a good idea to follow it. On the other, it is better to be bright and memorable. 
For this aim, I highly recommend using an introduction presentation about yourself.

You can find my presentation [here](https://github.com/iliailinskii/test-cases/blob/main/Self%20presentation.pdf).

It is a good instrument
* to bring structure to your speech
* to show visually how you work
* attract interest in yourself

Thank you if you have read till the end.
Please, feel free to add your comments and thoughts and share your expirience!




