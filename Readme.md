# ���������� �������� TCP �������

### ��������
���������� ���������� TCP ������� � ������� � ������� ������������ ����������� � �������� �����. ������ ���������� ������� ������ 
* quit - �������� ����������
* add - ���������� ��������� �����, ����� ������ �������� 4 ���������� 2� �����: ����� ���������� � �����, ������� �� ����������
* sq - ������ ������� ����� �� ��������� 2� ����������� ������
� ������ ���������� ��������� 
������������ ������ ���� ��������� ��������

### ������

������� 2 �������
    1) � ������ ��������� `go run proto.go server.go` 
    2) �� ������ `go run proto.go client.go`
���� ���������� ��������� ��������, �� ������ � ��������� ������� ���������� �.2)

### ������
������
```
C:\Users\����\go\src\all>go run proto.go server.go
2018/06/12 22:48:57 resolved TCP address 127.0.0.1:6000
2018/06/12 22:49:50 accepted connection address 127.0.0.1:59305
client 127.0.0.1:59305received command command add
client 127.0.0.1:59305received command command sq
client 127.0.0.1:59305received command command quit
client 127.0.0.1:59305shutting down connection
```

Client

```
C:\Users\����\go\src\all>go run proto.go client.go
command = add                               //�������� ������� ���������� �����
Ox = 1                                      //��������� �����
Oy = 2
x = 3
y = 4
ok                                       //�������� ������������� 
command = sq                            //�������� ������� ��������� �������
result: 25.120000                       //�������� �������� �� �������
command = quit                          //��������� ����������

C:\Users\����\go\src\all>
```