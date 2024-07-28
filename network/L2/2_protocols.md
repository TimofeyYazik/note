#### Ethernet Frame: 
1. Preambula 
2. SFD (появился только в стандарте Ethernet_802.3/802.2 (802.3 with LLC header))
3. Header ethernet
4. Payload – L3 пакет размером от 46 до 1500 байт
5. FCS 
#### Preambula 
Преамбула (Ethernet II занимает 8 байт также известен как DIX Ethernet standard) занимает 7 байт 0хАА и нужна для стабилизации и синхронизации сети
#### SFD (start frame delimiter) 
SFD содержит один байт 0xAB и предназначено для выявления начала кадра  
#### Header Ethernet
1. **Destination mac address**
2. **Source mac address**
3. **Type or length**
d_addr имеет размер 6 байта
s_addr имеет размер 6 байта
type or length имеет размер 2 байта
заголовок предназначен для коммутации

**MAC-адрес** (от [англ.](https://ru.wikipedia.org/wiki/%D0%90%D0%BD%D0%B3%D0%BB%D0%B8%D0%B9%D1%81%D0%BA%D0%B8%D0%B9_%D1%8F%D0%B7%D1%8B%D0%BA "Английский язык") Media Access Control — надзор за доступом к [среде](https://ru.wikipedia.org/wiki/%D0%A1%D1%80%D0%B5%D0%B4%D0%B0_%D0%BF%D0%B5%D1%80%D0%B5%D0%B4%D0%B0%D1%87%D0%B8 "Среда передачи"), также **Hardware Address**, также **физический адрес**) — уникальный идентификатор, присваиваемый каждой [единице сетевого оборудования](https://ru.wikipedia.org/wiki/%D0%9E%D0%BA%D0%BE%D0%BD%D0%B5%D1%87%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%BE%D1%80%D1%83%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85 "Оконечное оборудование данных") или некоторым их интерфейсам в компьютерных сетях Ethernet
### FCS (Frame control sum) 
4 байтное значение CRC используемое для выявления ошибок передачи. Вычисляется отправляющей стороной, и помещается в поле FCS. Принимающая сторона вычисляет данное значение самостоятельно и сравнивает с полученным.
#### Ethernet_802.3/802.2 (802.3 with LLC header)
 Ethernet_802.3/802.2 (802.3 with LLC header) также появились два поля по 1 байту — Source Service Access Point(**SSAP**) и Destination Service Access Point (**DSAP**). Цель, таже самая, – идентифицировать вышестоящий протокол, но какова реализация! Теперь, благодаря наличию двух полей в рамках одной сессии пакет мог передаваться между разными протоколами, либо же один и тот же протокол мог по разному называться на двух концах одной сессии также добавили 1 байтное поле **Control**. Отвечающее, не много, не мало, за Connection-less или же Connection-oriented соединение!
 **Замечание**: Рассматриваемые 3 поля — DSAP, SNAP и Control и являются LLC заголовком.
 (Logical Link Control)