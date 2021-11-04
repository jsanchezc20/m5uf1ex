[![Spring](https://spring.io/images/spring-logo-9146a4d3298760c2e7e49595184e1975.svg)](https://spring.io/)

## Spring framework
L'**Spring framework** (abreviant, **Spring**), és un [marc de treball][marcTreball] de [codi obert][codiObert] per la [plataforma Java][plataformaJAVA]. La primera versió va ser escrita per _Rod Johnson_, que inicialment va llençar el producte juntament amb el llibre One-on-One Java EE Design and Development.[1] També hi ha un port disponible per la plataforma .NET, Spring.NET.

[marcTreball]:https://ca.wikipedia.org/wiki/Entorn_de_treball_(inform%C3%A0tica)
[codiObert]:https://ca.wikipedia.org/wiki/Codi_obert
[plataformaJAVA]:https://ca.wikipedia.org/wiki/Plataforma_Java

### Funcionalitats clau
* Gestió de la configuració basada en JavaBeans, aplicant-hi principis d'Inversió de Control, més específicament usant la tècnica d'Injecció de Dependència.
* Una factoria de Beans central, que és usada globalment.
* Capa genèrica d'abstracció per la gestió de transaccions de la base de dades.
* Estratègies preincorporades per la JTA i un sol DataSource de JDBC. Això elimina la dependència en un entorn Java EE pel suport a les transaccions
* Integració amb entorns de persistència com Hibernate, JDO, iBatis i db4o.
* Entorn d'aplicació web MVC, construït al nucli de la funcionalitat de Spring. suportant moltes tecnologies per generar vistes, incloent-hi JSP, FreeMaker, Velocity, Tiles, iText i POI.
* Entorn extensiu de programació orientada a aspectes per proveir serveis, com ara gestió de les transaccions. Amb això es millora la modularitat dels sistemes.

### **Mòduls de l'Spring Framework**
>* **Contenidor d'[Inversió de Control](https://ca.wikipedia.org/w/index.php?title=Inversi%C3%B3_de_Control&action=edit&redlink=1)** : configuració de components d'aplicació i gestió del cicle de vida d'objectes Java
>* **Entorn de [Programació orientada a aspectes](https://ca.wikipedia.org/wiki/Programaci%C3%B3_orientada_a_aspectes)** (AOP):
>* **Entorn d'accés a les dades**: treballant amb sistemes de gestió de bases de dades relacionals, sobre la plataforma Java utilitzant JDBC i eines de mapeig objecte - relacional (JPA, Hibernate ...) aportant solucions a reptes tècnics que són reusables en una multitud d'entorns basats en Java.
>* **Entorn de gestió de transaccions**: harmonització de diferents APIs de gestió de transaccions i orquestració de transaccions configuratives per objectes Java.
>* **Entorn model-vista-controlador**: basat en HTTP i Servlet proveint moltes eines per la millora i la personalització.
>* **Entorn d'accés remot**: importació i exportació d'objectes java a la manera de l'RPC (informàtica) configurable, sobre xarxes informàtiques que suporten protocols basats en HTTP, com ara RMI, CORBA, i serveis web (REST).
>* **Entorn d'autenticació i personalització**: orquestració configurativa d'autenticació i processos d'autorització que suporten molts estàndards de la indústria, protocols, eines i pràctiques via el subprojecte Acegi security framework.
>* **Entorn de missatgeria**: registre configurable d'objectes que reben missatges per la consumpció transparent de missatges des de cues de missatges via JMS, millora d'enviament de missatges sobre APIs JMS estàndards. Suport pel protocol AMQP (RabbitMQ, Kafka Broker...).
>* **Entorn de testeig**: suporta classes per la creació d'unitats de testeig i proves d'integració.

### Exemple de codi Spring
```JAVA
@SpringBootApplication
@RestController
public class DemoApplication {
	@GetMapping("/helloworld")
	public String hello() {
	return "Hello World!";
	}
}
```