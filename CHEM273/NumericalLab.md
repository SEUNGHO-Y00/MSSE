Function Review

1. def Tiles(N = 100):
* default value
* Define a function ONCE, then call it as many times as you would like

2. Indexing
* V = np.random.uniform(0,1(N,1))
* D = np.zeros((N,N))
* What data type are V or D? 2D NumPy Array

3. Indexing
* "Chained Indexing" is something like this: X[0][0] this works, but what happens is two steps:
  - X[0] = will return a 1D array
  - [0] = indexing into that row
* Instead to easily get a value at a given set of indices, use X[0,0] which is more efficient and faster in NumPy
  - X[0][0] == X[0,0] but X[0,0] is faster

4. Testing
* You must test your code!
* Many of the errors I saw could have been avoided by a single print statement
* Best practice before you submit:
  - Restart your kernel
  - Re-run all of your cells
  - Ensure your output looks reasonable

5. Formatting
* Import statements should occur ONCE in the beginning of your file
* Include cells where you tested the timing (not just comments)
* Label the questions, and use relevant function names

6. Integral Practice
* Integral 12dy => 12y + c

* Integral 4x^6 - 2x^3 + 7x - 4dx => 4/7x^7-1/2x^4+7/2x^2-4x+c

* Integral (2sin(x) - cos(x)dx => -sin(x) - 2cos(x) + C

* Integral(0->2) f(x)dx => 4

* Integral(1->6) (12x^3 - 9x^2 + 2)dx => 3x^4 - 3x^3 + 2x from 6 to 1 => 6 - 1 => 3252 -2 = 3250

* Integral (4x +25y^2)dx => 2x^2+25y^2x+c

* Determine f(x) given that f'(x) = 12x^2 -4x and f(-3)=17 => 4x^3 - 2x^2 + c => c = 143
