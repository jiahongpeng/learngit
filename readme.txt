$ mkdir learngit
$ cd learngit    //������Ŀ¼
$ pwd//�����汾��ĵ�ַ

$ git init//�����Ŀ¼��ɿ��Թ���Ĳֿ�

$ git add readme.txt //���ļ���ӵ��ֿ�

addֻ��addһ���ļ���commit���ϴ��ö��ļ������Կ���add�ö࣬Ȼ����һ��commit
$ git commit -m"wrote a readme file"  //�ļ��ύ���ֿ�

$ git status    //��ǰ���״̬����û��û���ϴ����ļ�    modified�Ǳ䶯���ļ�

$ git diff   //�鿴difference����ʱ��س���֮������++++end�����q�˳���¼

$ git all//��ʾ�԰汾������в���



$ commit��ʱ�����������ͼ1�Ĵ�����ɾ��git�ļ��������index.log�ļ�


git add -A   // ������иĶ�

git add *     // ����½��ļ����޸ģ����ǲ�����ɾ��

git add .    // ����½��ļ����޸ģ����ǲ�����ɾ��

git add -u   // ����޸ĺ�ɾ�������ǲ������½��ļ�



�� commit ǰ���� add:

git reset <file> // �����ύ�����ļ�

git reset        // unstage all due changes


add/commit ǰ�������ļ����޸�:

git checkout -- README.md  // ע��, add��Ӻ�(ͬcommit�ύ��)���޷�ͨ�����ַ�ʽ�����޸�



�汾����

head ��ʾ��ǰ�汾��Ҳ�������µģ���һ���汾����head^,���ϸ��汾����head^^, 
ǰ100���汾����head~100

$ git reset --hard HEAD^  //���˵��ϸ��汾     �����add�ϣ�����û��commit�Ļ������������
��������HEADָ���ĸ��汾�ţ���Ͱѵ�ǰ�汾��λ���ġ�

cd ../   //�ص���һ��

$ cat readme.txt   //�鿴�ļ�����

$ git reflog //��¼ÿһ�������commit id

$ git reset --hard commitid//ָ���ص�ĳ���汾


���������ݴ���

�ڵ����ܿ�����Ŀ¼������˵learngit

�汾�� 

��һ�����ص�Ŀ¼ .git,����ǰ汾��

�汾������Ҫ���ǳ�Ϊstage ���ݴ���������git �Զ������ĵ�һ����֧master��
�Լ�ָ��master��һ��ָ���HEAD����ͼ1

�ļ���git�汾����ӵ�ʱ�򣬷�������

��һ������git add ���ļ���ӽ�ȥ��ʵ���Ͼ��ǰ��ļ��޸���ӵ���������
�ڶ�������git commit �ύ���ģ�ʵ���Ͼ��ǰѻ����������������ύ����ǰ��֧��

git commit������master��֧���ύ���ġ�

��Ҫ�ύ���ļ��޸�ͨͨ�ŵ��ݴ�����Ȼ��һ�����ύ�ݴ����������޸�


$ git diff HEAD -- readme.txt  //���Բ鿴�������Ͱ汾���������°汾������


$ rm test.txt  //ɾ���ļ����������ļ�

1.ɾ���汾���е��ļ�
$ git rm test.txt   
$ git commit -m "fdfd"
2.ɾ���ˣ���Ϊ�汾���ﻹ���أ����Կ��Ժ����ɵذ���ɾ���ļ��ָ������°汾��
$ git checkout -- test.txt
3.����汾��û���ˣ��볷�أ�ֻ�ܻ��˵���һ���汾��
$ git reset --hard HEAD^


git checkout -- readme.txt��˼���ǣ���readme.txt�ļ��ڹ��������޸�ȫ������
�����е� -- ����Ҫ��û��--���ͱ���ˡ��л�����һ����֧�������













