# Matplotlib_and_Seaborn

    Both Matplotlib and Seaborn are third-party Python libraries for data visualization, meaning we
    need to install them separately (pip install matplotlib seaborn).

**Matplotlib vs Seaborn: Basics and various Charts**

  **1. Matplotlib**
  
      >> Matplotlib is a low-level visualization library in Python that provides complete control over graphs and plots.
      >> It works well for creating customized and detailed visualizations but requires more coding.

How to import?

    import matplotlib.pyplot as plt
    
**Common Charts in Matplotlib**
   
     1.Line Plot (plt.plot())
   
     2.Bar Chart (plt.bar())
   
     3.Histogram (plt.hist())
   
     4.Scatter Plot (plt.scatter())
   
     5.Pie Chart (plt.pie())

**Seaborn** 

    >> Seaborn is a high-level visualization library built on top of Matplotlib
    >> It is designed for statistical visualizations and works well with Pandas DataFrames.
    >> It provides prettier and less code-intensive visualizations.

How to import?

    import seaborn as sns
    
**Common Charts in Seaborn**

    1.Scatter Plot (sns.scatterplot())
  
    2.Line Plot (sns.lineplot())
  
    3.Bar Plot (sns.barplot())
  
    4.Box Plot (sns.boxplot())
  
    5.Histogram(sns.histplot())
  
    6.Heatmap (sns.heatmap())

**When to Use Each Chart?**


| **Chart Type**   | **Used For**                                      | **Matplotlib Function** | **Seaborn Function**  | 
|----------------- |---------------------------------------------------|-------------------------|-----------------------|
| **Line Plot**    | Trends over time, continuous data                 | plt.plot()              |  sns.lineplot()       | 
| **Bar Chart**    | Comparing categories                              | plt.bar()               |  sns.barplot()        |
| **Histogram**    | Distribution of a single variable                 | plt.hist()              |  sns.histplot()       |
| **Scatter Plot** | Relationship between two numerical variables      | plt.scatter()           |  sns.scatterplot()    | 
| **Box Plot**     | Distribution & outliers                           | NA                      |  sns.boxplot()        |
| **Heatmap**      | Correlation between multiple variables            | NA                      |  sns.heatmap()        | 
| **PieChart**     | Show proportion of a whole                        | plt.pie()               |   NA                  |



**Matplotlib vs. Seaborn: How to Pass Data**



| **Library**     | **Data Format**    |                 **Example**                   |
|-----------------|--------------------|-----------------------------------------------|
| **Matplotlib**  | List/Array         |         plt.plot([1,2,3], [10,20,30])         |
| **Matplotlib**  | Dictionary         |         plt.bar(data["x"], data["y"])         |
| **Seaborn**     | List/Array         |      sns.scatterplot(x=[1,2,3], y=[10,20,30]) |
| **Seaborn**     | DataFrame          |      sns.lineplot(x="col1", y="col2", data=df)|
| **Seaborn**     | 2D Array (Heatmap) |      sns.heatmap(np.array([[1,2],[3,4]]))     |


**Key Takeaways**: 

       >> Matplotlib accepts lists, NumPy arrays, and dictionaries.  
       >> Seaborn works best with Pandas DataFrames but also supports lists and NumPy arrays.
       >> Seaborn requires `data=df` when using column names.  
       >> Heatmaps in Seaborn require a 2D array or DataFrame. 

