# Binary Tree

一、樹的種類

1.  滿二元樹 :

節點數量 2n+1

1.  完全二元樹:

除了底層其他層都是滿的

1.  二元搜索樹:

左子樹小於中間節點，右子樹大於中間節點

1.  平衡二元樹:

左子樹減右子樹 高度絕對值不超過1

二、儲存方式

1. 鏈式儲存
2. 線性儲存
    
    2 * i +1 = 左元素
    
    2 * i +2 = 右元素
    

三、樹的遍歷

1. 深度優先搜索
    
    遞歸的方式實現(棧 stack)
    
2. 廣度優先搜索
    
    層序遍歷(對列 queue)
    

前中後序遍歷:

1. 遞歸遍歷
2. 迭代法

四、前中後序遍歷

          5

    4          6

1     2     7    8

(看中在哪)

1. 前序
    
    中左右  5 4 1 2 6 7 8
    
2. 中序
    
    左中右  1 4 2 5 7 8 6
    
3.  後序
    
    左右中  1 2 4 7 8 6 5
    

五、廣度優先搜索

遍歷三部曲：

1. 確定遞歸函數的參數返回值
    
    傳入頭節 Array
    
2. 確定終止條件
    
    遇到空節點
    
3. 確定單層遞歸的邏輯
    
    以前序遍歷為例:
    
    中 : 存入 Array
    
    左 : 傳入左節點、Array 
    
    右 : 傳入右節點、Array