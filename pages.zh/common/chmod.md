# chmod

> 修改文件或目录的访问权限。
> 更多信息：<https://www.gnu.org/software/coreutils/manual/html_node/chmod-invocation.html>.

- 授予所有者［u］执行［x］文件的权限：

`chmod u+x {{文件}}`

- 授予所有者［u］读［r］和写［w］文件或目录的权限：

`chmod u+rw {{文件或目录}}`

- 移除用户组［g］的文件执行［x］权限：

`chmod g-x {{文件}}`

- 授予所有用户［a］读［r］以及执行［x］文件的权限：

`chmod a+rx {{文件}}`

- 授予其他用户［o］（不在所有者用户组）和用户组［g］同样的权限：

`chmod o=g {{文件}}`

- 移除其他用户［o］的所有权限：

`chmod o= {{文件}}`

- 递归授予用户组［g］和其他用户［o］目录下所有文件和子目录的写［w］权限：

`chmod {{[-R|--recursive]}} g+w,o+w {{目录}}`

- 递归授予所有用户［a］目录下文件的读［r］权限和子目录的执行［X］权限：

`chmod {{[-R|--recursive]}} a+rX {{目录}}`
