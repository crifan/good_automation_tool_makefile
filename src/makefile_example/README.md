# Makefile实例

下面列举一些自己用到过的`Makefile`去提高工作效率的实际的例子：

## `Makefile`中调用`Python`文件

[【已解决】Makefile中运行Python脚本文件](http://www.crifan.com/makefile_run_python_script_file)

## `Makefile`中实现自定义函数

[【已解决】Makefile中实现自己的函数并调用](http://www.crifan.com/makefile_implement_custom_function_then_call)

> #### Caution:: 自定义函数的一些注意事项
> * 自定义函数内部的内置函数需要加上`eval`才能正常运行
>   * 详见：[【已解决】Makefile中define的自定义函数中的lastword不工作](http://www.crifan.com/makefile_define_custom_function_lastword_not_work)
> * 自定义函数开头不能是`# xxx`的注释，否则语法出错而无法运行
>   * 详见：[【已解决】Makefile自定义函数调用出错：unterminated call to function `notdir': missing `)'.  Stop](http://www.crifan.com/makefile_custom_function_call_error_unterminated_call_to_function_notdir_missing_stop)
> * 自定义函数中打印变量，echo无效，需要用info
>   * 详见：[【已解决】Makefile中define自定义函数中打印输出没效果](http://www.crifan.com/makefile_define_custom_function_print_no_output_effect)
> * 自定义函数如何获取返回值
>   * 详见：[【已解决】Makefile中如何获得define自定义函数的返回值](http://www.crifan.com/makefile_get_define_custom_function_return_value)

## 提取出`gitbook`中公共部分的`Makefile`

详见：[【已解决】提取Gitbook中Makefile公共部分](http://www.crifan.com/gitbook_extract_common_part_of_makefile)
