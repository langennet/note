

设置代理
alias proxy='export all_proxy=socks5://127.0.0.1:1086'
alias unproxy='unset all_proxy'
查询IP属性
alias get_ip='curl cip.cc'

PATH="/Library/Frameworks/Python.framework/Versions/3.8/bin:${PATH}"
PATH=/usr/local/Cellar/python/3.6.5/bin:${PATH} 
alias burpsuite2.1="java -Dfile.encoding=utf-8 -javaagent:/Users/jing/tools/BurpSuite2.1/BurpSuiteCn.jar -Xmx1024m -noverify -Xbootclasspath/p:/Users/jing/tools/BurpSuite2.1/burp-loader-keygen-2.jar -jar /Users/jing/tools/BurpSuite2.1/burpsuite_pro_v2.1.jar &"



macos安装openjdk11
brew search openjdk
brew intall adoptopenjdk11

设置macos的Java的版本和版本切换
subl .bash_profile

设置java版本切换

# openjdk8 
JAVA_HOME_8=/Library/Java/JavaVirtualMachines/openjdk-8.jdk/Contents/Home

# openjdk 11
JAVA_HOME_11=/Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home

export JAVA_HOME=$JAVA_HOME_8
#export JAVA_HOME=$JAVA_HOME_11



这样设置默认是openjdk8
如果要切换的时候，删除java11前面的#，在java8前面加#
然后执行  . .bash_profile


或者如下：

# openjdk8 
java8=/Library/Java/JavaVirtualMachines/openjdk-8.jdk/Contents/Home

# openjdk 11
java11=/Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home

export JAVA_HOME=$java8
alias java8="export JAVA_HOME=$java8"
alias java11="export JAVA_HOME=$java11"
