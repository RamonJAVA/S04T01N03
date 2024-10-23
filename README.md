D04T01
N1
Aquest exercici és un primer contacte amb Spring i Maven.
Amb l'ajuda de la pàgina ->https://start.spring.io/, generem un projecte Spring boot.
A l’arxiu application.properties, configura la variable server.port amb el valor 9000.
Convertirem aquesta aplicació en una API REST:
Creem el subpackage anomenat controller, i dins seu, afegeix la classe HelloWorldController.
Dins tindrem dos metodes que responen a:
                                          http://localhost:9000/HelloWorld
                                          http://localhost:9000/HelloWorld?nom=El meu nom
                                          http://localhost:9000/HelloWorld2
                                          http://localhost:9000/HelloWorld2/elmeunom

N2
Aquest nivell es igual que l'anterior però fent servir un gestor de dependències Gradle.
Generem un nou projecte(aquest cop Gradle) amb ->https://start.spring.io/
A l’arxiu application.properties, configura la variable server.port amb el valor 9001.
Dins del subpackage controller, a la classe HelloWorldController afegirem els dos metodes que responen a:
                                          http://localhost:9001/HelloWorld
                                          http://localhost:9001/HelloWorld?nom=El meu nom
                                          http://localhost:9001/HelloWorld2
                                          http://localhost:9001/HelloWorld2/elmeunom

N3
En aquest nivell provem que els metodes funcionin a traves del software Postman.
Creem dos entorns, un per al projecte Maven i un per al projecte Gradle.
Dins l'entorn, li donem el valor(http://localhost:9000) o (http://localhost:9001) segons el projecte, a la variable {host}
  per a una comprovació més rapida.
A partir d'aqui, i amb l'aplicació en marxa a Intellij, només queda comprovar que les aplicacions API REST responen a les 
  peticions GET.
