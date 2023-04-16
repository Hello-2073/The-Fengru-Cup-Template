## 第三十三届“冯如杯”竞赛主赛道论文

本模板是为第三十三届“冯如杯”竞赛主赛道设计的Latex模板，基于以下作品
改进而来，将作为官方模板供同学们使用。

本模板原始版本来源于[此仓库](https://github.com/Somedaywilldo/Someday-XeLaTex-Template)，作者 Somedaywilldo 完成了此模板的第一个版本。

本模板第二版本来源于[此仓库](https://github.com/cpfy/FRB_template.git)，作者 cpfy 针对第三十二届赛制格式要求做出了多处适配与调整。

## 使用方法
本模板主文件为FRBTemplate.tex，请使用XeLatex编译。


## 修订版本更新内容（2023年4月16日）
* 修改图表标题大小，加入`font={small}`
```
\captionsetup[figure]{font={small}, labelfont=bf, labelsep=mysep, textfont=bf}   %图片caption格式
\captionsetup[table]{font={small}, labelfont=bf, labelsep=mysep, textfont={bf}}   %表格caption格式
```
* 修改表格字体大小
在表格开始处插入`\small`
```
\begin{table*}[t]
\small
\centering
\caption{表格使用示例}
\begin{tabular}{|l||c|c|c|c|c|c|}
\hline
{\textbf{表头 1}}     &  表头 2 	    & 表头 3 	  & 表头 4     & 表头 5 		\\ \hline\hline
内容 11 		          & 内容 12				& 内容 13		& 内容 14 	 & 内容 15		\\ \hline
内容 21	              & 内容 22				& 内容 23		& 内容 24	   & 内容 25		\\ \hline
\end{tabular}
\end{table*}
```
* 修复标题英文显示异常问题
```
\begin{spacing}{3}
    % \erhao
    \begin{center}
      {
        \fontsize{22pt}{3}\selectfont
        \zhongsong{第三十三届“冯如杯”竞赛主赛道项目论文Latex模板} %黑体这样调用，其余字体同理
      } 
        % \zhongsong{“冯如杯”竞赛主赛道项目是什么}
    \end{center}
    \rightline{\xinwei\sanhao{——基于 Latex 的论文模板}} % XSP 2023/3/3: 副标题二号华文新魏居右
\end{spacing}
```

## 本版本更新内容（2023年3月20日）
* 全局
  * 修改纸张大小为A4
  * 修改正文段落间距为0
  * 修改条标题的顿号为逗号

* 封面
  * 调整校徽和校名的位置
  * 导入华文新魏字体，设置副标题为三号华文新魏居右

* 摘要
  * 英文摘要标题加粗

* 目录
  * 加入结论、参考文献等无标号章节

* 正文
  * 修复页眉与正文对齐的问题，同时调整了合适的页边距
  * 将正文标题字体由加粗（\bfseries）修改为黑体

* 参考文献
  * 由于Bib对要求格式支持不全，暂时使用手动排版

* 内容
  * 修改模板内容为冯如杯格式规范

