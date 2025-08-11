# 1.1   Move The Cursor
# 1.2   Deletion Commands
dw,de,d$,dd
# 1.3   The Put Command
p,r,

c跟d差不多，但c组合指令会直接进入insert mode，而d组合指令不会进入insert mode

ce，修改至e定位的位置，即词尾

cb=db+i
# 1.4   Cursor Location and File Status
ctrl-g,gg,G,number+G
/,?,n,N
ctrl-o,ctrl-i
%，括号匹配
:s/old/new，向下匹配替换
:s/old/new/g，向下匹配替换全部
:#,#s/old/new/g，在#~#行内进行匹配替换
:%s/old/new/g，整个文件内匹配并全部替换
:%s/old/new/gc，g后面加c代表需确认
# 1.5   Execute an External Command
:!<command>
:w filename
v选择后，:w filename，将选择的文本保存至文件
:r filename，插入文件内的文本到当前光标处
# 1.6   The Open Command
o,O,e,a,R
y,p
:set ic，忽略大小写，ignore case
:set is，没搞懂
:set noic，不忽略大小写
:nohlsearch
# 1.7   Getting Help
<F1>
:help
:help <command>
:set nocp
...看不懂后面，不过够了
