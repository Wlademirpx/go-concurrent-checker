# Concurrent Service Checker 🚀

Pequeno projeto desenvolvido para estudar concorrência no ecossistema Go utilizando `goroutines` e `sync.WaitGroup`. 

O programa realiza múltiplas requisições HTTP simultaneamente para verificar o status de diferentes serviços, lidando com o fluxo assíncrono e medindo o tempo total de execução da bateria de testes.

## 🧠 Conceitos Praticados

*   Goroutines (Concorrência em Go)
*   Sincronização com `sync.WaitGroup`
*   Requisições HTTP assíncronas
*   Tratamento de erros e HTTP Status
*   Medição de tempo de execução (Benchmarking simples)

## 🛠 Tecnologias

*   **Go (Golang)**
*   Pacotes nativos: `net/http`, `sync`, `time`, `fmt`

## 📂 Estrutura do Projeto

```text
go-concurrent-checker/
 ├── main.go
 ├── go.mod
 └── README.md
 ```

## ▶️ Como executar


1. Clone o repositório:
```
git clone [https://github.com/Wlademirpx/go-concurrent-checker.git](https://github.com/Wlademirpx/go-concurrent-checker.git)
```

3. Entre na pasta do projeto
```
 cd go-concurrent-checker
```

5. Execute o programa:
```
 go run main.go
```


## 💻 Exemplo de Saída
```
Iniciando verificação de serviços...

[200 OK] [https://golang.org](https://golang.org) - Tempo de resposta: 450ms
[200 OK] [https://github.com](https://github.com) - Tempo de resposta: 620ms
[404 Not Found] [https://site-inexistente.com](https://site-inexistente.com) - Falha ao conectar

Todas as verificações concluídas!
Tempo total de execução: 625ms ```
