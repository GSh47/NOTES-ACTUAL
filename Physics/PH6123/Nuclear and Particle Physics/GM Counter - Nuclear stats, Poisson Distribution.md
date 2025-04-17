
In addition to the material provided in the manual, I believe this will be useful to those especially interested in being proficient in handling data with python.

I have included the resulting plot with borrowed data for reference  
```python 
# Hi ! this is a python program I wrote for the GM COUNTER EXPERIMENT 
  
import pandas as pd  
import numpy as np  
import matplotlib.pyplot as plt  
from scipy.stats import poisson,norm  
   
### PROCESSING DATA ###  
  
file = 'name.csv' # rename as per filename
#include path if csv and code in different folders 
data = pd.read_csv(file, header=None) # reads the file  
  
mu, sigma = norm.fit(data)# calculates mean(mu) and std. deviation(sigma) of your data  
begin = mu - 3*(sigma)  
end = mu + 3*(sigma)  
x = np.linspace(begin,end,100)  # Here, I have set the plot range in accordance with the '3 sigma rule', feel free to use different values  
p = norm.pdf(x, mu, sigma)  # generates a poisson distribution for the data you've collected  

### PLOTTING ###  

# this is straightforward. feel free to tweak bin values, colors, resolution etc  

plt.subplot(2, 1, 1)  # Divides the screen for 2 plots and allots section 1 
plt.hist(data, bins=10,   alpha=0.7, color='#073642', label='Histogram')  
plt.xlim(begin,end)  
plt.xlabel('Count')  
plt.ylabel('Frequency')  
plt.subplot(2, 1, 2)  #  allots section 2  
plt.plot(x, p, 'k', linewidth=2)  
plt.plot(x, p, color='#073642', label=f'Poisson Fit (λ={mu:.2f})')  
plt.axvline(mu, color='red', linestyle='--', label='Mean (λ)')  
plt.title('GM COUNTER ')  
plt.xlabel('Count')  
plt.ylabel('probability')  
plt.legend()  
plt.show()

# Best regards
# Govinda S 21 PMC 67
```

