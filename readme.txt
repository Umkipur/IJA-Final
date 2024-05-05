build:
clear && javac --module-path ./lib/ --add-modules javafx.base,javafx.controls,javafx.fxml,javafx.graphics,javafx.media,javafx.swing,javafx.web,javafx.swt --class-path ./src/main/java/ ./src/main/java/ijaproject23/simulation/RobotSimulation.java
run:
clear ; java -Dprism.order=sw --module-path ./lib/ --add-modules javafx.base,javafx.controls,javafx.fxml,javafx.graphics,javafx.media,javafx.swing,javafx.web,javafx.swt --add-opens=javafx.graphics/javafx.scene=ALL-UNNAMED --add-exports javafx.base/com.sun.javafx.event=ALL-UNNAMED -cp ./target/classes ijaproject23.simulation.RobotSimulation
+ argumenty (gridsizeX gridsizeY)

Chyby:
Musel jsem predelat zpetny prehrani, ale moc to nefunguje - radsi neprezentovat
Mazani objektu funguje, ale obcas se neodstrani vizualizace (zkousel jsem ho zpruhlednit i vynutit refresh okna)
Pri simulaci pohybu dvou a vic objektu obcas probliknou - radsi prezentovat roboty samostatne
Neni to v mavenu ani antu
