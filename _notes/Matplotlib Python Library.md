
## Function oriented

### Useful functions
| Function | Use                                 |
| -------- | :---------------------------------- |
| plot     | To create a plot                    |
| title    | To name your plot                   |
| xlabel   | To add a label                      |
| ylabel   | To add a label                      |
| legend   | To show the legend of each line     |
| grid     | To create a grid for the plot       |
| show     | To show the grid once it's finished |
### The plot function
#### Function's keywords
`plot(x, y)`  plot x and y using default line style and color
`plot(x, y, 'bo')`  plot x and y using blue circle markers
`plot(y)`  plot y using x as index array 0..N-1
`plot(y, 'r+')` ditto, but with red plusses
#### Plotting labeled data
`plot('xlabel', 'ylabel', data=obj)` 
The above line can plot indexable objects. It can be for exemple to plot a `dict` or a `pandas.DataFrame` or a structured numpy array.

### Exemple

```python
import matplotlib.pyplot as plt
x = [0.2*i for i in range(31)]
x2 = [a**2 for a in x ]
x3 = [a**3 for a in x ]
plt.plot(x,x2, 'o:r', ms= 4, label="x^2")
plt.plot(x,x3, 'o:c', ms= 4, label="x^3")
plt.title("Fonctions x^2 et x^3")
plt.xlabel("x [cm]")
plt.ylabel("y ")
plt.legend()
plt.grid(color = 'green', linestyle = '--', linewidth = 0.5)
plt.show()
```


[![https://imgur.com/80djl0M.png](https://imgur.com/80djl0Ml.png)](https://imgur.com/80djl0Ml.png)

## Object oriented
[![https://matplotlib.org/cheatsheets/_images/handout-beginner.png|1000](https://matplotlib.org/cheatsheets/_images/handout-beginner.png)](https://matplotlib.org/cheatsheets/)

