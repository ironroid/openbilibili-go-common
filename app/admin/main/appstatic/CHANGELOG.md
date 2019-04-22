### appstatic-admin

### v1.1.3
1. 新增逻辑：二次触发时，同时向redis中存入需要推送的resID

### v1.1.2
1. 分割出appstatic-admin中的定时任务至appstatic-job中
2. 增加ut
3. 修复正在计算中的增量包会重复计算的问题

### v1.1.1
1. 支持config中的仅wifi的条件
2. 增加UT，修复saga问题

### v1.1.0
1. 新增资源包时验证mod添加not deleted和valid条件

### v1.0.9
1. 调整参数验证逻辑，如大小范围允许一端为空

### v1.0.8
1. 支持更多增量包，10个
2. 支持二次触发（提供接口，由mgr后台告知需要二次触发）
3. 增加添加资源后的返回值（版本+资源ID）

### v1.0.7
1. 添加限制，job在非正式环境不运行

### v1.0.6
1. 支持更多参数,level, sysver, scale
2. 使用框架的client进行文件下载，设置timeout

### v1.0.5
1. 修改上传后重命名的文件名格式
2. 修改增量包的文件名格式

### v1.0.4
1. 取值检验使用bm Bind方法，简化写法，更清真
2. 新增适配测试权限点的上传接口
3. 新增从接口指定default_package的逻辑
4. 文件类型校验改为读取配置，如果配置为空则放开所有文件类型上传

### v1.0.3
1. 增加测试包和正式包的判断逻辑，计算差量包时，算出三个正式包的差量+三个测试包的差量

### v1.0.2
1. 新增加一层 department

### v1.0.1
1. 修改差量包计算逻辑：立即计算新上传，失败后每小时重试
2. 增加mod_name和file_name的正则检验

### v1.0.0
1. 支持从manager上传zip包创建新版本
2. 支持从第三方系统上传zip包创建新版本
