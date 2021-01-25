# @domain.js/checker
通用模块 checker，用于检测各种情况

[![Build status](https://travis-ci.com/domain-js/checker.svg?branch=master)](https://travis-ci.org/domain-js/checker)
[![codecov](https://codecov.io/gh/domain-js/checker/branch/master/graph/badge.svg)](https://codecov.io/gh/domain-js/checker)

# Installation
<pre>npm i @domain.js/checker --save</pre>

# cnf
专属配置名称 `checker`
<pre>无</pre>

# deps
| 名称 | 描述 |
| ------ | ---- |
| async.someSeries  | 多种权限均可以的时候调用该函数一次判断，直到返回为 true |
| errors.notAllowed | 权限不足的默认错误 |


# Usage
| 功能 | 描述 | 样例 |
| ---- | ---- | ---- |
| equal | 判断两个值是否相等, 相等返回 true, 反之 false | checker.equal(var1, var2) |
| privacy | 多权限判断，会依次判断，直到有符合条件的，全部没有，则抛出异常 | checker.privacy([[fn1, arg1, arg2], [fn2, arg1, arg2]], error) |
