# Welcome

Data quality profiling and exploratory data analysis are crucial steps in the process of Data Science and Machine Learning development. 
YData-profiling is a leading tool in the data understanding step of the data science workflow as a pioneering Python package. 

`ydata-profiling` is a leading package for data profiling, that automates and standardizes the generation of detailed reports, 
complete with statistics and visualizations. The significance of the package lies in how it streamlines the process of
understanding and preparing data for analysis in a single line of code! If you're ready to get started see the [quickstart](getting-started/quickstart.md)!

!!! tip "Advent of Code - Get featured on ydata-profiling"

    *“I want to get into open source, but I don’t know how.”* - Does this sound familiar to you? Have you been wanting to
    get more involved with open-source software, but no one’s given you an entry point?
    
    That's why we joined [The Advent of code this year](https://zilliz.com/advent-of-code). Contribute to ydata-profiling and win some 🐼🐼 swag!

    How can you be part of it?
    
    - Give us some love with a Github ⭐
    - Write an article or create a tutorial like other [members the community already did.](https://medium.com/@seckindinc/data-profiling-with-python-36497d3a1261)
    - Feeling adventurous? Contribute with a PR. We have a list of [great issues to get you started.](https://github.com/ydataai/ydata-profiling/issues?q=label%3A%22getting+started+%E2%98%9D%22+)

![ydata-profiling report](_static/img/ydata-profiling.gif)

## Why use ydata-profiling?

`ydata-profiling` is a valuable tool for data scientists and analysts because it streamlines EDA, provides comprehensive insights, enhances data quality,
and promotes data science best practices.

- **Simple to user**: It is so **simple to use** - a single line of code is what you need to get you started. *Do you really need more to convince you?* 😛
```python linenums="1"
import pandas as pd
from ydata_profiling import ProfileReport

df = pd.read_csv('data.csv')
profile = ProfileReport(df, title="Profiling Report")
```
- **Comprehensive insights in a report**: a report including a wide range of statistics and visualizations, 
providing a holistic view of your data. The report is shareable as a html file or while integrate as a widget in a Jupyter Notebook. 
- **Data quality assessment**: excel at the identification of missing data, duplicate entries and outliers. These insights are essential
for data cleaning and preparation, ensuring the reliability of your analysis and leading to early problems' identification.
-  **Ease of integration with other flows**: all metrics of the data profiling can be consumed in a standard JSON format.
- **Data exploration for large datasets**: even with dataset with a large number of rows, `ydata-profiling` will be able to help you
as it supports both Pandas Dataframes and [Spark Dataframes](integrations/pyspark.md).

To learn more about the package check out [concepts overview](getting-started/concepts.md).

## 📝 Features, functionalities & integrations
YData-profiling can be used to deliver a variety of different applications. The documentation includes guides, tips and tricks for tackling them:

!!! question "Data Catalog with data profiling for databases & storages"

    Need to profile directly from databases and data storages **(Oracle, snowflake, PostGreSQL, GCS, S3, etc.)**?
    
    Try [YData Fabric Data Catalog](https://ydata.ai/products/data_catalog) for interactive and scalable data profiling

    Check out the [free Community Version](http://ydata.ai/register?utm_source=ydata-profiling&utm_medium=documentation&utm_campaign=YData%20Fabric%20Community).

| Features & functionalities                                                       | Description                                                                                 |
|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| [Comparing datasets](features/comparing_datasets.md)                             | Comparing multiple version of the same dataset                                              |
| [Profiling a Time-Series dataset](features/time_series_datasets.md)              | Generating a report for a time-series dataset with a single line of code                    |
| [Profiling large datasets](features/big_data.md)                                 | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
| [Handling sensitive data](features/sensitive_data.md)                            | Generating reports which are mindful about sensitive data in the input dataset              |
| [Dataset metadata and data dictionaries](features/metadata.md)                   | Complementing the report with dataset details and column-specific data dictionaries         |
| [Customizing the report's appearance](features/custom_report_appearance.md )     | Changing the appearance of the report's page and of the contained visualizations            |
| [Profiling Relational databases **](features/collaborative_data_profiling.md)    | For a seamless profiling experience in your organization's databases, check [Fabric Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume data from different types of storages such as RDBMs (Azure SQL, PostGreSQL, Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake, etc.), among others. |
| [PII classification & management **](features/pii_identification_management.md ) | Automated PII classification and management through an UI experience          |

### Tutorials

Looking for how to use certain features or how to integrate `ydata-profiling` in your currect stack and workflows,
check our step-by-step tutorials. 

- **How to master exploratory data analysis with ydata-profiling?** Check this [step-by-step tutorial](https://medium.com/ydata-ai/auditing-data-quality-with-pandas-profiling-b1bf1919f856).
- **Looking on how to do exploratory data analysis for Time-series 🕛?** Check how to in this 
[blogpost](https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
To learn more about this feature [check the documentation](features/time_series_datasets.md).
- **How to compare 2 datasets? We got you covered with this [step-by-step tutorial](https://medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-pandas-profiling-2ae3a9d7695e)**
To learn more about this feature [check the documentation](features/comparing_datasets.md).
- **Want to scale for larger datasets?** Check the information about release with ⭐⚡[Spark support](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)!
For more information about spark integration [check the documentation](integrations/pyspark.md)

## 🙋 Support
Need help? Want to share a perspective? Report a bug? Ideas for collaborations? Reach out via the following channels:

- [Stack Overflow](https://stackoverflow.com/questions/tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how to use the package
- [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
- [Discord](https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions, ask questions, collaborations, general chat

!!! tip "Help us prioritizing - before reporting, double check, it is always better to upvote!"
    
    Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).

    If you want to validate if your request was prioritized check the [project pipeline details]()

## 🤝🏽 Contributing

Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).

A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://tiny.ydata.ai/dcai-ydata-profiling).

A big thank you to all our amazing contributors! 

### ⚡ We need your help - Spark!

Spark support has been released, but we are always looking for an extra pair of hands 👐.
[Check current work in progress!](https://github.com/ydataai/ydata-profiling/projects/3).
