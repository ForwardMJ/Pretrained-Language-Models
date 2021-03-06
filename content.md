**1.Github表格及其内容居中(离线):**

1. 在Typora中先创建好表格(Ctrl+T)，然后点击`编辑`-->`复制为HTML代码`后再将其粘贴至Noteppd++，安装Tydy2插件后对其进行格式化;
2. 从格式化后的内容中直接删除`<head>...</head>`、将`<th>`和`<td>`中的`style='text-align:center;'`全部替换(Ctrl+F)为`align="center"`;
3. 在`<table>`中添加`align="center"`以保证表格整体居中，若需要为其添加标题，在`<table>`上添加`<p align="center">title</p>`即可;

**2.Markdown表格内嵌列表:** 在Typora中的表格编辑时，在每一个分项前面加上`<li>`即可产生无序列表，此处尽量向左对齐，接着步骤同上;
<html>
    <body>
        <figure>
            <table align="center">
                <thead>
                    <tr>
                        <th style='text-align:left;'>候选者</th>
                        <th align="center">框架</th>
                        <th style='text-align:left;'>优点</th>
                        <th align="center">缺点</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td style='text-align:left;'>
                            <a href='https://github.com/PyUnit/pyunit-address'>Pyunit-Address</a>
                        </td>
                        <td align="center">Paddle</td>
                        <td style='text-align:left;'>
                            <ul>
                                <li>支持规则地址的自动补全和纠错</li>
                                <li>默认使用全国五级地址库，统计时间为2019年</li>
                                <li>对于非规则地址，提供了DL模型(Transformer)；</li>
                            </ul>
                        </td>
                        <td align="center">实用性较高</td>
                    </tr>
                </tbody>
            </table>
        </figure>
    </body>
</html>

**3.Markdown表格合并:** 表头和表体不能直接进行合并;
<html>
    <body>
        <figure>
            <table align="center">
                <thead>
                    <tr>
                        <th align="center">西门庆</th>
                        <th align="center">潘金莲</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td colspan="2" align="center">武大郎</td>
                    </tr>
                </tbody>
            </table>
        </figure>
    </body>
</html>

<html>
    <body>
        <figure>
            <table align="center">
                <tbody>
                    <tr>
                        <td rowspan="2">武大郎</td>
                        <td align="center">潘金莲</td>
                    </tr>
                    <tr>
                        <td align="center">西门庆</td>
                    </tr>
                </tbody>
            </table>
        </figure>
    </body>
</html>

**4.No module named 'tensorflow.contrib'**: 
- [Tensorflow不降级安装](https://blog.csdn.net/Rex__404/article/details/112798943)
- [Tensorflow降低安装](https://blog.csdn.net/qq_40900585/article/details/105382992)
