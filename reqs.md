# Especificação dos Requisitos do SITCC

## Requisitos Funcionais

### Lista de Requisitos Funcionais

- RF01 - Realizar Login
- RF02 - Login Orientador
- RF03 - Login Aluno
- RF04 - Login Administrador
- RF05 - Organizar Orientacao
- RF06 - Acompanhar Trabalhos
- RF07 - Avaliar Trabalhos
- RF08 - Gerar Ata de Banca
- RF09 - Gerar Certificado dos Professores
- RF010 -Gerar Folhas de Aprovação
- RF011 - Gerar cronograma das bancas
- RF012 - Enviar Arquivo
- RF013 - Receber Arquivo


### Diagrama de Casos de Uso

```plantuml
@startuml Login

package Login{
    usecase "Realizar Login" as UC1
    usecase "Login Orientador" as UC2
    usecase "Login Aluno" as UC3
    usecase "Login Administrador" as UC4
}
package Usuarios{
    actor Administrador as admin
    actor Aluno as aluno
    actor Orientador as ori
}
package Orientacao{ 
    usecase "Organizar Orientacao" as UC5
    usecase "Acompanhar Trabalhos" as UC6
    usecase "Avaliar Trabalhos" as UC7
}
package Documentacao{
    usecase "Gerar Ata de Banca" as UC8
    usecase "Gerar Certificado dos Professores" as UC9
    usecase "Gerar Folhas de Aprovação" as UC10
    usecase "Gerar cronograma das bancas" as UC11
}
package Arquivo{
    usecase "Enviar Arquivo" as UC12
    usecase "Receber Arquivo" as UC13
}
UC1 ..> UC2 : extends
UC1 ..> UC3 : extends
UC1 ..> UC4 : extends
admin --> UC8
admin --> UC9
admin --> UC10
admin --> UC11
admin -> UC4
aluno -> UC3
UC12 <-- aluno
ori -> UC2
UC13 <-- ori
ori --> UC5
ori --> UC6
ori --> UC7
@enduml
```

### Especificicações de Casos de Uso

- [UC_01](reqs_UC01.md)
- [UC_02](reqs_UC02.md)
- [UC_03](reqs_UC01.md)
- [UC_04](reqs_UC01.md)
- [UC_05](reqs_UC01.md)
- [UC_06](reqs_UC01.md)
- [UC_07](reqs_UC01.md)
- [UC_08](reqs_UC01.md)
- [UC_09](reqs_UC01.md)
- [UC_010](reqs_UC01.md)
- [UC_011](reqs_UC01.md)
- [UC_012](reqs_UC01.md)
- [UC_013](reqs_UC01.md)


## Requisitos não-funcionais

### Usabilidade

... Segundo ... Nilsen ...

## Referências

[1] Nilsen ...

[2] Ian Somerville ...

[3] Angular ...

[4] PlantUML ...
