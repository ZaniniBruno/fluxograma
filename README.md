# fluxogramaflowchart TD
    A[Início do Processo]
    B[Secretaria inicia matrícula]
    C[Gerar link de envio de documentos]
    D[Aluno envia documentos]
    E[Recebimento automático<br/>dos documentos]
    F{Análise documental}
    G[Solicitar correção<br/>ou documento pendente]
    H[Aprovar documentação]
    I[Finalizar matrícula]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F -->|Pendências| G
    G --> D
    F -->|Aprovado| H
    H --> I

