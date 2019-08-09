# Django-Auth
使用Django自带的Auth模块的User模型，实现用户注册与登录

利用Django 2.0开发一个叫users的app，来实现以下6项功能：

用户注册: 注册完成后转到登录页面 
用户登录: 登录完成后转到用户资料页面
用户资料页面: 查看用户注册信息，并提供编辑资料按钮
用户资料编辑：编辑完成后转到用户资料查看页面
用户密码重置
用户退出登陆

由于Django Auth自带的User模型字段有限，还需要自定义模型UserProfile对其扩展。

Django Auth模块自带User模型所包含字段：
username：用户名
email: 电子邮件
password：密码
first_name：名
last_name：姓
is_active: 是否为活跃用户。默认是True
is_staff: 是否为员工。默认是False
is_superuser: 是否为管理员。默认是False
date_joined: 加入日期。系统自动生成。

自定义的UserProfile模型:

user: 与User是1对1关系
org：用户名
telephone: 电话
mod_date: 最后修改日期。系统自动生成

注：前端页面有待完善。
