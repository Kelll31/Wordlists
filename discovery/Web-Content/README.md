# Списки слов для веб-сканирования

## AdobeCQ-AEM.txt
Используется для: обнаружения чувствительных путей файлов в **Adobe Experience Manager**  
Дата создания: 1 октября 2017 года  
С момента создания этот список не обновлялся.

## AdobeXML.fuzz.txt
Используется для: обнаружения чувствительных путей файлов в **Adobe ColdFusion**  
Дата создания: 27 августа 2012 года  
С момента создания этот список не обновлялся.

## Apache.fuzz.txt
Используется для: обнаружения конфиденциального содержимого на веб-серверах Apache.  
Дата последнего обновления: 26 января 2015 года

## ApacheTomcat.fuzz.txt
Используется для: обнаружения конфиденциального содержимого на серверах Apache Tomcat.  
Дата последнего обновления: 14 декабря 2017 года

## CGI-HTTP-POST-Windows.fuzz.txt
Используется для: эксплуатации различных уязвимостей в устаревшем WYSIWYG HTML-редакторе и инструменте администрирования сайтов, [Microsoft FrontPage](https://en.wikipedia.org/wiki/Microsoft_FrontPage)  
Источник: https://github.com/deepak0401/Front-Page-Exploit  
Дата последнего обновления: 27 августа 2012 года  
Последняя версия FrontPage была выпущена в 2003 году.

## CGI-HTTP-POST.fuzz.txt
Используется для: эксплуатации/обнаружения различных уязвимостей в крайне старых системах (около 1998 года), использующих "CGI".  
Дата последнего обновления: 27 августа 2012 года  

Этот список тестирует следующие уязвимости:
- Уязвимость с использованием пароля по умолчанию в системе телефонной коммутации **[Nortel Meridian](https://en.wikipedia.org/wiki/Nortel_Meridian)**. Источник: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L1167).  
- XSS уязвимость в **"Bajie HTTP JServer"** (сайт программного обеспечения полностью закрыт, архивов нет). Источник: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L803).  
- Уязвимость CGI в неизвестной системе (payload `lastlines.cgi?process`), позволяющая злоумышленникам "читать произвольные файлы и/или выполнять команды". Источник: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L1036).  
- Удаленное включение файлов (**Remote File Include**) в **[myPHPNuke](https://web.archive.org/web/20140812223623/http://www.myphpnuke.com/)**. Источник: [Nessus](https://www.tenable.com/plugins/nessus/11836).   
- DoS атака на **"D-Link Ethernet/Fast Ethernet Print Server DP-300+"**. Источник: [Архив советов по безопасности от Sullo](https://raw.githubusercontent.com/sullo/advisory-archives/master/phenoelit.de_dp-300.txt).

## CGI-Microsoft.fuzz.txt
Используется для: эксплуатации или обнаружения различных уязвимостей в скриптах CGI, работающих на операционных системах Microsoft.  
Дата последнего обновления: 27 августа 2012 года  

## raft-* wordlists
Используются для брутфорсинга директорий и файлов с целью выявления уязвимостей веб-приложений.   
Источник: [Google's RAFT](https://code.google.com/archive/p/raft/)  

## combined_words.txt
Используется для поиска файлов    
Этот список автоматически обновляется через GitHub Action всякий раз, когда любой из списков, из которых он состоит, изменяется.

Данный список является комбинацией следующих списков слов:
- big.txt
- common.txt
- raft-large-words-lowercase.txt
- raft-large-words.txt
- raft-medium-words-lowercase.txt
- raft-medium-words.txt
- raft-small-words-lowercase.txt
- raft-small-words.txt

## combined_directories.txt

Используется для поиска файлов и директорий    
Этот список автоматически обновляется через GitHub Action всякий раз, когда любой из списков, из которых он состоит, изменяется.

Данный список является комбинацией следующих списков слов:
 - apache.txt 
 - combined_words.txt 
 - directory-list-*.*.* и других 

### Использование:
Для поиска файлов и директорий  

### Источник:
Автоматически поддерживается через GitHub Action.

---

## dsstorewordlist.txt

ИСТОЧНИК : https://github.com/aels/subdirectories-discover 

Описание:

Идеальный список слов для поиска каталогов и файлов на целевом сайте с помощью таких инструментов, как ffuf.
- Данные были получены путем анализа сайтов Alexa, входящих в топ-миллион, на предмет наличия файлов **.DS_Store** (https://en.wikipedia.org/wiki/.DS_Store), извлечения всех найденных файлов, а затем извлечения названий найденных файлов и каталогов примерно с 300 тысяч реальных веб-сайтов.
- Затем отсортировал по вероятности и удалил строки с одним совпадением.
- полученный файл, который вы можете скачать, приведен ниже. Удачной охоты!

## vulnerability-scan_j2ee-websites_WEB-INF.txt
Используется для: обнаружения конфиденциальных файлов j2ee, использующих lfi

Рекомендации: 
    
- https://gist.github.com/harisec/519dc6b45c6b594908c37d9ac19edbc3
- https://github.com/projectdiscovery/nuclei-templates/blob/master/vulnerabilities/generic/generic-j2ee-lfi.yaml
- https://github.com/ilmila/J2EEScan/blob/master/src/main/java/burp/j2ee/issues/impl/LFIModule.java


## Frontpage.fuzz.txt
Используется для: Поиска общих путей к файлам на веб-страницах, созданных с помощью **[Microsoft Frontpage](https://en.wikipedia.org/wiki/Microsoft_FrontPage)**

Год первого выпуска Microsoft Frontpage: 1997
Год последнего выпуска Microsoft Frontpage: 2003

Дата последнего обновления: 14 октября 2010


## Web-Server-Java-Servlet-Runner-Adobe-JRun
Используется для: Поиска общих путей к файлам на веб-страницах, обслуживаемых с помощью **[Java Servlet Runner (Adobe JRun)](https://adobe.fandom.com/wiki/JRun)**

Год первого выпуска Java Servlet Runner (Adobe JRun): 1997
Год последнего выпуска Java Servlet Runner (Adobe JRun): 2007

Дата последнего обновления: 14 октября 2010


## Web-Server-Oracle-Sun-iPlanet.txt
Используется для: Поиска общих путей к файлам на веб-страницах, обслуживаемых с помощью **[Oracle Sun iPlanet](https://www.oracle.com/middleware/technologies/webtier.html)**

Год первого выпуска Sun-iPlanet (Adobe JRun): 1994
Год последнего выпуска Sun-iPlanet (Adobe JRun): 2017

Дата последнего обновления: 14 октября 2010


## Web-Server-Glassfish-Sun-Microsystems.txt
Используется для: Поиска общих путей к файлам на веб-страницах, обслуживаемых с помощью **[Glassfish - Sun Microsystems](https://glassfish.org/)**

Год первого выпуска Glassfish: [2005](https://en.wikipedia.org/wiki/GlassFish)
С 2024 года Glassfish продолжает получать обновления.

Дата последнего обновления: 14 октября 2010