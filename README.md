# sleepi-firmware  
slee-Pi のためのファームウェアを提供します。  

## 提供ファイル  
以下のファイルがパッケージに含まれています。  

* /boot/overlays/sleepi-overlay.dtb  
  slee-Pi を動作させるための devicetree overlay binary ファイルです。  

* /usr/share/doc/sleepi-firmware/copyright  
  パッケージ内のファイルの著作権を記述したファイルです。  

* /usr/share/doc/sleepi-firmware/changelog.Debian.gz  
  パッケージの変更点を記録したファイルです。  

## 編集ファイル  
インストール時に以下のファイルが変更されます。

* /boot/config.txt  
  以下のエントリが存在しない場合に追記されます。  
  ```
  device_tree_overlay=overlays/sleepi-overlay.dtb
  ```
  
* /etc/modules-load.d/modules.conf  
  以下のエントリが存在しない場合に追記されます。  
  ```
  i2c-dev
  ```
