Here we are storing a generic json data in db w/o usinf any third party library, w/o converting data
to any other format like String / text etc.

Here we are using quarkus 3 which supports Hibernate 6 so now we can use below syntax to store Json data -

https://docs.jboss.org/hibernate/orm/6.0/userguide/html_single/Hibernate_User_Guide.html

@JdbcTypeCode( SqlTypes.JSON )
private Map<String, Object> customJson;

So now we can store any kind of json data.