###Zabbix Server v5.0.10 ve agent 5.2.7'de test edildi##

agent active parametresi "server" ile aynı olmalı
"Server=proxy ya da zabbix server"
"ServerActive=proxy ya da zabbix server"
#!burada önemli bir noktaya dikkat etmelisin. Zabbix GUI üzerindeki hostname ile zabbixagent.conf içerisindeki "hostname" aynı olmalı yoksa active agent host bulunamadı hatası verecektir.!

Template üzerinde 411 ID için trigger oluşturuldu,bunu değiştirebilirsin.
Örnek event log event viewer'da "Microsoft-Windows-Kernel-Pnp/Configuration" altında bu yüzden item: "eventlog[Microsoft-Windows-Kernel-Pnp/Configuration]" gibi.
#;
Eğer başka bir lokasyonda olsaydı bunu log ekranındaki "General" tabı altında "Log Name: Microsoft-Windows-Kernel-Pnp/Configuration" path'inde doğrusunu bulabilir buna göre item'i düzenleyebilirsin.
![image](https://user-images.githubusercontent.com/85514498/193821492-4d224d2f-77ca-4bce-9fc4-cd082a3a7340.png)


Template'i import ettikten sonra yukarıdaki bilgileri düzenlediğinde log oluştuğunda veri getirecek ve alarm üretecektir.
