# kvadrat
<html xmlns="http://www.w3.org/1999/xhtml"> 
<head> 
<title> Виндхук.</title> 
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/> 
 
    <!-- 
    Подключаем API карт 2.x 
    Параметры: 
    - load=package.full - полная сборка; 
    - lang=ru-RU - язык русский. 
    --> 
    <script src="http://api-maps.yandex.ru/2.0/?load=package.full&lang=ru-RU" 
            type="text/javascript"></script> 
    <script type="text/javascript"> 
        ymaps.ready(init); 
        function init() { 
            var myMap = new ymaps.Map('map', { 
                center: [-22.571583, 17.090736], 
                zoom: 8 
            }), 
                myRect = new ymaps.Rectangle([      
                    [-22.5056, 17.013], 
                    [-22.6299, 17.147]
                ]) 

               ;
                myMap.geoObjects.add(myRect) 
                .add(myGeoObject); 
        } 
</script> 
</head>  
<body> 
<h2>Виндхук</h2> 
<div id="map" style="width:600px;height:400px"></div> 
</body>  
</html>
