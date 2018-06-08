
web.xml中encoding的值，如果与jsp页面顶端contentType中charset的值不一致，则会造成输入乱码

hibernate.cfg.xml文件中添加C3P0配置，就不会出现hibernate回滚失败的错误

<session-factory>
	<!--C3P0配置 -->
    <property name="hibernate.connection.provider_class">org.hibernate.connection.C3P0ConnectionProvider</property>
    <property name="hibernate.c3p0.max_size">20</property>
    <property name="hibernate.c3p0.min_size">5</property>
    <property name="hibernate.c3p0.timeout">120</property>
    <property name="automaticTestTable">Test</property>
    <property name="hibernate.c3p0.max_statements">100</property>
    <property name="hibernate.c3p0.idle_test_period">120</property>
    <property name="hibernate.c3p0.acquire_increment">1</property>
    <property name="c3p0.testConnectionOnCheckout">true</property>
    <property name="c3p0.idleConnectionTestPeriod">18000</property>
    <property name="c3p0.maxIdleTime">25000</property>
    <property name="c3p0.idle_test_period">120</property>
	<!--C3P0配置 -->	
	
	...
</session-factory>