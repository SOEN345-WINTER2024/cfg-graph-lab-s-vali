Sofia Valiante 40191897

## Basic Calculator
![IMG_2063](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/876ffc93-b3e2-44cc-a03c-539c272971a7)
![IMG_2064](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/6b6c2971-a45b-402a-8734-8453791c9939)

## Android App
Method:
protected void applyCustomTheme() { ... }

1) CFG

![code2flow_aotaKM](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/9701a6eb-4d00-46ef-b1f3-dcd5dcdfe3b9)
![IMG_2065](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/83f1d3ed-d961-4bcd-92e4-4311a36eaf99)

2) Node coverage
<br> TR = { 1, 2, 3, 4, 5, 6, 7, 8, 9 }
<br> TP = { (1,2,4,5,7,8,9), (1,2,3,5,7,9), (1,2,4,5,6,7,9) }

3) Edge coverage
<br> TR = { (1,2), (2,3), (2,4), (3,5), (4,5), (5,6), (5,7), (6,7), (7,8), (8,9), (7,9) }
<br> TP = { (1,2,4,5,7,9), (1,2,4,5,7,8,9), (1,2,3,5,7,9), (1,2,4,5,6,7,9) }

4) Edge-pair coverage
<br> TR = { [1,2,3], [1,2,4], [2,3,5], [2,4,5], [3,5,6], [3,5,7], [4,5,6], [4,5,7], [5,6,7], [5,7,8], [5,7,9], [6,7,8],  [6,7,9], [7,8,9] }
<br> TP = { [1,2,3], [2,3,5], [3,5,7], [5,7,9], [1,2,4], [2,4,5], [4,5,7], [5,7,9], [1,2,3], [2,3,5], [3,5,6], [5,6,7], [6,7,9], [1,2,4], [2,4,5], [4,5,6], [5,6,7], [6,7,9], [1,2,4], [2,4,5], [4,5,7], [5,7,8], [7,8,9], [1,2,4], [2,4,5], [4,5,6], [5,6,7], [6,7,8], [7,8,9] }

5) 
