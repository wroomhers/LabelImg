.. image:: /readme/images/labelimg.png
        :target: https://github.com/heartexlabs/label-studio

Label Studio modern, çok modlu bir veri işaretleme aracıdır
=======
Burada paylaşılan her şey `HumanSignal'in repository'sinden <https://github.com/HumanSignal/labelImg>`__ çekilip düzenlenmiştir. Readme dosyası Türkçe'ye çevrilmiş ve kısaltmılmış, Ubuntu 20.04 için kurulum yönergesi düzenlenip geliştirilmiş ve data/predefined_classes.txt düzenlenmiştir. 
  

`Demo videosu <https://youtu.be/dKS-fINMySA>`__

Kurulum
------------------

Ubuntu 20.04 Kurulum
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Ubuntu 20.04 sistemler için kurulum yönergesi

Öncelikle pip yoksa kurulmalıdır.

.. code:: shell

        python3 -m pip --version

Şeklinde kontrol edilir. Eğer versiyon görünmezse aşağıdaki adımlarla kurulur.

.. code:: shell

        sudo apt-get install python3-setuptools
        sudo python3 -m easy_install install pip

Daha sonrasında LabelImg Dosyası git komutuyla indirilir.

.. code:: shell

        git clone https://github.com/wroomhers/LabelImg.git

labelImg klasörüne girilir ve gerekli bağımlılıklar kurulur.

.. code:: shell

        cd labelImg
        sudo apt-get install pyqt5-dev-tools
        sudo pip3 install -r requirements/requirements-linux-python3.txt
        make qt5py3

LabelImg başlatılır ve diğer adımlara geçilir.

.. code:: shell

        python3 labelImg.py

Her kullanım için labelImg klasörüne gidilip başlatılması gerekmektedir.



Ek açıklama görselleştirmesi
~~~~~~~~~~~~~~~~~~~~~~~

1. Uygulamayı başlatın

2. Sol taraftaki Dosya'ya tıklayın ve 'Dizini Aç'ı seçin, ardından size gönderilen verilerin bulunduğu klasörü açın.

3. Dosya Listesi'nde görseli seçin, o görseldeki tüm nesneler için etiket isimleri ve eğer işaretlendiyse kutucuklar görünecektir.



Kısayollar
~~~~~~~

+--------------------+----------------------------------------------+
| Ctrl + u           | Bir dizindeki tüm görüntüleri yükleyin       |
+--------------------+----------------------------------------------+
| Ctrl + r           | Bir dizindeki tüm görüntüleri yükleyin       |
+--------------------+----------------------------------------------+
| Ctrl + s           | Kaydet                                       |
+--------------------+----------------------------------------------+
| Ctrl + d           | Bir dizindeki tüm görüntüleri yükleyin       |
+--------------------+----------------------------------------------+
| Ctrl + Shift + d   | Açık görüntüyü sil                           |
+--------------------+----------------------------------------------+
| Space              | Seçili görüntüyü doğrulanmış olarak işaretle |
+--------------------+----------------------------------------------+
| w                  | Kutu Oluştur                                 |
+--------------------+----------------------------------------------+
| d                  | Sıradaki Görsel                              |
+--------------------+----------------------------------------------+
| a                  | Önceki Görsel                                |
+--------------------+----------------------------------------------+
| del                | Seçili Kutucuğu sil                          |
+--------------------+----------------------------------------------+
| Ctrl++             | Yaklaştır                                    |
+--------------------+----------------------------------------------+
| Ctrl--             | Uzaklaştır                                   |
+--------------------+----------------------------------------------+
| ↑→↓←               | Seçili kutuyu ok yönünde ilerlet             |
+--------------------+----------------------------------------------+

