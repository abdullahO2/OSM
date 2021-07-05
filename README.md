# OSM-city-and-town
في هذه الصفحة استخراج للمدن المضاف عليها عدد السكان بالوسمين:

place=city المدن الكبيرة
![place=city](https://github.com/abdullahO2/OSM-city-and-town/blob/main/place%3Dcity.png)

و

place=town المدن الغير كبيرة
![place=town](https://github.com/abdullahO2/OSM-city-and-town/blob/main/place%3Dtown.png)

على شبكة خرائط الشارع المفتوحة

وذلك عبر الاستعلام التالي الذي تم تنفذيه بواسطة محرر جوسم

```
[out:xml][timeout:9999];

(
  nwr["place"="city"]["population"];
);
(._;>;);
out ids;`
```
--------------------------------------
```
[out:xml][timeout:9999];

(
  nwr["place"="town"]["population"];
);
(._;>;);
out ids;`
```

![image](https://user-images.githubusercontent.com/61907628/124501833-f183a180-ddca-11eb-91f5-c2939dc4577a.png)



