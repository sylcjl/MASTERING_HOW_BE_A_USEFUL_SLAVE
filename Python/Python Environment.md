##建立Python的環境

 - 方法一：從官網下載   
    Python2.7.11   ([x64](https://www.python.org/ftp/python/2.7.11/python-2.7.11.amd64.msi))([x86](https://www.python.org/ftp/python/2.7.11/python-2.7.11.msi))   
    此為Python最基本環境，只包含基礎套件。   
 - 方法二(建議)：   
    Anaconda   ([x64](http://repo.continuum.io/archive/Anaconda2-4.0.0-Windows-x86_64.exe))([x86](http://repo.continuum.io/archive/Anaconda2-4.0.0-Windows-x86.exe))   
    Anaconda是已經整合過所有非常常用的package安裝檔。   
    內建jupyter notebook(教學使用)、numpy(做data science必備)、scipy(做data science必備，內含Machine Learning套件)等強大套件。
    
   
   
 - [Sublime text 3](https://download.sublimetext.com/Sublime%20Text%20Build%203103%20x64%20Setup.exe) (ST3)   
    * 安裝package control:   
      安裝完成後進入ST3，按下 "```ctrl + ````"，貼上下面程式碼:   
         
      ```import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)```   
    * 上面動作後重新啟動ST3，按下 "```ctrl + shift + p```"，輸入install並選擇install package安裝下面幾個套件：   
      1. SublimeTmpl: 可以快速新增開發模版，包括python, html, javascript, php等   
      2. Anaconda: 可以檢驗python的語法，並有自動完成的功能   
      3. SublimeCodeIntel: 可以檢驗html, javascript等的語法，並有自動完成的功能   
 
 - Jupyter NoteBook
    安裝好Anaconda後，可以開啟Jupyter Notebook，預設網址是[localhost:8888](localhost:8888)   
    教學Python的過程都使用此軟體。
