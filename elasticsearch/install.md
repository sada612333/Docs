1. 下载  
https://www.elastic.co/cn/downloads/elasticsearch

2. 启动   
>单机启动`>bin/elasticseach` 

>浏览器查看是否启动成功`127.0.0.1:9200`
   
>查看已安装的插件`>bin/elasticseach-plugin list`

>安装插件`>bin/elasticsearch-plugin install analysis-icu`(分词插件)

>浏览器查看插件`127.0.0.1:9200/_cat/plugins`

>集群启动

`bin/elasticsearch -E node.name=node1 -E cluster.name=geektime -E path.data=node1_data -d` 
`bin/elasticsearch -E node.name=node2 -E cluster.name=geektime -E path.data=node2_data -d `
`bin/elasticsearch -E node.name=node3 -E cluster.name=geektime -E path.data=node3_data -d `

>浏览器查看节点`127.0.0.1:9200/_cat/nodes`

