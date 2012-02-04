對於中文Windows用戶的一份聲明:

原來host在google code上的項目hosts-generate目前已經二零一零年三月份就放棄繼續開發了. 雖然這個項目目前還有一些用戶, 但我已不再涉足Windows領域了, 因而該項目有的一些問題尚且未能解決, 或者不能滿足各位用戶的需求.

作為替代, 我在linux下使用Perl編寫了一個擁有類似功能的腳本, 並重新host在Github網站上, 如果你在*nix環境下或者在Windows下可以使用Perl解釋器, 依然可以正常使用該腳本來達到你的目的. 你可以在 https://github.com/shouya/hostgenerator 得到它.

為了不辜負用戶的期望, 對這個項目維護的需求, 我希望能夠有一些Windows下的技術人員可以志願接手此項目, 因為我目前沒有時間對此項目繼續開發維護了.

謝謝你的支持.



以下是對該腳本的使用使用說明:

Windows用戶使用說明:
1. 正確安裝一套Perl解釋器, 比較優秀的有ActivePerl和StrawBerry Perl.
2. 下載該腳本和配置文件(host_generator.conf)
3. 切換至有代理的環境, 譬如打開VPN.
4. 打開命令執行器(cmd.exe), 並切換至腳本所在的目錄.
5. 執行perl host_gernerator.pl -c host_generator.conf, 並獲取輸出.
6. 把輸出內容拷貝至C:\\Windows\\system32\\drivers\\etc\\hosts文件之中.


*nix使用說明:
1. 如果在*nix下運行, 請確保你擁有Perl的運行環境(一般而言該類系統自動安裝有Perl解釋器), 可以通過 whereis perl 查看. 如果沒有, 請安裝.
3. 在終端下切換到腳本所在的目錄.
2. 使用git clone獲得腳本.
4. 切換到代理內的環境運行腳本, 譬如VPN或者使用tsocks/proxychains之類的環境.
5. 執行 ./host_generator.pl -c host_generator.conf > tmp 以把結果輸出至一個臨時文件.
6. 查看臨時文件是否正確, 如果無誤, 將之拷貝到/etc/hosts即可.



自由萬歲!
