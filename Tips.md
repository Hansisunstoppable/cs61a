### Tips

```
--local # 用于本地测试，所有命令都需要加上！否则会卡在填写学校邮箱界面
```

```python
# run all doctests in a file
py -m doctest <python_source_file> -v   
```

```python
# Doctests
>>> def sum_naturals(n):
        """Return the sum of the first n natural numbers.

        >>> sum_naturals(10)
        55
        >>> sum_naturals(100)
        5050
        """
        total, k = 0, 1
        while k <= n:
            total, k = total + k, k + 1
        return total
# Doctests调试方法
>>> from doctest import run_docstring_examples
>>> run_docstring_examples(func, globals(), True)
```

