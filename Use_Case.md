@startuml Login
rectangle login{
    (Realizar Login) ..> (Login Professor) : extends
    (Realizar Login) ..> (Login Administrador) : extends
    (Realizar Login) ..> (Login Aluno) : extends
}
(Login Professor) <-- :Professor: 
(Login Administrador) <-- :Administrador:
(Login Aluno) <-- :Aluno:
@enduml
