#### 1. Какие виды тестов есть? 
#### 2. Как протестировать приватный метод? 
#### 3. Для чего тестировать приватный метод? 
Это может быть полезно в следующем случае. Был публичный метод, он разросся, решили поделить его на несколько маленьких приватных методов. В каждом методе описана какая-то узкая 
логика и ты решил ее поменять. В этом случае полезно протестировать именно этот маленький приватный метод, потому что чтобы протестировать публичный метод нужно много 
дополнительных переменных, которые к твоей задае не относятся. 
