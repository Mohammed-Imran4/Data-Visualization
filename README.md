Basic defintion of Matplotlib and solving the some questions:
1.Line plot Bar, horizontal bar ,Scatter, Histogram ,KDE Boxplot, Violin, Stacked bar Area plot Error bar, Pie chart ,Doughnut chart ,Stem plot
2.Stackplot Hexbin plot,plt.figure() plt.subplots() 
3.fig, ax usage Canvas vs Axes explanation Basic plot example,
4. Customizations Titles, labels Legend Colors, linewidth, linestyle Marker styles Grid Figure size,
5. Subplots plt.subplot() plt.subplots() Sharing axes Tight layout,
6. Styles & Themes plt.style.use() Custom colors (name, HEX, RGB) ✔
7. Saving Figures

1. What is Matplotlib?
Matplotlib is a Python library used to create visualizations such as line plots, bar charts, pie charts, scatter plots, etc.
It gives:
Low-level control → every pixel can be customized
Flexible → supports almost any type of plot
Works with NumPy, Pandas, Seaborn

2. Why do we use Matplotlib?
We use it because:
Highly customizable
Can produce publication-quality charts
Supports multiple plot types
Easy to integrate with machine learning and data analysis

3. Installation:
pip install matplotlib

4. Import Syntax:
import matplotlib.pyplot as plt

5.What is a Figure? (Canvas)
The overall window or page where plots appear.

6.What is Axes? (Plot area)
The area inside the figure where the visual graph is drawn.
Axes contains: title, ticks, x/y labels, plot lines, etc.

 7.## Basic Plot Types (Definitions Only)
a.Line Plot:
Shows change over continuous data (time, sequence).
plt.plot(x, y)

b.Bar Plot:
Used for comparing categories.
plt.bar(x, height)

c.Horizontal Bar Plot:
Same as bar but horizontal.
plt.barh(y, width)

d.Scatter Plot:
Shows relationship between two numeric variables.
plt.scatter(x, y)

e.Histogram:
Shows frequency distribution of data.
plt.hist(data)

f.KDE Plot:
Kernel Density Estimation — smooth version of histogram.
sns.kdeplot(data)

g.Boxplot:
Shows distribution using quartiles & outliers.
plt.boxplot(data)

h.Violin Plot:
Combines boxplot + KDE (distribution shape).
plt.violinplot(data)

i.Stacked Bar Plot:
Shows total + contribution of subsets.
plt.bar(x, a)
plt.bar(x, b, bottom=a)

j.Area Plot:
Continuous filled region under a curve.
plt.fill_between(x, y)

k.Error Bar Plot:
Shows measurement uncertainty.
plt.errorbar(x, y, yerr=error)

l.Pie Chart:
Circular chart showing percentage composition.
plt.pie(values)

m.Doughnut Chart:
Pie chart with a hole in the center.
plt.pie()
# add circle in middle

n.Stem Plot:
Shows discrete data as lines with a marker at top.
plt.stem(x, y)

o.Stackplot:
Plots multiple datasets stacked on top over X.
plt.stackplot(x, y1, y2)

p.Hexbin Plot:
Shows density of points in hexagonal bins.
plt.hexbin(x, y)

8. ## Customization Options
Title:
plt.title("My Plot")

X and Y Labels:
plt.xlabel("X axis")
plt.ylabel("Y axis")

Legend:
plt.legend()

Colors
You can use:
color name: "red"
hex code: "#00ff00"
RGB tuple: (0.5, 0.2, 0.8)

Line Width:
plt.plot(x, y, linewidth=3)

Line Style:
plt.plot(x, y, linestyle="--")

Marker Styles:
plt.plot(x, y, marker="o")

Grid:
plt.grid(True)

Figure Size:
plt.figure(figsize=(8, 5))












































































