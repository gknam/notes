# Numpy


a = [[1, 2, 3], [4, 5, 6]]

### np.array(a)
Convert list into array. Each element in the array should be of same data type.

### a.shape
Show dimensions of array

### a.dtype
Show data type of elements.

### a.astype()
Converts data type
E.g. **a.astype("float")** converts values to float.

### np.sum(), np.max(), np.min()
Gets sum, max and min value of all elements in an array or specified dimension
**a.sum(axis=1)** returns [6, 15] - sums of rows.
**a.sum(axis=0)** returns [5, 7, 9] - sums of columns.


### np.genfromtxt()
Read in dataset
e.g. np.genfromtext("example.csv", delimiter=",", dtype="U75", skip_header=1) reads in "example.csv" parsing columns at ",", skipping first row and reading in "[each value as a 75 byte unicode data type](https://www.dataquest.io/m/6/getting-started-with-numpy/7/reading-in-the-data-correctly)"

### a[rowInd, columnInd]
Access element in matrix.
e.g. **a[1, 2]** returns 6.

### a[rowInd1:rowInd2, columnInd1: columnInd2]
Slice matrices by rows and columns

### a == value
This returns an array of boolean values which becomes "True" for all matching
elements (otherwise "False").
e.g. **a == 4** returns [[False, False, False], [True, False, False]]

### a[a == value] = newValue
This replaces value with newValue in the array.
E.g. **a[a == ""] = 0** replaces missing values with 0.

### (a == value1) | (a == value2)
Multiple comparisons. Each condition should be put in brackets.
e.g. **(a == 2) | (a == 5)** returns [[False, True, False], [False, True, False]]

# Other stuff
## Scientific notation
["We can represent 100 in scientific notation as 1e+02. The e+02 indicates that we should multiply what comes before it by 10 ^ 2(10 to the power 2, or 10 squared). This results in 1 * 100, or 100."](https://www.dataquest.io/m/6/getting-started-with-numpy/6/inspecting-the-data)

