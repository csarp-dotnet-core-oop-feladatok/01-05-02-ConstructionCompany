# 01-05-02-ConstructionCompany
Osztálychierarchia UML diagram alapján
## Építéssel foglalkozó KFT
Készítsen osztályokat az alábbi UML diagramok alapján:
1. diagram  
![UML](https://github.com/csarp-dotnet-core-oop-feladatok/01-05-02-ConstructionCompany/blob/main/Vehile.png?raw=true)

2. diagram  
![UML](https://github.com/csarp-dotnet-core-oop-feladatok/01-05-02-ConstructionCompany/blob/main/Team.png?raw=true)

3. diagram  
![UML](https://github.com/csarp-dotnet-core-oop-feladatok/01-05-02-ConstructionCompany/blob/main/Company.png?raw=true)

A fejlesztését tesztelje a következő kóddal:  
```
Vehicle fordVehicle = new Vehicle("ford", 400, 5.2);
Vehicle toyotaVehicle = new Vehicle("toyota", 500, 6.3);
Vehicle citroenVehicle = new Vehicle("citroen", 200, 3.6);
Team brickayerTeam = new Team("Köműves", fordVehicle);
Team electricianTeam = new Team("Villanyszerelő", toyotaVehicle);
Team machineMechanicTeam = new Team("Gépésszerelő", citroenVehicle);

ConstructionCompany delKft = new ConstructionCompany("Dél KFT", brickayerTeam, electricianTeam, machineMechanicTeam);
Console.WriteLine(delKft);
```

A kód a következő kimenetet eredményezze:
```
A Dél KFT csapatainak jelenlegi adatai:
Köműves csapat jelenelegi átlagsebessége: 76,92 km/h
Villanyszerelő csapat jelenelegi átlagsebessége: 79,37 km/h
Gépésszerelő csapat jelenelegi átlagsebessége: 55,56 km/h
```
