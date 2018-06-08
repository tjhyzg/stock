
web.xml��encoding��ֵ�������jspҳ�涥��contentType��charset��ֵ��һ�£���������������

hibernate.cfg.xml�ļ������C3P0���ã��Ͳ������hibernate�ع�ʧ�ܵĴ���

<session-factory>
	<!--C3P0���� -->
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
	<!--C3P0���� -->	
	
	...
</session-factory>