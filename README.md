# data-science
import numpy as np
my_list = [1, 2, 3, 4, 5, 6]
my_array = np.array(my_list)
csv_array = np.genfromtxt('sample.csv', delimiter=',')
a = np.array(l)
a_plus_3 = a + 3

import numpy as np

temperatures = np.genfromtxt('temperature_data.csv', delimiter=',')

print(temperatures)

temperatures_fixed = temperatures + 3

print(temperatures_fixed)

monday_temperatures = temperatures_fixed[0,:]

thursday_friday_morning = temperatures_fixed[3:5,1]

temperature_extremes = temperatures_fixed[(temperatures_fixed < 50) | (temperatures_fixed > 60)]


import numpy as np

cupcakes = np.array([2, 0.75, 2, 1, 0.5])

recipes = np.genfromtxt('recipes.csv', delimiter=',')

print(recipes)

eggs = recipes[:, 2]
print(eggs)
one_egg = recipes[(eggs == 1)]
print(one_egg)
cookies = recipes[2, :]
double_batch = cupcakes * 2
grocery_list = cookies + double_batch
print(grocery_list)

example_array = np.array([24, 16, 30, 10, 12, 28, 38, 2, 4, 36])

example_average = np.average(example_array)
