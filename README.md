# Data analyst tech tasks

During my career, I have faced many different tech tasks for data analysis. In this repository, you can find my solutions and a couple of recommendations for analysts. 
## Repository structure
* Real tech tasks solutions
* Best practice
* How to introduce yourself 
## Real tech tasks solutions
All cases in this repository are real interview tech tasks for a senior data analyst position, mostly in marketing or growth teams.
I rename companies to protect their anonymity. 
I chose only successful tech tasks. Thus, you can see an acceptable work level for successful data analyst tech interview completion. 
Basically, there are 3 types of tech interviews for data analysts:
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
This is a fintech company. The task challenges analyst's ability to analyze cohorts and work as a growth-hacker.

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
This is a fintech company that distributes digital subscription products. The task is focused on marketing analysis and testing the ability of channels evaluation.

Case content:
* [Task description](https://github.com/iliailinskii/test-cases/blob/main/company%20d/Company%20%20D%20tech%20task.pdf)
* [Solution scripts](https://github.com/iliailinskii/test-cases/blob/main/company%20d/Company%20D%20scripts.ipynb)

## Best practice
Here I collected main points of how to complete analyst tech task and some small tips for it.

### Choose instrument 
Nowadays, there are lots of instruments that allow you to demonstrate your analyst skills. 
I suppose [Jupyter Notebooks](https://jupyter.org/install) to be one of the most widespread ones. There is a number of pros to using it:
- Use python for working with data
- Ability to organize research structure
- Convenient markdowns system, so you can follow your scripts with comments and conclusions
- Standard format 

So you can write scripts and presentations for research all in one. 
By the way, I conduct all my studies in [Colab](https://colab.research.google.com/notebooks/basic_features_overview.ipynb). I chose it because I had only the old-fashioned laptop with 2 cores processor and sometimes worked in the library public computers. Thus, Colab let me not be limited with laptop resources and be flexible in working on the project from different devices. Among other pros Colab is much easier to set up. In fact, you need just open the link and also you can share it by link. 
> Small tip. You can use Colab Pro version with GPU and additional RAM for 10 euros per month. And still, all these things are highly affordable, because you can have lots of calculation resources even on the super cheap devices (in extremal case even on tablet or smartphone)

### Instrument to demonstrate SQL skills
In the beginning, I highly recommend trying this [site](https://sqliteonline.com/). Here you can import CSV files and work with them on SQL lite. Also, you can deploy MariaDB, Postrgres, or MS SQL locally and use this site as an interface. 

However, sqliteinline has limits for table size and you can not make a dashboard in it to share your results by link. That's why I suggest using [pandasql](https://pypi.org/project/pandasql/) in combination with Jupyter Notebook. In such approach, you can demonstrate all your skills in one document.
> Small tip. If you use pandasql you need to format your values to 8-bit datatype. It is SQL lite limit. 

### How to organize proccess
Tech task usually is quite a stressful process. That is why having a plan allow you keep focus and worry less. 
Surprisingly, most of the tasks are structured the same. You have a dataset, its description (hopefully), and a task list. 
>  It is critical to understand what the company wants to test to make a good solution. 
From my managerial expirience, I suppose most the companies follow aim to test candidates for the next skills.
- Work process organization
- Ability to work with the new dataset
- Understanding of metric tree in the company field (funnels, unit economy, statistics, etc)
- Python / SQL level
- Data Visualisation 
- Make conclusions and insights based on Data

Based on these information we can tune our approach for task solution.
I suggest following the next checklist in every solution.

1. Read the task mindfully and the dataset description
2. If there is no dataset description, have a look at it (how to do it in the next parts)
3. Create a research plan.
>  I know that research is a creative process and most analysts create a plan during working with data. However, in a test task, you do not have enough time to spend in a such way.
4. Describe your plan in Notebook
5. Read the data
6. Clear data
7. Create an analytical platform for yourself. It includes all your scripts to complete the task.
8. Reassume scripts and reorganize them to save only the working hypothesis to make it clearer for the examinator
9. Tune visualizations
10. Write down conclusions and markdown comments on scripts
11. Make a presentation to the manager
12. Create a solution pack, describe it and send it to the company

Doing our best at every of these points we will increase our chances to pass the test.
You can see that most of them are very universal for any tasks. Thus, I think my advice will work for the magority of analyst tech tasks.

### Tips to improve solution
*Read test task*











 

