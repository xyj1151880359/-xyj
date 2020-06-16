git init
git add *
git commit -m''
// 配置本机与github 链接 用 ssh密钥
// 第一步：生成密钥 ssh-keygen -t rsa -C '1151880359@qq.com'
// 创建密钥文件：将生成的密钥写入到文件中

// 第二步：查看密钥 cat ~/.ssh/id_rsa.pub
- xxx.pub 文件表示的是【密钥文件】

// 第三步：来到github [new ssh] 将ssh密钥复制进去；建立电脑与github 链接

如何将本地仓库 添加到 远程仓库
- 第一步：创建一个远程仓库  创建一个本地仓库(有忽略)
- 第二步：建立本地仓库与远程仓库链接
   git remote add origin git@github.com:xyj1151880359/-xyj.git
   语法总结 git remote add origin 远程仓库地址
- 第三步：将本地仓库添加到远程仓库 git push -u origin master
  - git push 添加
  - -u 表示谁添加的
  - origin 表示组织
  - master 主支


如果说更改需要添加到远程
git add------> git commit ----> git push

注意：只有第一次 才需要建立 电脑与github 链接
      只有是一个新的仓库 才需要建立 本地仓库与远程仓库的链接

方式二：直接用github 工具直接上传


### github 使用
1：创建远程仓库； （生成README.md）
2：git clone 将远程仓库下载到本地
3：git add git commit git push

当本地仓库与远程仓库不是一个仓库的时候；本地init仓库，远程新建仓库
1：先建立本地与远程仓库连接
   git remote add origin master '远程仓库地址'

2：将本地推送到远程
   git push -u origin master

注意：尽量不要让远程生成READNE.md文件，在本地创建README.md 然后提交
      如果远程已经创建 推送时候 远程会拒绝
      解决：
      git pull --rebase origin master 将README.md 文件拉到本地

### 如何利用github 学习
  1：知道自己搜索内容是什么 content_problem
  2：查询范围  name description README
  3：提交 starts forks 数量越高代码越好 时间越近越好 stars:>num  forks:>num
  4：语言范围 开源代码中有所有语言 language:javascript
  5：更新时间越近越好  pushed:>YYYY-MM-DD

  总结：
  1：搜索条件为多个条件，条件与条件之间是且关系；分割方式用【空格】

  2：范围的条件查询
  in:name in:description in:README

  3：stars 与 focks 拆线

  stars:>1000 forks:>100

  4：限制语言的搜索范围
  language:javaScript language:C++

  5：搜索时间为 2018年5月1号之后的
  pushed:2018-05-01

  综上：
  in:name in:desciption vue项目 stars:>1000 forks>1000 pushed:>2018-05-01 language:javaSctipt 其他条件

### github
1：如何使用 github 进行项目管理
2：如何使用 github 自学 找到优秀的开源项目
3：如何使用 github 进行合作开发

