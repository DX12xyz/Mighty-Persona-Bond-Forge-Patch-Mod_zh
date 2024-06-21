## Mighty-Persona-Bond-Forge-Patch-Mod_zh
DX12_XYZ的机翻润色汉化,  
该mod为人格武器制造添加了更多mod联动配方,  
这里是大家一起汉化的地方，以下是向我发送汉化的方法和提交标准
# 1. GitHub分支
这个我还不会弄，你只能百度或者[GitHub文档](https://docs.github.com/zh/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches)  
简单来说是复制一份这个项目，然后自己添加汉化文件，然后提交合并分支
# 2.Excel to mail
你需要弄一个Excel表格按照以下格式制作然后发送到我的邮箱1715989736@qq.com  
文件名称 = 联动mod.xlsx
原物品中文 | PBF物品英文 | 联动mod对象标签 | PBFmod对象标签
-- | -- | ----- | -----
名字 | name | xxx.label | PBF_XX_XXX.label
名字 | name | xxx.description | PBF_XX_XXX.description
名字 | name | xxx.jobString | PBF_XX_XXX.jobString
...
  
注意:中文是必须的，而英文、标签等是可选的，如果联动mod没有中文或中文太老则优先使用边缘汉化组的汉化mod再考虑其他汉化且要在文件头标注使用哪位的汉化  
如果你想提取文本标签你可以看那些汉化教程或者：  
找到你要汉化的东西  
在你的steam文件夹下去到\steamapps\workshop\content\294100\2802598983找PBFmod的文件夹和去到要联动mod的文件夹:\steamapps\workshop\content\294100\创意工坊ID  
在PBFmod文件夹下看看有没有和要联动mod的名字相像的文件，用Visual Studio Code,notepad++,或者windos自带的文本编辑器和其他文本编辑器打开  
联动mod找找有Def名称的文件夹，里面可能有你你要汉化的东西，同上打开它
搜索你要汉化的东西的名字或者介绍，找到<PBF_XX_XXX.label>name</PBF_XX_XXX.label>,其中XX_XXX可能包含这个东西在另一边(联动mod)的标签名字(请全找完，有写代码是注册用的)  
.label可以是其他的东西如.description，如果没有用你要汉化的东西的名字或者介绍机翻看联动mod哪那个意思更相近  
下面是举例  
PBFmod   
```xml
<xxx>PBF_XX_XXX_name</xxx>
  <label>PBFname</label>
```
联动mod
```xml
<xxx>XX_XXX_name</xxx>
  <label>name</label>
```
其中`<xxx>PBF_XX_XXX_name</xxx>`是东西的PBF标签，`<xxx>XX_XXX_name</xxx>`是东西的联动mod标签,label是他们各自的显示名称
