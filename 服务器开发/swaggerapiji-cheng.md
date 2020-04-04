# Swagger API 集成

git地址：[https://github.com/swagger-api](https://github.com/swagger-api)



添加SwaggerConfig

```java
public class SwaggerConfig {

    @Bean
    public Docket createRestApi() {
        return new Docket(DocumentationType.SWAGGER_2)
                .apiInfo(apiInfo())
                .select()
                .apis(RequestHandlerSelectors.basePackage("cn.codingxiaxw.web"))
                // 注意修改此处的包名
                .paths(PathSelectors.any())
                .build();
    }

    private ApiInfo apiInfo() {
        return new ApiInfoBuilder()
                .title("接口列表 v1.1.0") // 任意，请稍微规范点
                .description("接口测试") // 任意，请稍微规范点
                .termsOfServiceUrl("http://你的ip地址/swagger-ui.html")
                // 将“url”换成自己的ip:port
                .contact("dexter") // 无所谓（这里是作者的别称）
                .version("1.1.0")
                .build();
    }
}
```


