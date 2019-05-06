Varios
Patterns

-SINGLETON
-THE STRATEGY (NormalStrategy, HappyHourStrattegy) 
-THE FACTORY PATTERN
-FLUENT BUILDER

Bases de datos
-Postgres
-Mysql
-Oracle
-Dynamo
-mongodb
-Firebase
-Lokidb
-couchbase


Servidores
	-AWS
	-Openshift
	-mockito

## Testing
- Unit Test
    - mockito
- Integration Test (User histories into test suite)
- Performance TEst
    - Guava stopwatch
    - Revisar el uso de la cpu cuando x metodo esta corriendo
    - New Relic / data dog
    - java mission control
    - j meter / Bees with machine guns
    - behavior Test A test is a behavior test  if it checks if certain methods were called with the correct input parameters

	selenium
	sonar

## Code review
- pull request

## immutabilidaad

## General

### SOLID:   five design principles:    software more understandable, flexible and maintainable
	-Single responsibility
	-Open-closed  "software entities … should be open for extension, but closed for modification."
		A module will be said to be closed if [it] is available for use by other modules. This assumes that the module has been given a well-defined, stable description (the interface in the sense of information hiding).[3].
		The existing interface is closed to modifications and new implementations must, at a minimum, implement that interface.
	-Liskov substitution
		"objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program."
	-Interface segregation
		The interface-segregation principle (ISP) states that no client should be forced to depend on methods it does not use.[1] ISP splits interfaces that are very large into smaller and more specific ones so that clients will only have to know about the methods that are of interest to the
	-Dependency inversion: ISP is intended to keep a system decoupled and thus easier to refactor, change, and redeploy. 
	    inversion de dependencias, inversion de control
		A. High-level modules should not depend on low-level modules. Both should depend on abstractions.
		B. Abstractions should not depend on details. Details should depend on abstractions.

### GRASP: General responsibility assignment software patterns
 patrones generales de software para asignación de responsabilidades,

consist of guidelines for assigning responsibility to classes and objects
patterns: controller, creator, indirection, information expert, high cohesion, low coupling, polymorphism, protected variations, and pure fabrication.

Polymorphism
	According to polymorphism principle, responsibility of defining the variation of behaviors based on type is assigned to the type for which this variation happens. This is achieved using polymorphic operations. The user of the type should use polymorphic operations instead of explicit branching based on type.

### ACID   Cuando se dice que es ACID compliant se indica permite realizar transacciones.

	Atomicidad: Si cuando una operación consiste en una serie de pasos, bien todos ellos se ejecutan o bien ninguno, es decir, las transacciones son completas.

	Consistencia: (Integridad). Es la propiedad que asegura que sólo se empieza aquello que se puede acabar

	Aislamiento: Esta propiedad asegura que una operación no puede afectar a otras. Esto asegura que la realización de dos transacciones sobre la misma información sean independientes y no generen ningún tipo de error.

	Durabilidad: (Persistencia). Esta propiedad asegura que una vez realizada la operación, esta persistirá y no se podrá deshacer aunque falle el sistema y que de esta forma los datos sobrevivan de alguna manera.

### BASE (Basically Available, Soft State, Eventually Consistent


Transactions
	public interface TransactionStatus extends SavepointManager {

    boolean isNewTransaction();

    boolean hasSavepoint();

    void setRollbackOnly();

    boolean isRollbackOnly();

    void flush();

    boolean isCompleted();

}




### REST (Representational State Transfer) es una arquitectura que se ejecuta sobre HTTP.

It should be stateless

It should access all the resources from the server using only URI

It does not have inbuilt encryption

It does not have session

It uses one and only one protocol that is HTTP

For performing CRUD operations, it should use HTTP verbs such as get, post, put and delete

It should return the result only in the form of JSON or XML, atom, OData etc. (lightweight data )

RESTful hace referencia a un servicio web que implementa la arquitectura REST.


As Jason said in the comments, RESTful is just used as an adjective describing something that respects the REST constraints


Sprint Planning, Daily Scrum, Sprint Review, Sprint Retrospective y Sprint Grooming o Refinement	


error vs excepcion

having group by


_________________________________________________________________
FRONT
pruebas unitarias:
- jest, test running and asserting
- mocha. test runner
- chai, asserting
- puppeter, headless browser 

