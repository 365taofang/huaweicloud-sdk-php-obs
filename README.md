Version 3.22.601

新特性： 基于华为Version 3.22.6，增加ObsImageClient。 

使用方法
````
$obs = new Obs\ObsImageClient([
    'key' => '*** Provide your Access Key ***',
    'secret' => '*** Provide your Secret Key ***',
    'endpoint' => 'https://your-endpoint',
    'custom_domain' => 'img.house365.com',//非必填。需要替换的域名
    'project_name'=>'comment_sysytem',//必填。文件路径1级目录
    'project_sub_name'=>'asdasdd',//非必填。文件路径2级目录
]);

$resp = $obs->putObject([
    'Bucket' => 'bucketname',
    'Key' => 'objectname',//必填。文件名称，如：123.jpg
    'Body' => '********',
]);
````
----
Version 3.22.6

新特性：

资料&demo:

修复问题：
1. 修复三方依赖冲突的问题；

----

Version 3.19.9

新特性：

资料&demo:

修复问题：
1. 修复OBS请求时，Host偶尔被异常替换的问题；
2. 修复特殊场景下，日志模块无法正常工作的问题；
3. 修复header中的正常特殊字符被url编码的问题；

-------------------------------------------------------------------------------------------------

Version 3.1.3
新特性：

资料&demo:

修复问题：
1. 修复连接OBS服务超时时，解析request-id报错导致异常信息被截断的问题；

