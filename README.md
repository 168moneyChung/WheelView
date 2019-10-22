# WheelView

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-WheelView-green.svg?style=true)](https://android-arsenal.com/details/1/3853 ) [![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14 )

Android滾輪控件，基於ListView實現，可以自定義樣式。

Features
--
* 支持自定義滾輪樣式
* 支持common和holo兩種皮膚
* 支持文本和圖文混排兩中數據模版
* 支持循環顯示數據
* 支持選中項添加附加文本
* 支持設置滾輪刻度
* 支持聯動功能
* 支持嵌入滾動控件中([NestedScrollView](https://github.com/venshine/WheelView/blob/master/wheelview/src/main/java/com/wx/wheelview/widget/NestedScrollView.java))
* 支持滾輪對話框
* 支持滾輪選中項點擊事件

<li>| void **setWheelAdapter**(BaseWheelAdapter<T> adapter) | 設置滾輪數據源適配器（required） |</li>
<li>| void **setWheelData**(List<T> list) | 設置滾輪數據（required） |</li>
<li>| void **setLoop**(boolean loop) | 設置滾輪是否循環滾動 |</li>
<li>| void **setWheelSize**(int wheelSize) | 設置滾輪個數 |</li>
<li>| void **setSkin**(Skin skin) | 設置皮膚風格 |</li>
<li>| Skin **getSkin**() | 獲得皮膚風格 |</li>
<li>| void **setStyle**(WheelViewStyle style) | 設置滾輪樣式 |</li>
<li>| WheelViewStyle **getStyle**() | 獲得滾輪樣式 |</li>
<li>| void **setWheelClickable**(boolean clickable) | 設置滾輪選中項是否可點擊 |</li>
<li>| void **setSelection**(final int selection) | 設置滾輪位置 |</li>
<li>| int **getSelection**() | 獲取滾輪位置 |</li>
<li>| void **join**(WheelView wheelView) | 連接副WheelView（聯動設置） |</li>
<li>| void **joinDatas**(HashMap<String, List<T>> map) | 副WheelView數據（聯動設置） |</li>
<li>| int **getCurrentPosition**() | 獲取當前滾輪位置 |</li>
<li>| T **getSelectionItem**() | 獲取當前滾輪位置的數據 |</li>
<li>| void **setExtraText**(String text, int textColor, int textSize, int margin) | 設置選中行附加文本 |</li>
<li>| int **getWheelCount**() | 獲得滾輪數據總數 |</li>
<li>| void **setOnWheelItemSelectedListener**(OnWheelItemSelectedListener<T> onWheelItemSelectedListener) | 設置滾輪滑動停止時事件，監聽滾輪選中項 |</li>
<li>| void **setOnWheelItemClickListener**(OnWheelItemClickListener<T> onWheelItemClickListener) | 設置滾輪選中項點擊事件 |</li>
<li>| WheelViewDialog **setDialogStyle**(int color) | 設置Dialog外觀顏色 |</li>

History
--
* 1.0.0(2016-03-24)
    - 完成滾輪控件
* 1.1.0(2016-03-28)
    - 支持聯動功能
* 1.2.3(2016-04-14)
    - 支持嵌入滾動控件
* 1.3.0(2016-04-15)
    - 支持滾輪對話框
* 1.3.1(2016-04-18)
    - 增加滾輪選中項點擊事件
