This is simple workoround for java.lang.NoClassDefFoundError: sun/reflect/Reflection .<br>

Usually occurs after upgrading to Java 11 Tomcat 9.<br>

Just put this Reflection.class file in WEB-INF/classes/sun/reflection directory. <br>

org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.security.apacheDirectoryServerContainer': Invocation of init method failed; nested exception is **java.lang.NoClassDefFoundError: sun/reflect/Reflection**
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.initializeBean(AbstractAutowireCapableBeanFactory.java:1514)
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:521)
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:458)
	at org.springframework.beans.factory.support.AbstractBeanFactory$1.getObject(AbstractBeanFactory.java:293)

