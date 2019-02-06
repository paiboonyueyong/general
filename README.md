��͹�����Ҩ�价Ӥ������ѡ�Ѻ JWT ����ҷӤ������ѡ�Ѻ 2 �ӹ���͹��Ѻ
Stateful
Sateless

Stateful ���¶֧ ��è���ʶҹ� (state)
Stateless  ���¶֧ �����訴��ʶҹ� (state)

�ѭ��

        HTTP (HyperText Transfer Protocol) �� Protocol �����㹡��������� / �Ѻ�觢����ŷҧ��ҹ Web Application ��÷ӧҹ�ͧ HTTP ���繡�����ҧ������ Request ��ѧ Web Server ������ͧ�� Resources 
����� Web Server ���Ѻ Request  ��зӡ�õ�Ǩ�ͺ�Է������ Request ������Է�����Ҷ֧ Resource �ѧ������������ �ҡ���Է��� Web Server ��ШѴ��� Resource �������� Request �����ͧ���� 

        HTTP �� Protocol �������ա�è���ʶҹС�÷ӧҹ  �ء���駷�� Request � ���繡�����ҧ Request ���������  ������ա�èѴ�� / ���Ӣ������� ����� Web Server  �ء Request ������ �ж١ Web Server ��Ǩ�ͺ�Է�������ء����  ������¡��÷ӧҹ�ͧ HTTP ����繡�÷ӧҹẺ Stateless   

        �ҡ�ѭ�Ҵѧ�����  �Ҩ֧��Դ���Ըա�÷������ Web Server ����ö����ʶҹС�÷ӧҹ  ����ʶҹТͧ Client ���������繵�ͧ��Ǩ�ͺ�Է�������ء����  �Ըա�÷����������¡��� Session 

        Session ���Ըա�÷�� Web Server ������Ѻ����ʶҹС�÷ӧҹ / �кص�ǵ��ͧ Client
����� Client �ӡ�� Log in �������к� Web Server �����ҧ���ʪش�֧����� ���¡��� Session Id  ���Ƿӡ���� Session Id ��Ѻ仾�����Ѻ Request �ͧ Client 

        Client ���� Session Id �����ٻẺ������¡��� Cookies  ������ա���� HTTP Request ��ѧ Web Server �ա����  Client �е�ͧ�� Session Id ��Ѻ���� Web Server ����  ���ͺ͡�Ѻ Web Server ��� ���� Log in �������к�����  (���� Session Id �ѧ�����) ��������ͧ��Ǩ�ͺ�Է��������ա����  ������¡��÷ӧҹẺ������ Stateful

        �Ѩ�غѹ  ��  Application ���ӧҹ��駷����Ẻ Stateful ��� Stateless
Stateful ��� Application ����� Session
Stateless ��� Application �������� Session  ��������ҧ���᷹  ������¡��� Token



Token

        �����ʪش�֧��������᷹ Session Id �������кص�ǵ��ͧ Client  ��� Client �������
������ٻẺ��µ��  ����������Ըշ�������  �շ�駷���� Standard ��кҧ����Դ�Ըա�����ҧ Token �������ҹ�ͧ  ������Ѻ���������  ����� Standard Token ����ժ������ JWT (Json Web Token) ������ Json data �ͧ����������ҧ������ (Token)



��ʹբ������ �ͧ Stateful ��� Stateless

Stateful
    
��ʹ� 
����  �дǡ ��������ö����ʶҹТͧ Client ��  �·���������ͧ��Ǩ�ͺ�Է�������ء����
����  ��������ͧ��Ǩ�ͺ�Է���  ����ѧ����ö�红��������� �ͧ Client ��麹 Memory ��  �·���������ͧ query �����Ũҡ Database ����ء����
�������
�������СѺ�к�����ͧ��â��¢�Ҵ (scale) �͹Ҥ�  ���� Session �������੾������ Cluster ���� ��ҹ�� �������ö������Ѻ�к������   ��� Session Id ���բ�Ҵ������ǨӡѴ ������¤������ �ͧ�Ѻ Client ��ӹǹ�ӡѴ
������ͧ Memory ���������������¹����� ����  �Ҩ�� Session ���㹡���红�����
�������СѺ�����ҹ�����Ѻ Native Mobile  ���� Native Mobile ����� browser �֧����������СѺ��÷ӧҹ�����Ѻ Cookies
�����¹������դ�����ӫ�͹  ��� Service ����� 㹡óշ����������շ�� Web App ��� Mobile App ��������������ö�¡ Front end (html, css, js) �������ǹ�ʴ��� �͡�ҡ Back end (java, php, node.js, asp) ����� Business Logic ��  
����ͧ Session Expire ���� Session ������� �����Ҩе�ͧ�ӡ�� Log in ����ء���� 
���

Stateless

��ʹ�
�����ͧ�ͧ��â����к�  �����ѹ����ͧ�� Session  ������������ͧ�� Cluster  ������ö���к� HA (High Ability System) ��  �֧������ Server ����ͧ�����ͧ˹�觨� down �������������� Cluster ���ǡѹ  ��ҡ�����ö��ҹ Application �����������  ������ͧ Log in ����
����ö��¹ Front end ��� Back end �¡�͡�ҡ�ѹ��
����Ѻ Application �ء�ٻẺ�����Ҩ��� Web Desktop Mobile ������������ Session
���
�������
��ͧ��Ǩ�ͺ�Է���ء����  �����ӧҹ��ҡ���Ẻ Stateful
��¹����� + �ҧ�к�����ҡ����