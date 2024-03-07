## Task1
### def BinarySearch(nums, target):
    :param nums: list[int]
    :param target: int
    :return: int
```
if(len(list)==0):
	return 0
array.sort()
mid_index=len(array)/2
if(list(mid_index)==target):
	return True
	return self.BinarySearch(list[mix_index+1:],target) if target>list[mid_index] else\
	self.BinarySearch(list[mid_index-1:],target)
```
## Task 2
###### 2.矩阵加法,乘法

给定两个$n\times n$的整型矩阵 `A `和 `B `, 写两个函数 `MatrixAdd `和 `MatrixMul`, 分别得出这两个矩阵加法和乘法的结果.

两个矩阵的数据类型为嵌套列表, 即 `list[list]`, 且满足 `len(list)==n, len(list[0])==n`.

注意不要打乱原矩阵 `A` 和 `B` 中的数据.

```
def MatrixAdd(A, B):
    """
    :param A: list[list[int]]
    :param B: list[list[int]]
    :return: list[list[int]]
    """

def MatrixMul(A, B):
    """
    :param A: list[list[int]]
    :param B: list[list[int]]
    :return: list[list[int]]
    """
```
```
def MatrixAdd(A,B):
ans_mat = [[0]*n for i in range(n)] 
for i in range(n):
	for j int range(n):
		temp = A[i][j]+B[i][j]
		ans_mat[i][j] += temp
return ans_mat	
```
```
def MatrixMul(A,B):
ans_mat = [[0]*n for i in range(n)] 
for i in range(n):
	for j int range(n):
		temp = A[i][j]*B[i][j]
		ans_mat[i][j] += temp
return ans_mat	
```
## Task 3
###### 3.字典遍历

给定非空字典 `dict1` , 其键为姓名, 值是学号. 写一个函数 `ReverseKeyValue` 返回另一个字典, 其键是学号, 值是姓名.

例如, `dict1={'Alice':'001', 'Bob':'002}`, 则 `ReverseKeyValue(dict1)`返回的结果是 `{'001':'Alice', '002':'Bob'}`

```
def ReverseKeyValue(dict1):
    new_dict = {v:k for , in dict1.items()}
    return new_dict