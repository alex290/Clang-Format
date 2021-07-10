# ������������� clang-format � QtCreator

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/linux-code-2-e1620113254838.png)


### ������������� clang-format � QtCreator ��� �������������� ����� ���� � ������� C ++

����� ������ �� ������ ������ - ���, ��������, ������ clang. ���� ������������� ����������� ����������� � ���, ��� ��� ������������ (����� ����) ����� ���� ����� ������������ � ����������� ����. ���, ��� ���������, - ��� ���� � ������� .clang (��� _clang-format), ���������� ������������. ���� ������ ������������ ������� .clang, ������� ����� ������ ������������� ����� Qt (��������� Qt ����� ������������ ��� � ������������ ������� � �������), ����� ����� �����:  http://code.qt.io/cgit/qt/qt5.git/tree/_clang-format . ������ IDE � ��������� ������������ ���� ����������. QtCreator ����. ��� ��� ����� / ���� ���������� ������� ����� ��������������� ����� �����������. � ��� ������� ����������� � ���, ��� ��������� QtCreator ��� ������������� clang-�������:

������� ��� ����� ���������� clang-format. ��� Windows �� ������� � ����� clang  http://releases.llvm.org/download.html . � ������������ Linux ������ ��� �������� ������. ������������ MacOS �����, ��������, ������������ brew ��� ��� ���������.

����� ���������� ������� ���� ������� .clang � �������� �������� ������ �������. ��������� ������������ ����� ����� �����:  https://clang.llvm.org/docs/ClangFormatStyleOptions.html . ���������� ���� (����� ���������) ���������� ��� �������� ������������ �� ������ ������������� ����  https://github.com/johnmcfarlane/unformat .

� QtCreator ������������ ������ beautifier ������ ���� ������� � �������� -> � ��������� 

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_plugins.png)

� ���������� QtCreator ������ beautifier ������ ������������ clang-format. � ��� ������� �������� �������������� �������������� ��� ���������� (������������ �������������).

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_beautifier.png)

����� ��������� clang-format ��� ������������� ����� ������������. � ��� ������������� ������� ���� � ������������ ����� ������� clang. 

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_clang-format.png)

��� ������� �� ������ ��������������� ��� ������� � ������� ��������� ������. ������� ���������� ���������� �����.

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_shortcut.png)

� �������� ����� ��������� ����� ������������ ������� [����](https://raw.githubusercontent.com/PickNikRobotics/roscpp_code_format/master/.clang-format "����")