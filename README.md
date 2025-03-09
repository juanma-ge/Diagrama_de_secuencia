# Diagrama_de_secuencia

## Sacar dinero
    @startuml
    actor Usuario
    participant "Interfaz" as I
    participant "Control" as C
    participant "Entidad" as E
    
    Usuario -> I: Solicita el dinero
    I -> C: Valida la solicitud
    C -> E: Verifica saldo
    E -> Usuario: Si es válido, se entrega el dinero
    E -> C: Actualiza el dinero
    @enduml

![image](https://github.com/user-attachments/assets/d9c2f4a1-8c6a-456a-b516-2eb814dd6eba)

## Validación usuario

    @startuml
    actor Usuario
    participant "Interfaz" as I
    participant "Control" as C
    participant "Entidad" as E
    
    Usuario -> I: Ingresa pin
    I -> C: Se mandan y analizan los datos
    C -> E: Valida o no las credenciales
    E -> I: Notifica el mensaje de su validez o no
    @enduml

![image](https://github.com/user-attachments/assets/2044c853-de5b-4776-bb8e-ac4e7ae412ee)


## Interpretación del diagrama de Validación usuario
- El diagrama de secuencia representa la interacción entre los diferentes componentes durante el proceso de validación del usuario.
- Usuario: Inicia el proceso ingresando sus datos en la interfaz.
- Interfaz: Recibe la información y la envía al Control.
- Control: Se encarga de procesar la validación, consultando la entidad **Usuario** para verificar si las credenciales son correctas.
- Entidad: Almacena los datos y responde si estos son válidos o no.

## ¿De que manera te ayuda un diagrama de secuencias durante el proceso de desarrollo del software?

Los diagramas de secuencias son fundamentales en el desarrollo de software porque permite visualizar la interacción entre los diferentes componentes del sistema. Ayuda a identificar la lógica de los procesos y además en un hipotético futuro podría servir para detectar posibles errores o mejoras.

