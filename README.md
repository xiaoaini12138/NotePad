# Notepad
* 期中实验

## 主界面  

![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/09.png)

## 更改了图标美化了界面

# 说明

## 新建Note

![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/01.png)

## 增加Note搜索索引

![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/02.png)
![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/03.png)
## 输入index 后左上角会显示index


## 创建同样的两个Note B、C和D

![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/04.png)
![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/05.png)
![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/06.png)

## 搜索Note 的Index 

![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/07.png)
![image](https://github.com/xiaoaini12138/Notepad/blob/master/screenshot/08.png)

//源码
  public SimpleCursorAdapter(Context context, int layout, Cursor c, String[] from, int[] to) {
      super(context, layout, c);
      mTo = to;
      mOriginalFrom = from;
      findColumns(c, from);
  }
  ```
  ```
   //from 第二项为增加项 下同
   String[] dataColumns = {NotePad.Notes.COLUMN_NAME_TITLE,  NotePad.Notes.COLUMN_NAME_MODIFICATION_DATE};

   //to
   int[] viewIDs = {android.R.id.text1, R.id.tv_time_stamp};
  ```
