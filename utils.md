# 一些脚本和工具

## 一键评教

```js
$('input[name*=fs]').each(function(){$(this).val(Math.round(1+6*Math.random()))})
```

当你想要选课时，发现评教阻碍你？一键脚本帮你忙！

评教的主要困难在于打分，本脚本旨在一键为您将**一节课**的分全部打完，对于文字评论，
请自行动手。

使用方法：进入教评系统，**打开某一节课**，按下 F12，找到控制台(console)界面，
在控制台中复制粘贴上述脚本然后回车运行，相关分数即打好。需要注意的是，打分后
星星不会亮（无回显），这是正常现象，请放心填写文字评论后提交。

然后脚本中的 1 + 6可以调整为 5 + 2，3 + 4 等各种组合，可根据需要自行调整。
需要注意的是不能打 0 分，即至少有 1 分保底分（0 + 7 是不可行的），
然后对于 6 + 1 或 7 + 0，提交时会提醒评分过高，请自行把握。

credit: [Konano](https://github.com/Konano)

## 选课冲突标记

你还在为抢课时满怀期待提交选课，却发现时间冲突而错失选课吗？
你还在一边记忆已选课时间，一边对照开课列表而感到缓慢吗？
这个脚本帮你忙！

这个脚本检测你已经选好的课，自动将候选课中有冲突时间的课标红，使得你浏览
百万课程时速度有如神助。当鼠标在在标红的时间上悬停时，会显示所有与其冲突的课程。

需要注意的是，现在未对半学期课做完全支持，也就是说可能出现假的时间冲突；
同时在开课信息以及选课查询界面无法工作，只在选课操作界面工作。

本脚本在 aux/TsinghuaCourseConflictMarker.user.js 中，需要使用油猴安装。

或者可以通过访问[这里](https://greasyfork.org/en/scripts/408340-tsinghuacourseconflictmarker)
来一键获得脚本。

现在已经增加 webvpn 支持。

感谢 [CircuitCoder](https://github.com/CircuitCoder) 提供的技术指导
感谢 [SharzyL](https://github.com/SharzyL) 的建议与 DEBUG
