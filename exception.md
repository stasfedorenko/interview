#### 1. Можно ли RuntimeException обернуть в try-catch?
Да. 

#### 2. В каких случаях не выполнится finally?
* System.exit();
* В потоке-демоне, так как поток-демон внезапно прерывает свою работу. 
* Если в самом finally возникло исключение и нет обработчика, то оставшийся код в finally не выполнится.