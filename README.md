# Matplotlib1

## 1 Problem 1 : Matplotplib - Introduction	(	https://www.geeksforgeeks.org/python-introduction-matplotlib/ )
import matplotlib.pyplot as plt

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.plot(x, y)
plt.show()
import matplotlib.pyplot as plt

x = [0, 2, 4, 6, 8]
y = [0, 4, 16, 36, 64]

fig, ax = plt.subplots()  
ax.plot(x, y, marker='o', label="Data Points")

ax.set_title("Basic Components of Matplotlib Figure")
ax.set_xlabel("X-Axis") 
ax.set_ylabel("Y-Axis")  


plt.show()


## 2 Problem 2 : Pyplot in Matplotplib (	https://www.geeksforgeeks.org/python-introduction-matplotlib/ )
import matplotlib.pyplot as plt

x = [0, 1, 2, 3, 4]
y = [0, 1, 4, 9, 16]

plt.plot(x, y)
plt.show()
import matplotlib.pyplot as plt

x = [0, 2, 4, 6, 8]
y = [0, 4, 16, 36, 64]

fig, ax = plt.subplots()  
ax.plot(x, y, marker='o', label="Data Points")

ax.set_title("Basic Components of Matplotlib Figure")
ax.set_xlabel("X-Axis") 
ax.set_ylabel("Y-Axis")  


plt.show()



## 3 Problem 3 : Matplotplib - Axes Classes	Matplotlib1	30	https://www.geeksforgeeks.org/matplotlib-axes-class/ )
import matplotlib.pyplot as plt 


fig = plt.figure() 

[left, bottom, width, height] 
ax = plt.axes([0.1, 0.1, 0.8, 0.8]) 

import matplotlib.pyplot as plt 


fig = plt.figure() 

[left, bottom, width, height] 
ax = fig.add_axes([0, 0, 1, 1]) 
import matplotlib.pyplot as plt 


fig = plt.figure() 

[left, bottom, width, height] 
ax = plt.axes([0.1, 0.1, 0.8, 0.8]) 

ax.legend(labels = ('label1', 'label2'), 
		loc = 'upper left') 
import matplotlib.pyplot as plt 
import numpy as np 


X = np.linspace(-np.pi, np.pi, 15) 
C = np.cos(X) 
S = np.sin(X) 

[left, bottom, width, height] 
ax = plt.axes([0.1, 0.1, 0.8, 0.8]) 

'bs:' mentions blue color, square 
marker with dotted line. 
ax1 = ax.plot(X, C, 'bs:') 

'ro-' mentions red color, circle 
marker with solid line. 
ax2 = ax.plot(X, S, 'ro-') 

ax.legend(labels = ('Cosine Function', 
					'Sine Function'), 
		loc = 'upper left') 

ax.set_title("Trigonometric Functions") 

plt.show() 




## 4 Problem 4 : Multiple Subplots	Matplotlib1	30	https://www.geeksforgeeks.org/how-to-create-multiple-subplots-in-matplotlib-in-python/
importing library
import matplotlib.pyplot as plt

Some data to display
x = [1, 2, 3]
y = [0, 1, 0]
z = [1, 0, 1]

Creating 2 subplots
fig, ax = plt.subplots(2)

Accessing each axes object to plot the data through returned array
ax[0].plot(x, y)
ax[1].plot(x, z)
importing library
import matplotlib.pyplot as plt
import numpy as np

Data for plotting
x = np.arange(0.0, 2.0, 0.01)
y = 1 + np.sin(2 * np.pi * x)

Creating 6 subplots and unpacking the output array immediately
fig, ((ax1, ax2), (ax3, ax4), (ax5, ax6)) = plt.subplots(3, 2)
ax1.plot(x, y, color="orange")
ax2.plot(x, y, color="green")
ax3.plot(x, y, color="blue")
ax4.plot(x, y, color="magenta")
ax5.plot(x, y, color="black")
ax6.plot(x, y, color="red")
import matplotlib.pyplot as plt

Create a 2x2 grid of subplots
fig, axs = plt.subplots(2, 2)

Now axs is a 2D array of Axes objects
axs[0, 0].plot([1, 2, 3], [4, 5, 6])
axs[0, 1].scatter([1, 2, 3], [4, 5, 6])
axs[1, 0].bar([1, 2, 3], [4, 5, 6])
axs[1, 1].hist([1, 2, 2, 3, 3, 3, 3, 3, 3, 4, 4, 5])

plt.show()
