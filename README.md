# Guia para Configuração do Ambiente Virtual Python

## Passo 1: Criar a Pasta para o Ambiente Virtual

1. **Crie uma pasta para o ambiente virtual**:
   - No seu desktop, crie uma pasta chamada `QA` (se ainda não tiver feito isso).

## Passo 2: Criar o Ambiente Virtual

1. **Navegue até a pasta `QA`**:
   - Abra o PowerShell e execute:

     ```powershell
     cd C:\Users\guilherme.batista\Desktop\QA
     ```

2. **Crie o ambiente virtual**:
   - Dentro da pasta `QA`, crie o ambiente virtual chamado `QA-TESTES-CRM`:

     ```powershell
     python -m venv QA-TESTES-CRM
     ```

## Passo 3: Ativar o Ambiente Virtual

1. **Permitir a execução de scripts no PowerShell**:
   - Execute o comando abaixo para permitir a execução de scripts para o processo atual do PowerShell:

     ```powershell
     Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
     ```

2. **Ativar o ambiente virtual**:
   - Agora, ative o ambiente virtual com:

     ```powershell
     .\QA-TESTES-CRM\Scripts\Activate.ps1
     ```

   - O prompt deve mudar para algo como `(QA-TESTES-CRM)`.

## Passo 4: Instalar Pacotes Necessários

1. **Instale o pacote `selenium`**:
   - Com o ambiente virtual ativo, instale o `selenium`:

     ```powershell
     pip install selenium
     ```

2. **Verifique os pacotes instalados**:
   - Para confirmar que o pacote foi instalado corretamente, execute:

     ```powershell
     pip list
     ```

Agora seu ambiente virtual está configurado e pronto para uso!
