# Pure JAVA @ Android
> �ϥ� Android Studio�@��IDE �}�o ��Java 

# AS�}�@�ӷs�M���[��@�U!
![N|Solid](http://i.imgur.com/Fubooy7.jpg)

# �T�{�}�n�F
![N|Solid](http://i.imgur.com/pt3O0vN.jpg)

# ������Project�Ҧ�
```sh
 �ݬ�Android app �bAndroid Studio ������Ƥ��G�榡
```
![N|Solid](http://i.imgur.com/IYGyiVh.jpg)

# ��Ƥ��G�榡
```sh
 �D�n�Osrc���]main�A�]java�M��~�Opackagename
```
![N|Solid](http://i.imgur.com/p03wK9i.jpg)

# �إߤ@�ӷs�M��
```sh
 ��y�}�l--����Java�Ϊ�
```
![N|Solid](http://i.imgur.com/wgBO3qd.jpg)

# �T�{�ئn�F����������
![N|Solid](http://i.imgur.com/OvllIPc.jpg)

# ��F�o���ɮ׻P��Ƨ�

```sh
app build  settings.gradle
```
![N|Solid](http://i.imgur.com/uv5xgoU.jpg)

# �إ�src���]main�A�]java�A�]packagename
```sh
���i���� �����qapp�̭����ԥX�Ӥ]�i�H
```
![N|Solid](http://i.imgur.com/kv7q12O.jpg)
![N|Solid](http://i.imgur.com/u6wFpYK.jpg)

# �ץ�build.gradle���e
```sh
�i�H�βĤT��n�骽���}�ҽs��ץ�
```
![N|Solid](http://i.imgur.com/nqNe87v.jpg)
```sh
�o�O�ϥ�AS�}�ҫ�ץ�
```

![N|Solid](http://i.imgur.com/XYSpiHW.jpg)
```sh
apply plugin: 'java'
version = '1.0'
sourceCompatibility = 1.8
targetCompatibility = 1.8

mainClassName = 'idv.neo.TCPServer'
jar {
    manifest {
        attributes 'Implementation-Title': 'TCPServer Examples', 'Implementation-Version': version,
                'Main-Class': mainClassName
    }
}

run {
    standardInput = System.in
}

repositories {
    mavenCentral()
    jcenter()
}

dependencies {
    compile fileTree(dir: 'libs', include: ['*.jar'])
}
```
![N|Solid](http://i.imgur.com/KhLSkNu.jpg)

# ���s�R�WClass name��FirstJava
```sh
�]���O���i������app����
```
![N|Solid](http://i.imgur.com/lhlRJl0.jpg)
![N|Solid](http://i.imgur.com/PQ5WfGb.jpg)

# �bFirstJava���ɤW���T���d��code
![N|Solid](http://i.imgur.com/2DEh5Fp.jpg)

# �ץ��ýs��Run�պA�]�w��1
```sh
�[�JJava����W�䴩
```
![N|Solid](http://i.imgur.com/dKE9f70.jpg)

# �ץ��ýs��Run�պA�]�w��2 : ��Fapp
```sh
����Android �����պA
```
![N|Solid](http://i.imgur.com/hgV0E4M.jpg)

# �ץ��ýs��Run�պA�]�w��3 : �[�WJava�պA
```sh
�[�WJava�պA
```
![N|Solid](http://i.imgur.com/4uexG1c.jpg)

# �ץ��ýs��Run�պA�]�w��4 : ����packagename�W��
```sh
��JMain Class ������packagename�W�� 
```
![N|Solid](http://i.imgur.com/HUGsFZq.jpg)
# �s��Run�պA�]�w��4 : Use classpath of module
```sh
�O�o��J Use classpath of module (�o�O�n���w��)
```
![N|Solid](http://i.imgur.com/2jIy4YC.jpg)

# �ϥγ]�w�ɹ��հ���ݬ� 
![N|Solid](http://i.imgur.com/J9jIK4W.jpg)
![N|Solid](http://i.imgur.com/wWM3whY.jpg)

# �i���s��Run�պA�]�w��  : �䴩��Xjar
![N|Solid](http://i.imgur.com/lQYaYHB.jpg)
![N|Solid](http://i.imgur.com/dNrqde6.jpg)
![N|Solid](http://i.imgur.com/6e1Qz10.jpg)
![N|Solid](http://i.imgur.com/cwg3RDs.jpg)
![N|Solid](http://i.imgur.com/YJFwLOl.jpg)
![N|Solid](http://i.imgur.com/O3Jj3Ae.jpg)


# �ثe���Fclasses����X�~�S����L��Ƨ����ɮ� 
![N|Solid](http://i.imgur.com/FQWFiCQ.jpg)
# �ϥγ]�w�ɦA����ݬ� 
![N|Solid](http://i.imgur.com/BHcTxy0.jpg)
# ���浲�G �h�X�F��Ƨ���jar
![N|Solid](http://i.imgur.com/rrUVPbz.jpg)
# jar�ɰ��浲�G 
![N|Solid](http://i.imgur.com/i0ffW94.jpg)
