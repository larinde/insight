test broker ofered by mosquito

mqtt://test.mosquitto.org


npm install -g @asyncapi/generator

ag --version


npm install -g @asyncapi/nodejs-template

ag ./orders-asyncapi.yaml  @asyncapi/nodejs-template -p server=development -o producer-node


ag ./orders-asyncapi.yaml  @asyncapi/java-spring-template  -p server=development -o producer-java


## Generate Spring Java code

npm install -g @asyncapi/java-spring-template

ag ./orders-asyncapi.yaml  @asyncapi/java-spring-template  -p javaPackage=com.demo.orders asyncapiFileDir=src/main/resources/api -o producer-java

npm install -g @asyncapi/java-spring-cloud-stream-template 

ag ./orders-asyncapi.yaml @asyncapi/java-spring-cloud-stream-template   -p javaPackage=com.demo.orders asyncapiFileDir=src/main/resources/api -o producer-cloud

@asyncapi/java-spring-cloud-stream-template



## Generate HTML Doc

npm install -g @asyncapi/html-template

ag ./orders-asyncapi.yaml  @asyncapi/html-template   -o doc/html

ag ./orders-asyncapi.yaml  @asyncapi/html-template  -o doc --force-write

## Generate Markdown Doc

npm install -g @asyncapi/markdown-template

ag ./orders-asyncapi.yaml  @asyncapi/markdown-template -o doc/markdown

ag ./orders-asyncapi.yaml  @asyncapi/markdown-template -o doc --force-write
