# [linux](https://en.wikipedia.org/wiki/Linux_kernel)

- Linux…是一種自由和開放原始碼(open source)的UNIX-like作業系統。
- The Linux kernel is a free and open-source, monolithic, modular,multitasking(多工), Unix-like operating system kerne
- Linux作業系統的核心(kernel)由林納斯·托瓦茲Linus Torvalds在1991年首次發布。
- [公布在github的linux核心原始碼(Linux kernel source tree)](https://github.com/torvalds/linux)


# 目錄結構
## windows 作業系統目錄結構
```
Windows 作業系統目錄結構==> 有 C: D:

   目錄 C:\Windows\System32 ==>  有許多檔案與子目錄  
   ==> 點選  diskmgmt ==> 開啟 【磁碟管理】 
   ==> 點選  compmgmt ==> 開啟 【電腦管理】    
   
   calc
   notepad
   winword
```
## Linux 作業系統目錄結構 
```
沒有 C: D:

最上層目錄 /
          /etc  ==> 主機或系統配置文件或設定檔絕大部分都在此目錄
          /bin
          /root ==> 最高權限使用者(管理者)登入時的目錄
          /home ==> 一般使用者登入時的目錄
          /home/ksu ==> ksu使用者登入時的目錄     
```
# 實作練習:目錄存取常用指令(linux command)
```
pwd ==>  顯示目前的工作目錄位置(Print Working Directory)

cd ==> 用來變換工作目錄的指令(Change Directory)
cd ==> 回到使用者目錄
cd .. ==> 回到上層目錄
cd /bin ==> 切竄到/bin 目錄

ls ==> 列出目前目錄中的檔案與目錄列表

cat ==> (1)印出檔案內容 (2)合併多檔(concatenate）
  cat flag
  cat /etc/passwd
```
## 指令與參數
```
試輸入底下指令與參數 看看結果有何不同
ls
ls -l   <== 注意:有空格  顯示檔案與目錄的詳細資訊
ls -a    <== 注意:大小寫有區別(Case-sensitive) -a 參數可以顯示隱藏的檔案與目錄
ls -A

可以把兩個參數合在一起
ls -Al

梗多說明請參看
https://blog.gtwang.org/linux/linux-ls-command-tutorial/
```
## pwd 指令語法與參數
```
pwd 的語法:  pwd [OPTION]

參數[OPTION]：
-L 如果當前目錄為連結檔, 會顯示連結檔名稱。
-P: 如果當前目錄為連結檔, 不會以連結檔的路徑來顯示, 會顯示實際的目錄位置。
–help: 顯示幫忙訊息。
–version: 顯示 pwd 版本。
```
## 查閱指令參數小撇步
```
1.直接在terminal 查 
    ls -h
    ls --h
    ls -help
    ls --help
    
2.上網google ==> linux ls

3.man ls
```
## xxd指令
- 上網google ==>linux xxd
- [xxd 簡易使用方式紀錄](https://blog.kalan.dev/2020-03-28-xxd-%E7%B0%A1%E6%98%93%E4%BD%BF%E7%94%A8%E6%96%B9%E5%BC%8F%E7%B4%80%E9%8C%84/)
- [linux 命令 xxd linux下檢視二進位制檔案](https://www.itread01.com/p/1382700.html)

## base64指令
- 上網google ==>linux base64
- [Linux base64 --用base64編解碼](https://www.itread01.com/p/144447.html)

## 找尋資料的find指令
- 上網google ==>linux find
- [Unix/Linux 的 find 指令使用教學、技巧與範例整理](https://blog.gtwang.org/linux/unix-linux-find-command-examples/)
