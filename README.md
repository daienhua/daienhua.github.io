# 命名规范
### 1、类和接口命名
**规则：** 使用驼峰规则，首字母必须大写，使用名词或名词词组。要求简单易懂，富于描述，不允许出现无意义或错误单词。

 - 如：class UserFragment

### 2、方法的命名
**规则：** 使用驼峰规则，首字母必须小写，使用动词。要求简单易懂，富于描述，不允许出现无意义或错误单词。

 - 如：public String getUserName()

### 3、变量的命名
**规则：** 使用驼峰规则，首字母必须小写，使用名词或名词词组。要求简单易懂，富于描述，不允许出现无意义或错误单词。

 - 非静态成员变量命名以m开头，如：private int mScore = 0;
 - 静态成员变量命名以s开头，如：private static int sFlag = 0;

### 4、常量的命名
**规则：** 常量全为大写字母，以_分隔
如：public static final int CODE_REQUEST = 100;

### 5、布局文件的命名
**规则：** 使用**前缀_逻辑名称**命名，单词全部小写，单词间以下划线分割。

 - Activity对应的布局使用activity_ 开头，如：activity_home.xml;
 - Fragment对应的布局使用fragment_开头，如：fragment_message.xml;
 - Dialog对应的布局使用dialog_开头，如：dialog_logout_tips.xml;

### 6、资源文件的命名
**规则：** 使用**前缀_用途**命名，单词全部小写，单词间以下划线分割。

 - drawable:
    - btn_back_selector.xml 控件前缀命名
    - common_circle_gray.xml 通用资源多处使用common_开头

 - drawable_xxhdpi:
    - btn_back_normal.png 控件前缀名称
    - btn_bakc_press.png 控件前缀名称
    - ic_login_lock.png ic_+用途

### 7、布局文件中id的命名
**规则：** 使用驼峰命名，**前缀+逻辑名称**，不需要下划线分割

**控件前缀规则：**

 - TextView/EditText: tv
 - Button/RadioButton/ImageButton: btn
 - ImageView: img
 - RelativeLayout/LinearLayout/FrameLayout: layout
 - ListView: listView
 - WebView: webView
 - CheckBox: checkBox

 - 如：TextView @+id/tvTitle
 - 如：EditView @+id/tvName
 - 如：Button @+id/btnSearch


#约定
 - Activity.onCreate()，Fragment.onActivityCreated()，作为程序入口，不用写入太多代码，尽量保持只调用initXXX()方法，简单明了展示调用过程。如：initData()，initView()。
 - 单个方法体不要过长，拆分臃肿方法，每个方法只作一件事
 - 做同一个逻辑的方法，尽量靠近放到一块，方便查看
 - 统一调整IDE的Tab缩进为4个空格
 - 空行的使用，拒绝拖沓无分割，关联代码段放一块并与后面代码分割
 - 用好TODO标记
    - 记录想法，记录功能点，开发过程中可以利用TODO记录一下临时想法或为了不打扰思路留下待完善的说明
    - 删除无用TODO，开发工具自动生成的TODO，或则已经完善的TODO，一定要删除。
 - 所有意义数字全部抽取到Constant公共类中，避免散布在各位类中
 - 使用JSON工具类，不要手动解析和拼装数据
 - 使用ButterKnife注解代替findViewById
 -

