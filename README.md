# NovelSpidersSimple
其实就是为了用iRead听小说，自己弄了一个小说的爬虫,使用这个脚本需要稍微知道一点html结构和node命令就行;

## 初次运行
如果是初次运行，请先执行npm install 根据package.json安装依赖;

## 正式运行

打开工程根目录book.config.js文件，这个文件是用来设置爬小说的源数据;
const book = {
    'url': 'http://www.wutuxs.com/html/4/4041/',//这是小说的目录页
    'href': 'http://www.wutuxs.com',//这是小说的目录页
    'name': '修真聊天群',//设定保存的书名
    'listDom': '#at tr td a',//小说列表的内容html结构
    'artTitle': '#amain dd h1',//每一篇的标题html结构
    'artContent': '#contents'//每一篇的内容html结构
};
在工程根目录打开控制端命令界面
执行npm run list，获取小说目录
执行npm run art，获取小说每一篇文章内容
然后等着就好了
