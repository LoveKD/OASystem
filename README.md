#OAϵͳ���
##**What is OA?**
�ٷ�һ���˵����OA��Office Automation����д������Ϊ���ü������ֶ���߰칫��Ч�ʣ�����ʵ�ְ칫���Զ�������ʵ����Ϣ������ֽ���칫���ɷ��������ͳ�Ʊ���ȡ�
˵���ˣ�������߰칫Ч�ʵ�һ�����ϵͳ��

��Ŀ����ٵ�ʱ�򣬸��Ŵ��ǲ��͵���Ƶ���ģ��Լ��ֶ��������һ�顣����˵���Լ�����Ŀ���������ã��������Ƶ���ջ��˺ܶࡣ��֮ǰѧ���������ܵ�֪ʶ��ϵͳ�����ϵ���һ����ʵ���е������á�[��Ƶ�����ص�ַ](http://down.51cto.com/zt/5298)

##**How to Run this project?**

##**1.��������**

| ģ��| ���� |
| ------------- |:-------------:| -----:|
| ��֯���û����� | ��λ���� |  |
| | ���Ź��� |  |
| | �û����� |  |
| ϵͳȨ�� | ��ʼ��Ȩ��| |
| | ����Ȩ��|  |
| | ��֤Ȩ��|  |
| ���Ͻ���--��̳ | ������ | |
| | ����������������|  |
| | ���¹���|  |
| ������ת���������� | ��ģ����� | |
| | �������̹���|  |
| | ������ת|  |
| | ����ѯ|  |



##**2.�������**

* ��ʾ�㣺JSP��Struts2
* ҵ���߼��㣺Spring2.5
* ���ݷ��ʲ㣺Hibernate3.6

##**3.�������߼��漰����**

###һ����������
* Windows7
* MyEclipse8.5
* Mysql5.5
* Tomcat6.0
* JDK7.0
* Chrome

###�����漰����
* Struts2
* Hibernate
* Spring
* jbpm
* junit
* Jquery

##**4.���ݿ����**

###һ���������ݿ�

` create database oa charset utf8; ` 

###����ERͼ

![des](12.png)


###�������ݱ���

| ����| �ֶ��� | �ֶκ��� |
| ------------- |:-------------:| -----:|
| **itcast_user**| loginName |��¼��  |
| | password |����  |
| | name |��ʵ����  |
|  | gender|�Ա� |
| | phoneNumber| �绰���� |
| | email| �����ʼ� |
| | description |˵�� |
| | departmentId|���ź�  |
|**itcast_role** | name|��ɫ����  |
| |description |��ɫ���� |
| **itcast_privilege**|name |Ȩ������  |
| |url |����  |
| | parentId|��Ȩ��ID  |
| **itcast_department**|name |��������  |
| | description|ְ������  |
| |parentId|��������ID|
|**itcast_forum**|name|�������|
||description|�������|
||position|���λ��|
||topicCount|������|
||articleCount|������|
||lastTopicId|���һ�η��������ID|
|**itcast_topic**|title|��������|
||content|����|
||faceIcon|ͼ��|
||postTime|����ʱ��|
||ipAddr|�����ߵ�IP��ַ|
||authorId|����ID|
||type|�������ͣ���������ͨ���ö���|
||replyCount|�ظ���|
||lastUpdateTime|���һ�θ���ʱ��|
||forumId|�������ID|
||lastReplyId|���һ�λظ���ID|
|**itcast_reply**|title|����(ͬTopic���̳�Article)|
||content|����|
||faceIcon|ͼ��|
||postTime|����ʱ��|
||ipAddr|�ظ��ߵ�IP��ַ|
||authorId|�ظ��ߵ�ID|
||topicId|���������ID|


##**5.����������**

###1�����BaseDao
	һ����6������
	
```
	void save(T entity);//��
	
	void delete(Long id);
	
	void update(T entity);
	
	T getById(Long id);//��
	
	List<T> findAll();
	
	List<T> getByIds(Long []ids);
```

###2�����BaseDaoʵ����

>ʵ������6������
���BaseDaoImplʵ��
	��ȡT����ʵ���ͣ�
	ʹ�÷���ķ���

	
```
	ParameterizedType pt=this.getClass().getGenericSuperClass();
	clazz=(Class<T>)pt.getActualTypeArguments()[0];
```

##������ѧϰ

QQ:188273928
CSDN Blog:http://blog.csdn.net/wisewolf_life
Email:wy_lumia@outlook.com
**��ӭ����ѧϰ^.^**

